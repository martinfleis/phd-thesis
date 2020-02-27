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

The final set is 74 morphometric characters spanning across the subsets of relational model and covering all categories, even though not equally.\footnote{The balance across categories within the specific set is not required as different categories offer different information relevant for different purposes.} The set is non-overlapping and does not contain logically correlated characters. As such, it should provide unbiased and non-skewed description of each of the elements. 

#### Contextualised characters
Looking at the primary characters and their spatial distribution, they could be really abrupt and do not necessarily capture urban patterns as they are (even though all capture some patterns as per spatial autocorrelation). Two illustrations of such an abrupt change and the weak pattern description are XXX (fig) and YYY (fig). [TODO: ADD EXAMPLES AND THEIR DESCRIPTION]

To become useful for pattern detection within DHC recognition model, most of the characters defined above has to be expressed using their contextualised versions. *Context* here is defined as neighbourhood of each tessellation cell within 3 topological steps on MT. That covers approximately 40 nearest neighbours (median 40, standard deviation ~13.4 based on Prague) providing balance between the spatial extent large enough to capture a pattern and at the same time small enough not to over-smooth boundaries between different patterns (see Annex XXX for sectional diagram analysis). Contextualised character is then capturing a central tendency or a distribution of a primary character within a set context.

Within this method, four types of contextualised characters are proposed. One capturing a local central tendency and three capturing the various kinds of diversity of values within the context. For each of the primary characters, each of the contextualised is then calculated and then used within clustering algorithm itself. The resulting set of used characters is then composed of 4 times 74 characters, giving 296 individual contextualised characters.

##### Local central tendency
Statistics knows central tendency as a measure of a typical value for a probabilistic distribution [Weisberg H.F (1992) Central Tendency and Variability, Sage University Paper Series on Quantitative Applications in the Social Sciences, ISBN 0-8039-4007-6 p.2]. Having a set of data of unknown distribution, central tendency aims to simplify the whole set into one representative number. In the case of morphometric characters, we can measure central tendency of values of a single character across the whole case study, but that would not give us much information. As contextualised characters are defined on three topological steps, it is proposed to measure *local central tendency*, thus a value unique for each building measured as a typical within its immediate context.

Commonly used measures of central tendency are mean, median or mode. Each of them fits a different purposes. To use arithmetic mean to determine central values, underlying distribution should not be skewed, otherwise outliers may significantly affect the resulting value. Mode is, by definition, not suitable for continuous variables like those obtained in primary characters. Median is the most robust of all, measuring the middle value. However, the robustness comes at a cost - the distribution is not reflected at all. Another option is to find a middle ground between easily distorted mean and robust median using truncated mean. Instead of computing arithmetic mean of the whole distribution, we can work with interquartile (smallest and largest 25% are omitted) or interdecile (smallest and largest 10% are omitted) range to minimise the outlier effect on the mean.  

The distribution of values of individual characters vary and in some cases tends to be skewed. As shown in Appendix XXX analysing the difference between mean, interdecile mean, interquartile mean and median (being equal to extremely truncated mean) on a selection of 8 characters, it is clear, that majority of data is rather asymmetric, causing volatility of mean, which should not be used in such cases. The question is then limited to the distinction between median and truncated means (leaving aside midhinge and similar estimators). The data indicate, that the difference between median and interquartile mean is minimal (but still present, e.g., in the case of *shared walls ratio*). As interquartile mean uses more information than median, while being similarly robust to outliers, this research settles on implementation of interquartile mean as a measure of local central tendency. 

##### Diversity as a statistical dispersion
Apart from local central tendency, which aims to capture representative value, it is fundamental to understand how the actual distribution of values within the context looks like. In other words, to capture the diversity of each of the characters. While discussion on importance of  diversity has been central to urban discourse since the era of Jane Jacobs (REF), as shown in the chapter 3, there is not very wide range of characters actually measuring diversity and focus mostly on Simpson's diversity index, originally developed for categorical, not continuous variables and hence relies on pre-defined “bins” (classes of values). For example, @bobkova2017a use this index to measure the diversity of plot sizes, but their binning into intervals based on the actual case-specific values makes the comparability of outcomes limited: if we apply the same formula to another place, we will get different binning. This appears to be a rather ubiquitous problem in applying the Simpson’s diversity index, i.e., it is necessary to set a finite set of pre-established bins prior to undertaking the analysis. However despite the need for urban morphology analysis to produce comparable outcomes, it is difficult to ensure specific descriptiveness to “universal” predefined bins. The use of the Simpson’s diversity index in ecology is encouraged [@jost2006] because ecologists have a finite number of groups enabling them to pre-define all bins appropriately (moreover, bins are usually not defined on a continuous numerical scale), however this is not often the case in urban morphology. The Simpson's diversity index and similar based on binning  provide values specific to individual cases where binning was set and has to be interpreted as such.

Recent literature shows that we now have alternative ways to measure the diversity of morphological characters. @caruso2017 applied the Local Index of Spatial Autocorrelation (LISA) in a form of local Moran’s I, defined as “the weighted product of the difference to the mean of the value of a variable at a certain observation and the same difference for all other observations, with more weight given to the observations in close spatial proximity.“ [@caruso2017, p.84] LISA aims to identify clusters of similar values in space, describing their similarity or dissimilarity, which could be seen as a proxy for diversity, but due to limited number of significant categories (4), its application is limited and rather reductionist.

Another approach grounds the diversity character on the statistical distribution of all measured values and compares it to the ideal distribution. One example is a test whether such distribution follows the principle of the Power Law used by @salat2017, but that is a not straightforward measurement, especially if the distribution is of different shape. Another is an application of the Gini index initially used to measure inequality or entropy-based indices. In the case of diversity, the more unequal the distribution is, the more diverse. Since none of these measurements requires pre-defined grouping, they resolve the problem of binning highlighted above with reference to the Simpson’s diversity index.

Moreover, diversity of continuous variables could be seen as a statistical dispersion, i.e., the ratio to which the distribution is stretched (wide distribution) or squeezed (narrow distribution). Together with central tendency, dispersion is often used to describe the distribution. 

There are multiple ways of measuring dispersion. The most used are probably standard deviation, range or interquartile range as examples of *dimensional* (resulting value have the same units as initial character) measures. Other options would be *dimensionless* (resulting values have no units) and to include Simpson's diversity index mentioned above, *binned* measures. To understand their properties and behaviour on the real morphometric data, wide selection of most relevant from each group is analysed as a way of selecting the most appropriate measures of dispersion/diversity to be used as contextualised characters.

Dimensional measures of dispersion are the most common as they are generally easy to understand and interpret. Similarly to measure of central tendency, all van be measure on the full range of values or on limited, usually again as interquartile (IQ) or interdecile (ID) range. In the analysis are included *standard deviation (SD)*, *range*, and *absolute deviations (median - MAD, average - AAD)*. Both standard deviation and range is measured for IQ, ID and unrestricted range of values. Dimensionless measures are not expressed in the same units as original characters, so while dimensional measure of dispersion for building area will be in meters, dimensionless will have no units (the values are relative). Included are *coefficient of variation (CoV)*, *quartile coefficient of dispersion (QCoD)*, *Gini index*, and *Theil index * (a special case of the generalised entropy index). In terms of binned measures, the key question is not which one should be used, either Simpson's diversity index as in @bobkova2017a or Gini-Simpson diversity index as in Feliciotti (REF), but how to define binning as that can significantly affect the resulting diversity values. For that reason, Simpson's diversity is tested using *natural breaks* REF (number of classes is based on the Goodness of Absolute Deviation Fit (GADF)), *Head Tail breaks* [@jiang2013] Goodness of Absolute Deviation Fit and *quantiles* (5 and 10 bins). Details of the implementation of each are in table \ref{diversity_table} below. The reason for inclusion of Simpson's diversity index, even though it may not be fully comparable across cases is the fact that DHC recognition is always local, always case-specific. However, using the values in further profiling and comparison of clusters across cases (identified separately) might lead to misleading results.

*ADD TABLE WITH FORMULAS*

\newpage

----------------------------------------------------------------
Column 1            Column 2                Column 3
--------------      -------------------     -------------------
Row 1               0.1                     0.2

Row 2               0.3                     0.3

Row 3               0.4                     0.4      

Row 4               0.5                     0.6

----------------------------------------------------------------

Table: This is the table caption. Suspendisse blandit dolor sed tellus venenatis, venenatis fringilla turpis pretium. \label{diversity_table}

Using four morphometric characters as test data - building area, building height, covered area ratio and floor area ratio, all potential measures of diversity listed in table \ref{diversity_table} were measured on three topological steps around each building. Second steps was a visual assessment of resulting maps to eliminate those unfit for pattern recognition, either for relative randomness of result or significant outlier effect (typically present in measures based on unrestricted range of values) (figure XXX). Then was built a correlation matrix of remaining measures for each of the characters and assessed to identify potential overlaps and uniqueness of values. Illustrative correlation matrix\footnote{Complete results of the analysis are available as an Appendix XXX.} based on building area (figure XXX) indicates that intra-group correlation is significant, while correlation between groups less so, suggesting that each of the groups capture different information. For that reason, it might be worth identifying the most suitable of each group and using all three of them as contextualised characters to obtain rich description of underlying distribution of values.

###### Selected diversity characters
Complete analysis of selected measured is available in an appendix XXX. Within dimensional measures, IQ range and IQ SD are better in capturing boundaries between types of development and are robust to outliers. Interquartile range was used by @dibble2017 and is easier to interpret, hence has been chosen as a representative of the dimensional category to be used as contextualised character. 

Differences between tested dimensionless measures are very minor with selection from Theil index, Gini index and Coefficient of Variation, all based on ID or IQ values. Due to tis definition, CoV will tends to infinity when the mean value tends to zero, being very sensitive to changes of mean. Theil index and Gini index are both used to asses inequality, but Theil index, unlike Gini, is decomposable to within-group inequality and between-group differences, making it more suitable for spatial analysis than Gini index would be. ID values used within Theil index are better as the resulting analysis is more sensitive, while outlier effect is still minimal. ID captures, for example, inner structures of blocks better than IQ, where such a structures might be filtered out. In fact, it may help distinguishing between blocks with and without internal buildings, hence second contextualised character will be *interdecile Theil index*. 

I terms of Simpson's diversity index, due to the fact that most of the values follow power-law (or similar exponential) distribution within the whole dataset, binning method has to acknowledge that. For that reason, HeadTail Break are the ideal method as it is specifically tailored to exponential distributions [@jiang2013]. Those which do not resemble exponential distribution should use natural breaks or similar classification method sensitive to the actual distribution, rather than quantiles, which may cause significant disruptions and very similar values may fall into multiple bins causing high diversity values in place where is not.


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
*Non-deterministic nature of GMM*

#### Dimensionality issue
*As resulting morphometric description of each building/cell has ~300 values, we are facing 'dimensionality curse'.*
*possible reduction of dimensionality (PCA, Factor analysis).*
*PCA and how it works*
*Tested PCA results - 95% and ~160, ~30 and 65%*
*We'll have to deal with it and employ a bit more computational power, data are too cleaned to be reduced to PC.*

#### Levels of DHC resolution and its scalability
*Introduce discussion on the resolution of DHC (number of clusters) and scalability of method (exponential growth of resource needs as case study area grows).*

##### Selection of number of components
Gaussian Mixture Model clustering requires, similarly to k-means, specification of number of components of the model (i.e., clusters) prior clustering. However, that number is usually not known, especially in the case of urban form. Assumptions can be made based on the expert knowledge, but that would limit the application and unsupervised nature of the whole process and go essentially against the prepositions set in chapter 5. 

The way around is to estimate the ideal number of components based on the goodness of fit of the model for each of them. That essentially means that the GMM is trained multiple times based on range of feasible options of number of components and each of the models is then assessed against the whole dataset (how well are clusters distinguished). The assessment is of a quantitative statistical nature, keeping the method relatively unsupervised. The only input researcher needs to make at this stage is an interpretation of the resulting values and the curve of goodness of fit to specify the number of components for the final clustering.

###### Goodness of fit
The goodness of fit measures a fit of a trained model to a set of observations (e.g., the original dataset)REF. It describes how consistent is the distribution of clustered model to the distribution of the whole dataset, to put it in simple words. With K-means clustering is often used silhouette method REF, which could in theory be used with GMM as well. DEFINE Another option is measuring average log-likelihood score DEFINE, which is SOMETHING. 

*Silhouette, score, BIC, AIC, BIC gradient, TT distance intro*


*We use BIC, BIC gradient and TT distance due to…*


Non-deterministic nature of GMM means that each of the trials should be repeated multiple times to understand what is the confidence interval of possible outcomes. Testing each number of components only once might lead to incorrect interpretation of results. The ideal situation is to compute multiple runs (the higher the number, the better the result) of each option and plotting the confidence interval to help with the interpretation later.

The interpretation of the goodness of fit score is not question of comparing the numbers only, but understanding the resulting curve. In theory, the lower the BIC score is the better the model fits the original data. However, it has to be kept in mind that there is a certain confidence interval and that BIC itself penalises higher number of clusters. The optimal number is not always the one which reaches the lowest BIC score, especially if the score is within the confidence interval of other options. The aim of the clustering is to simplify the whole dataset into the smallest number of meaningful clusters, but not too small. Hence in the situation with multiple options within the same confidence interval, we should select the first significant minimum,REF i.e. the smallest number of components which has its mean score within the confidence interval of the numerically best fit. 


###### Stability of procedure
*There is a certain effect of randomness in the process, so clustering comes with a confidence interval*
*the answer of clustering is never fixed, there is certain variability*
*confidence interval should help us in interpretation*
*there is an issue of multiplication of computational demands*

##### Sample-based clustering
As the dataset grows, it may become increasingly impossible to run clustering on the whole dataset, especially if we want our data with meaningful confidence interval. The calculation of dimensions between components of the model in hyperspace of 296 dimensions is a demanding task requiring time and computational power. While data for Prague (~140 000 features) could be processed on a desktop with modern multi-core processors within days (multiple options with a confidence interval, not a single run), that is not true for larger metropolitan areas where number of feature can reach millions. The data like this can be run in a same way on cloud-based services providing significantly more computational power and servers tailored to data analysis, but this solution can be costly.

For that reason, it might be worth training the method on sampled data before classifying the whole dataset. Instead of using all features to train the model, randomly samples subset could be used as a training set for GMM, which, once fitted, could be used to classify the whole dataset. This solution lowers computational demands as the number of features used in the learning process is smaller, but there are also issues with it. The random sample should reflect the structure of the whole dataset to provide results comparable with GMM trained on the whole dataset. However, that is never fully true. The larger the sample is, the more similar to the whole data is, but at the same time the effect of sampling on computation is becoming less significant. Even larger samples may, in some cases, miss smaller clusters present in the full-data clustering as features composing these cluster would not be present in the sample (the smaller the cluster, the higher the probability than it will be missed in the sample).

The decision whether train GMM on the full of sampled data should reflect the balance between what is ideal (full) and what is possible in certain conditions. The different options of sample-based clustering are tested and compared to the default clustering in following section, to assess the behaviour of sample-based clustering in the case of Prague. The behaviour will be likely different at different places as the real structure and distribution of values affects the sampling-effect. Places with more diverse structure and number of smaller cases will be probably affected more than places with homogenous structure where the likelihood of proper sampling of all clusters is higher.

##### Subclustering
*sometimes our cluster are too big and we want better resolution*
*clusters defined by the lowest score can still be splitter as the dataset is rich, when appropriate*
*iteration of the clustering method on a sample of one (stable) cluster*
*relation to other clusters is different and has to be interpreted as such*
*the other way, joining clusters to larger groups, will be discussed in the next chapter*

### Data preprocessing
Before doing any of these steps, it is fundamental to ensure that data are good enough to represent morphological/morphometric elements. That could be an issue for both building and street network layers, so there are cases when the data needs to be prepared for morphometric analysis. The preprocessing can be in some cases automatised, in other, unfortunately, manual or at least semi-manual to have the data in the correct shape in the end.

While each dataset coming from different source is specific hence the cleaning procedure needs to be tailored to each source, there are some common issues which are not unique to specific datasets. Following section outlines these common issues and how to resolve them or at least minimise the error under the significant level. As the method described above is error-prone due to the design of contextualised characters, the data do not have to be perfect all the time. However there are cases where even contextualised character can be significantly affected and skew the result of clustering.

#### Preprocessing of buildings
Having data layer correctly representing building footprints is crucial from two reasons as it not only affect morphometric characters based on buildings, but also morphological tessellation and consequently characters based on morphological cells, which in the end are all contextualised characters.

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
