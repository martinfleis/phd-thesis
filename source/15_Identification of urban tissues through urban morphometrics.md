# Identification of urban tissues through urban morphometrics
*intro as a link back to theory in chapter 4 and 6 reintroducing morphometrics and numerical taxonomy*
*the aim of this chapter is to develop a morphometric method able to distinguish distinct types of urban tissues*

The aim of this chapter is to provide theoretical and practical grounds to the novel method allowing automatic detection of distinct types of urban tissues. Similar research has been done before (REF), but it was never linked to the coherent theory of morphometrics and numerical taxonomy, nor it was both rich in terms of number of characters used within a model and the spatial extent (see Chapter 3). Following pages present a method which aims to be both inclusive as per morphometric characters and at the same time automatised and efficient to allow for examination of large datasets spanning across metropolitan regions.

Following chapter will introduce key principles of systematic morphometric description, which will be later applied to the methodology. Then it will outline the basis for the recognition of distinct homogenous clusters (DHC), from the selection and definition of morphometric characters to unsupervised classification using Gaussian Mixture Model clustering. Methodological proposition will be later tested on the case of Prague, Czechia. 

## Principles of systematic morphometric description
*Restate principles of numerical taxonomy in biology*
In the context of the whole research, theory of numerical taxonomy is applied twice - in the DHC recognition and then in development of a taxonomy (Chapter 8).

*Link to the urban form and this specific methodology*
*Systematic methodology means that it is…*
*Comprehensive methodology means that it is…*
*This method is trying to be both by…*

## Methodological proposition

The detection of DHCs within their spatial context is not simple nor straightforward process. The design of the method consist of several steps outlined in the following section. The first step is definition of principles of DHC recognition which are then followed  as subsequent steps through the rest of the method design, and consequently reflected in the structure of the section. 

### Principle of DHC recognition

Recognition of DHCs is based on the principles we know from numerical taxonomy, but is a slightly specific way. In biology, the issue of individual delimitation is non-existent. Single individual of selected species is usually well defined in space (e.g., a bird), however in urban form this distinction is not so simple. Hence, the methodology which is used in biology needs to be adapted, while keeping the fundamental principles in place. The specificity is in the shift of the scale. While previous chapters identified urban tissue as *individual* of urban form, at this stage we pretend that this role holds duality building-tessellation cell as the smallest entity of urban form. The whole DHC recognition is then based on the assumption that entities recognised as a part of the same cluster (*species*) are, in fact, elements of the single urban tissue (where continuous) or of multiple individuals of the same kind of urban tissue (where discontinuous). 

Another difference between traditional method outlined by numerical taxonomy and the one adapted for the purpose of DHC recognition is the nature of morphometric characters. While in biology, each individual is usually measured independently of the rest (REF), that is not viable for urban form. The overall aim is to identify built-up patterns within urban fabric. However, the urban form itself is full of exceptions form the pattern. Individual plots follow different development process and are in some cases amalgamated or split. That does not happen tot he rest of the same tissue at the same time (while it might or might not later), causing the constant emergence of exceptions from the pattern. To overcome the issue of exceptions, proposed method is working with two kinds of characters - primary and contextualised.

The primary characters are those focusing on the individual elements  and their relationships as identified in a relational model (Chapter 6). Typical example could be building height or area. Both are specific to each individual building and in the context of plots with internal construction, buildings in the head and the back of the plot will have significantly different values.

As primary characters by definition do not describe the pattern but rather its individual elements, they should not be used within pattern detection algorithms. The second kind of characters, contextualised, has been designed specifically to turn values captured by primary characters into values describing the central tendency in the area - describing the pattern.  As such, they can be used as an input for clustering aiming to distinguish DHCs.

Finally, the data captured by contextualised characters are used to cluster individual building-tessellation cell entities to statistically homogenous clusters each capturing distinct kind of urban tissue. 

Following section will detail the use of primary characters, contextualised characters and the clustering method itself.

### Morphometric characters
The main scope of this research is not to develop new morphometric characters (even though there are some), but to use existing knowledge in urban morphometrics and combine it in a complex coherent framework. The chapter 3 mapped in detail the existing characters used across the field and the resulting database and classification is the basis for selection and definition of primary characters and to some extent even contextualised characters. 

#### Primary characters
As briefly outlined above, primary characters describe different elements and their relationships as are identified within the relational model of urban form. Adapting the definition of the term *primary* from Oxford English Dictionary (REF), we can define primary characters witting the context of DHC recognition as *characters occurring first in a sequence of methodological steps capturing individual features of urban form elements and their basic relations*. The link to the relational model is crucial here as it defines which relations are meant and later reflected in the whole recognition model.

Chapter 3 shows that there is a large number of characters which could be, in theory, used within the model. However, the selected set of characters needs to have specific nature. The information captured should be non-overlapping, each of them should describe different unrelated feature of urban form to avoid clustering result distortion towards features occurring multiple times. For that reason, specific principles of characters selection were defined.

##### Principles of character selection and definition
*To select set of primary characters, following principles are followed.*
*rules based on relational model and characters classification*
*rules based on Sneath and Sokal (check with Annex 2)*
*Initial selection and then expansion*
*cleaning of the selection (check with rules above)*
*full details of the steps are in Annex 2*

The process of selection itself starting form the database retrieved from chapter 3 and details of each decision which characters should be part of the final set and why is available as Annex 2. Following section describes the final set only.

##### Identified set of primary characters
Based on the principles described in the section above, following morphometric characters compose the final set of primary characters. For detailed description of each character and its implementation please refer to the original reference and to the documentation and code of momepy.

*LARGE TABLE OF CHARACTERS WITH FORMULAS AND REFERENCES*

The final set is 74 morphometric characters spanning across the subsets of relational model and covering all categories, even though not equally.[^The balance across categories within the specific set is not required as different categories offer different information relevant for different purposes.] The set is non-overlapping and does not contain logically correlated characters. As such, it should provide unbiased and non-skewed description of each of the elements. 

#### Contextualised characters
Looking at the primary characters and their spatial distribution, they could be really abrupt and do not necessarily capture urban patterns as they are (even though all capture some patterns as per spatial autocorrelation). Two illustrations of such an abrupt change and the weak pattern description are XXX (fig) and YYY (fig). [TODO: ADD EXAMPLES AND THEIR DESCRIPTION]

To become useful for pattern detection within DHC recognition model, most of the characters defined above has to be expressed using their contextualised versions. *Context* here is defined as neighbourhood of each tessellation cell within 3 topological steps on MT. That covers approximately 40 nearest neighbours (median 40, standard deviation ~13.4 based on Prague) providing balance between the spatial extent large enough to capture a pattern and at the same time small enough not to over-smooth boundaries between different patterns (see Annex XXX for sectional diagram analysis). Contextualised character is then capturing a central tendency or a distribution of a primary character within a set context.

Within this method, four types of contextualised characters are proposed. One capturing a local central tendency and three capturing the various kinds of diversity of values within the context. For each of the primary characters, each of the contextualised is then calculated and then used within clustering algorithm itself. The resulting set of used characters is then composed of 4 times 74 characters, giving 296 individual contextualised characters.

##### Local central tendency
*central tendency is, local central tendency is …*
*Mean, IQ, ID, Median as options, including truncated versions*
*Interquartile mean (def) is used because…*

##### Diversity as a statistical dispersion
*apart from central tendency, we need to understand the diversity of values within the immediate context of each building*
*diversity on continuous values could be seen as statistical dispersion*
*there are multiple ways of measuring dispersion, many were analysed*
*three main (largely correlated) groups are there - absolute, unitless, binned*
*absolute are these*
*unitless are those*
*binned are that*
*Analysis of selection as an annexe*

###### Selected diversity characters
*interquartile range definition*
*interdecile Theil definition*
*Simpson diversity index definition, bin issue and solution*
*Each of the primary characters is represented by its local central tendency and local diversity (using all 3 characters)*
*Conclude contextualised characters*
*conclude all characters*

### Gaussian clustering
*Once we have a description of individual elements, we have to cluster them to identify DHC*
*General principle of clustering aka unsupervised machine learning*
*Short overview of available methods and differences in their application*

#### Gaussian Mixture Model clustering
*introduction of Gaussian Mixture Model clustering and explanation of its selection and potential issues*
*relation to k-means*
> k-means clustering tends to find clusters of comparable spatial extent, while the expectation-maximization mechanism allows clusters to have different shapes. (https://en.wikipedia.org/wiki/K-means_clustering)
*definition based on gaussians*
*probabilistic (soft clustering); given a data point x, what is the probability it came from Gaussian k*
*Expectation — Maximization algorithm*
*Scikit-learn implementation is used, for detail see REF.*

#### Dimensionality issue
*As resulting morphometric description of each building/cell has ~300 values, we are facing 'dimensionality curse'.*
*possible reduction of dimensionality (PCA, Factor analysis).*
*PCA and how it works*
*Tested PCA results - 95% and ~160, ~30 and 65%*
*We'll have to deal with it and employ a bit more computational power, data are too cleaned to be reduced to PC.*

#### Levels of DHC resolution and its scalability
*Introduce discussion on the resolution of DHC (number of clusters) and scalability of method (exponential growth of resource needs as case study area grows).*

##### Selection of number of components
*we have to set number of components (clusters)*
*trial of many options*
*test the goodness of each number*

###### BIC, AIC, etc.
*Introduce measures of goodness of clustering*
*Silhouette, score, BIC, AIC, BIC gradient, TT distance intro*
*We use BIC, BIC gradient and TT distance due to…*
*Interpretation of scores is another question*
*we can go with lower number of clusters to maximise stability of procedure (may incur under-fitting) or with the smallest BIC (might be overfitted). However, as the next step is hierarchical clustering, we can use its help in interpretation of smaller clusters.*
- [thoughts only] score is always only indicative, it will not give us a one final answer. There are generally two options - go for conservative clustering (elbow), which might be the best idea in this case, or go for the true minimum. However, there is a clear possibility of overfitting and the minimum can be influenced by the penalisation of BIC. Conservative clustering (15 clusters in this case) will likely need sub-clustering to get a better detail.

###### Stability of procedure
*There is a certain effect of randomness in the process, so clustering comes with a confidence interval*
*the answer of clustering is never fixed, there is certain variability*
*confidence interval should help us in interpretation*
*there is an issue of multiplication of computational demands*

##### Sample-based clustering
*As the dataset grows, it may become increasingly impossible to run clustering on the whole dataset, especially if we want our data with confidence interval.*
*For that reason, it might be worth training the method on sampled data before classifying the whole dataset.*
*There are an issues linked to it.*
*It is always a balance between what is ideal and what is possible.*

##### Subclustering
*sometimes our cluster are too big and we want better resolution*
*clusters defined by the lowest score can still be splitter as the dataset is rich, when appropriate*
*iteration of the clustering method on a sample of one (stable) cluster*
*relation to other clusters is different and has to be interpreted as such*
*the other way, joining clusters to larger groups, will be discussed in the next chapter*

### Data preprocessing
*Before doing any of these steps, we have to make sure that our data are good enough to represent morphometric elements*
*sometimes we need to preprocess data to have them in a correct shape*

#### The common issues with input data
*there are some common issues which are not unique to specific datasets, which needs to be resolved and some of them can be dealt with algorithmically*

#### Preprocessing of buildings
*to ensure precise results of tessellation and building-based characters*
*topologically correct*
	*joined where joined*
	*non-overlapping*
*the detail should be consistent - overly detailed shapes are bad, overly simplified as well*
*buildings needs to come as one polygon - so either some way of splitting (complicated) or dissolving (depends on the data) needs to be employed*
*missing height attribute*
*it is not so complicated to find cases with ideal data, but these are not everywhere, esp. with height*

#### Preprocessing of street network
*to ensure topologically correct network representing streets in morphological terms*
	*correctly splitted*
	*representing morphology, not transport*
	*definition of what is street and what is not (lanes)*
*transport-based network is fairly available, there are ways (not 100% though) how to generate morphological out of it*
*conclude preprocessing*

*conclude methodology*

## DHC recognition | Case study Prague
*Application of the whole methodology to the case study of Prague*

### Primary characters
*illustration of primary characters on parts of Prague*
- Few examples, rest in Appendix

### Contextualised characters
*illustration of contextualised characters esp. in relation to primary ones*
- Few examples, rest in Appendix?

### Clustering
*introduction of clustering - abc will happen*

#### Complete  data
*BIC*
*BIC gradient*
*TT distance*
*Interpretation of score*
*map and its (basic, as detailed is in Ch8) interpretaion*

#### Sampled data
*Score*
*BIC*
*BIC gradient*
*TT distance*
*Interpretation of score*
*Comparison of sampled and complete*
	*compared graphs and statistical values*
	*compared resulting clustermaps*

#### Probability of cluster (change)
*note on probability of cluster assignment*
*due to the richness of data, clusters are very well defined, there is probability but they are insignificant*

#### Subcluster illustration
*Sub-clustering question test on compact urban form (perimeter blocks and modernism)*

##### Compact Prague 
*BIC and others*
*Map*
*Interpretation*

##### Modersnist Prague 
*BIC and others*
*Map*
*Interpretation*

## DHC as an urban tissue
*morphometric characters certainly help in description of urban tissues*
*clustering helps make sense out of it*
*DHC is a numerical, morphometric statistical proxy of urban tissue*
*Clustering is non-deterministic, so boundaries are not fixed, rather indicative.*
*It is not a ground truth and the meaning and relation of clusters has to be interpreted before any further steps*
*hierarchical clustering will help with that*
