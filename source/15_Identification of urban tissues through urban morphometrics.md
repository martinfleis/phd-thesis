# Identification of urban tissues through urban morphometrics
*intro as a link back to theory in chapter 4 and 6 reintroducing morphometrics and numerical taxonomy*
*the aim of this chapter is to develop a morphometric method able to distinguish distinct types of urban tissues*
*this chapter goes to aim by (slight contents overview)*

## Principles of systematic morphometric description
*Restate principles of numerical taxonomy in biology*
*Link to the urban form and this specific methodology*
*Systematic methodology means that it is…*
*Comprehensive methodology means that it is…*
*This method is trying to be both by…*

## Methodological proposition
*intro - method introduces several steps to get to DHC recognition*

### Principle of DHC recognition
*DHC recognition is using the principles we know from numerical taxonomy, but in a specific way*
*characters are of dual nature due to the nature of urban form - one big exception*
***primary** characters are those focusing on elements based on relational model and their relationships*
***contextualised** characters are capturing the central tendency*
*contextualised characters are then used as an input for clustering aiming to distinguish DHC*
*following sections detail the principle*

### Morphometric characters
*going back to chapter 3 for a resource*

#### Primary characters
*primary characters are those (define), link to relational model*
> Primary: Occurring or existing first in a sequence of events; belonging to the beginning or earliest stage of something; first in time (OED)
*there is a large number of possible characters, but the set needs to be specific, non-overlapping etc.*

##### Principles of character selection and definition
*To select set of primary characters, following principles are followed.*
*rules based on relational model and characters classification*
*rules based on Sneath and Sokal (check with Annex 2)*
*Initial selection and then expansion*
*cleaning of the selection (check with rules above)*
*full details of the steps are in Annex 2*

##### Identified set of primary characters
*based on the principles, following characters compose the final set of primary characters*
*LARGE TABLE OF CHARACTERS WITH FORMULAS, ignore definitions*
*conclude primary characters*

#### Contextualised characters
*primary characters could be abrupt and do not necessarily capture patterns as they are*
*To follow the principles of DHC recognition, most of the characters tested above has to be expressed using their contextualised versions*
*That is calculation of central tendency and diversity characters for each one of them within 3 topological steps on MT. These characters will then be used within clustering algorithm itself.*

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
