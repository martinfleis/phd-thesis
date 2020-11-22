\setcounter{chapter}{7}

# Taxonomic relationships of urban tissues

The previous chapters introduced the framework implementing comprehensive urban morphometrics on a metropolitan scale. Based on the selection of measurable characters, it established a method of a complex description of urban form on the granularity of individual buildings. As reported, derived information then enabled the identification of urban tissue types within urban form. Consequent results of the cluster analysis indicate the validity of morphometric method in recognition of urban form patterns and the potential for both additional subdivision and upscaling of the model.

In this chapter, therefore, the observed clusters are employed in the role of input data and investigated from two perspectives - 1) conceptualisation of clusters as *OTUs*, leading to the taxonomic classification, 2) validity of clusters as a proxy of urban tissues via assessment of relation to additional data, the transferability of the method to the different geographical context, and expandability of the taxonomy.

This chapter relates back to chapter 3 and introduces numerical taxonomy of urban tissues. The resulting classification is subsequently validated together with initial clusters based on the study of its relationship to the supplementary, non-morphological data known to be descriptive of urban form. Finally, the case study of Amsterdam is included to examine the ability of the proposed morphometric framework to identify urban tissues in the context of another heterogenous historical city, although of different patterns of development. 

Structurally, this chapter is divided into two major parts. It first outlines the need for a classification of urban tissues (section \ref{need_taxonomy}) and bridges the concept of numerical taxonomy from chapter 3 to the context of morphometric tissue types (section \ref{taxonomy_as_method}). Furthermore, it explains the importance of validation and two validation models used within this study (section \ref{need_validation}).

The two major parts are Methodological proposition (section \ref{method_prop8}) and Case studies (section \ref{case8}). The structure of the methodological section is reflected in the structure of case studies, having each part of the proposed method tested in the relevant part of the associated case studies section.  

Methodological propositions first introduce the method of hierarchical clustering, leading to the taxonomy of urban tissues (section \ref{hierarch_method}). Moreover, the results are utilised in the next section \ref{meth_validation} establishing the method of validation of identified urban tissues and their taxonomy, using data on historical origin, land-use patterns and qualitative classification of urban areas. Finally, the second part of the section \ref{hierarch_method} brings in another case study (Amsterdam) and presents the method of evaluation of transferability of the morphometric assessment. The evaluation focuses on the identification of urban tissue types, their hierarchical classification and combination of two geographically distinct datasets to a single taxonomy, examining the expandability of the method. Following section \ref{case8} presents the results of proposed method applied to case studies in the same order and hierarchy of sections.

The final section (\ref{conclusion8}) of the chapter summarises the findings and prepares the foundation for chapter 9, synthesising and discussing the whole research.

## Classification and validation \label{need_taxonomy}
The urban tissue types presented in the previous chapter are all seen as equal, meaning that there is no specified relationship between them at this stage. However, the degree of similarity between individual clusters varies and can be quantified. Therefore, a numerical representation of similarity, based on already measured morphometric characters, becomes a basis for the further classification of urban tissues. 

As illustrated in the chapter 2, there have been attempts to deliver classification frameworks, some even taking hierarchical structure but still deviating from the *optimal classification model*. This section proposes application of biological model of classification in a form of a numerical taxonomy leading to the establishing hierarchical classification as a conceptual basis for the *atlas of urban form.*

However, the model of identification of urban tissues and their classification needs to be validated. There are two critical questions regarding the validity which needs to be answered:

1. Are morphometric clusters a valid proxy of urban tissue types?
2. Is the method transferable outside of the context of initial case study?

To answer the first question, this chapter introduces a validation as an  assessment of relation of the tissue types and their taxonomy to additional data, which are known to be linked to the form of cities. The significant relationship between them and proposed clustering and classification would therefore indicate their validity and the validity of the proposed method. The second question requires inclusion of another case study from a different geographical and historical context. Clusters identified in that case study should be internally valid and comparable with those identified in Prague. 

### Taxonomy of tissue types \label{taxonomy_as_method}

Resulting clusters can be theoretically interpreted, in a conceptual sense, as populations and studied as such.  Based on the propositions outlined in the chapter 3, biological analogy is taken further in this chapter, to propose a numerical taxonomy of urban form. The operational taxonomic unit (OTU) in this case is a morphometric urban tissue type. Each cluster as a whole is considered as a unit for the classification, conceptually mirroring classification on the level of populations, following the principles of numerical taxonomy [@sneath1973] with only a minor adaptations related to the specificity of urban form.

Urban form is traditionally classified not in a taxonomic, but in a typologic way [@kropf2017]. Where taxonomy is based on quantitative relations between its elements, typology follows conceptual division [@bailey1994]. Both approaches are valid as they assess the same entity (urban form) from a different perspective. Moreover, if the classification results coincide, the method can validate each other. This study aims to explore the potential of quantitative description of urban form, hence it is natural that it chooses the path of taxonomy.

The taxonomy results in the hierarchical tree capturing the relationship of clusters, or *taxa*. That allows agglomeration of the lowest-level taxa into higher level ones, adaptively changing the resolution of  classification. That is especially helpful for studies assessing the effect of urban form on socio-economic aspects as it can adapt to coarser data.

### Validation and applicability \label{need_validation}
Validation is an assessment of correctness of a result. In the context of this work, validation should mainly focus on the understanding whether the identification of urban tissue types works as intended and whether the method is transferable to other contexts and eventually extensible.

The validation of a clustering method which does not have a ground truth data is always indirect. That means that any validation procedure can give only an indication of the method's performance, not a precision estimate. To make the validation more robust, it is better to compare results to more than a one validation layer. Furthermore, it is critical to ensure that literature identifies that there is an expected relation between the concept validation layers capture and urban form patterns.

Transferability of the proposed method should be tested by its application on other case studies and validating the results independently of the first one. If the method produces reasonable results and validation via proxy layers indicates statistical relation, we can assume that the method is transferable to contexts in which it was tested.

Finally, expandability of hierarchical classification (i.e. taxonomy) is critical for the future development of a taxonomy of urban form. The method is extensible if the results of tissue type identification from one case can be successfully linked to tissue types from the other case to build a common taxonomy.

The following section first proposes a method of hierarchical clustering to derive the basis for a taxonomy of urban form. Then it outlines methods of validation using the test of relation to proxy layers, transferability to different context and finally, expandability as an attempt to merge two cases into a single classification. 

## Methodological proposition \label{method_prop8}
Methodological propositions of this chapter focus on two distinct questions. The first one has been defined in chapter 5 as one of the supplementary research questions:

1. How to determine the taxonomic relationship between OTUs to derive taxa of urban form?

To answer that, this section proposes the application of hierarchical clustering method outlined below.

The second question is related to the both results of the previous chapter 7 and hierarchical clustering proposed in this chapter:

2. Is the overall method valid for classification of urban form?

That is a question which is critical but at the same time hard to answer. Therefore, this section proposes a series of tests to get a reliable indication of what the answer could be.

### Hierarchical clustering \label{hierarch_method}
Hierarchical clustering in case of urban tissues aims to develop a hierarchy of similarities between observations based on their morphometric profiles. We can generally distinguish two main principles, agglomerative and divisive. The former starts with the pool of observations each with its own cluster and identifies pairs of clusters while moving up the hierarchy. The latter does the opposite as it starts with a single cluster and iteratively divides it while moving down the hierarchy. Statistics offer a wide range of procedures for both principles, which description is out of scope of this research. This research employs Ward's minimum variance hierarchical clustering, as the method with a long lineage in academic use [@singleton2009] and recent application in urban morphology [@serra2018a; @dibble2017]. Each tissue type is represented by its centroid (mean of each character) within the hyperspace  and the Ward's algorithm agglomeratively links observations together in a way, which minimises an increase in total within-cluster variance [@ward1963hierarchical]. The classification has a form of a dendrogram capturing a cophenetic relationship between observations (i.e., morphometric similarity).

Resulting dendrogram can be further interpreted and initial OTUs flexibly clustered together based on the branching of the diagram. That can in turn be mapped and the spatial distribution of branches can be visually assessed. Furthermore, branching enables focused analysis of individual macro clusters, if that is of interested of one's particular study. 

### Validation \label{meth_validation}
Validation of identification of tissue types and consequent hierarchical clustering is done in two ways. The first one studies the relationship of resulting classification to additional non-morphometric data to verify whether the expected link between morphology and other aspects is present in the data. The second approach tests the applicability of the method outside of the initial case study. As the design and decision making behind it was based on the Prague dataset, it may have incurred context-specific features which limits the applicability of the method elsewhere. To ensure that this did not happen, the method should be applied to unrelated data and resulting classification should be examined to ensure that the results are comparable.

#### Relation to non-morpohological data \label{meth_validation_rel}
Capturing the relation of proposed classification to additional data is an indirect validation method. There are theoretical grounds on which we can expect that the relation between urban form and other data exist and hence should be present in the classification. It is well known that urban patterns change based on the era in which they are built, meaning that there is a significant relation between urban types and their historical origin [@dibble2017; @panerai2004]. Similar relation could be find with land use patterns [@castro2019] and some other data. 

However, such additional data should not be seen as a ground truth for classification as it does not reflect the same concepts. The relation should be seen as indicative. 

In this research, proposed classification will be compared to three datasets -  1) the period of historical origin of a place, 2) predominant land-use patterns, and 3) qualitative typology of urban form. All three will use the method of validation, based on cross-tabulation, using a) statistical analysis using chi-square statistic and related Cramér's V, further interpreted based on b) compositional analysis focusing on the composition of each cluster in relation to the tested data, and c) visual assessment of spatial distribution to illustrate the behaviour of both compared data in space.

##### Analytical tools
Validation is using cross-tabulation (contingency table) as an input for all Chi-square test, Cramér's V and compositional analysis. Cross-tabulation measures the number of observations within each cluster-category pairs, where categories are reflecting the different classes of used proxy data (e.g. land use types).

The detailed method of application of selected analytical tools is proposed below.

###### Chi-square test of independence
The proposed classification as well as proposed additional data are categorical variables, including the historical origin which is presented as unevenly distributed eras rather than age. The chi-square test of independence of variables determines whether there is a significant relationship between two categorical variables based on a contingency table [@agresti2018introduction]. The null hypothesis ($H_0$) and alternative hypothesis ($H_1$) of the analysis states that 

> $H_0$: Morphometric classification of urban tissues is independent of $variable$.
> $H_1$: Morphometric classification of urban tissues is not independent of $variable$.

The statistic itself is denoted as

(@eq_chi) $\sum \chi_{i j}^{2}=\frac{(O-E)^{2}}{E}$,

where $O$ is the actual observed count, $E$ is the expected value, $chi^{2}$ is the cell Chi-square value. The expected value $E$ is calculated as

(@eq_chi_e) $E=\frac{M_{R} \times M_{C}}{n}$,

where $M_{R}$ is the row marginal (sum of the row) for the cell, $M_{C}$ is the column marginal (sum of the column) for the cell and $n$ is the total sample size [@agresti2018introduction].

The chosen alpha level of significance is $\alpha = 0.01$.

The actual implementation is based on `scipy.stats.chi2_contingency` function from open-source toolkit SciPy [@jones2001]. 

###### Cramér's V
The chi-squared statistic does indicate whether there is an association or not, but does not tell how strong it is. Cramér's V coefficient is based on chi-squared statistic, but extends it to provide a value between 0 and 1 reflecting the level of association in a similar way as Pearson's correlation does. Value 0 corresponds to no association while 1 to perfect association [@crewson2006applied].

Cramér's V coefficient is denoted as 

(@eq_cramer) $V=\sqrt{\frac{\chi^{2}}{n(q-1)}}$

where $q$ is the smaller number of either rows or columns. The strength of association described by $V$ is illustrated in table \ref{cramer}.

| $V$ | association |
|--:|:--|
| >.5 | high |
| .3 to .5 | moderate |
| .1 to .3 | low |
| 0 to .1 | little if any |

Table: Strength of association of two categorical variables based on Cramér's V coefficient. Reproduced from [@crewson2006applied]. \label{cramer}

###### Cross-tabulation compositional analysis
Each of the clusters and each of the branches are then studied independently to understand what is its composition in relation to the validation data, focusing on individual rows of a contingency table. The perfect relation would show all observations of a single class within a single cluster and none within any other. No relation would be reflected by equal count among the classes. Compositional analysis is aimed to provide more in-depth interpretative values that chi-square and Cramér's-V, but it does not state any significance level.

###### Visual assessment of spatial distribution 
The visual assessment of spatial distribution overlays the boundaries defined by morphometric classification over the validation classes to determine spatial relationship visually. Alongside the compositional analysis, the visual assessment is meant to provide interpretative information, allowing better understanding of the relation between tested data. It does not provide any numerical results as it only links compositional analysis with the geographical context.

##### Validation data
Three datasets are used within the validation framework - historical origin, land use patterns and qualitative typology of urban form linked to the predefined boundaries.

###### Historical origin
The link between the historical origin and the patterns of urban form is well established in the literature [@panerai2004] and has been recently studied using morphometric tools, from the composition and configuration of street networks [@porta2014a; @boeing2020off] to the complex morphometric assessment of sanctuary areas [@dibble2017]. The relation, which is described in literature, should be present in the data studied in this research. The existence of the significant relationship between the historical origin and results of morphometric classification would indicate the validity of the proposed classification.

The data on historical origin provided by Institute for Planning and Development Prague denotes the time frame in which was each part of the city first built-up. However, the data do not provide a single year, but a specific range, presenting what would be continuous variable of age as ordered categorical one. Moreover, the categories are not equal distributed in time, with maximums within each category being 1840, 1880, 1920, 1950, 1970, 1990, and 2012. That may lead to the situation where three adjacent building, built in years 1878, 1879 and 1881 are not seen as of the (almost) same age. The first two are in the second category, being treated as equal while the last is in the third category being treated as different. Moreover, its difference from 1841 is the same as the difference from 1949. 

These data ignore the redevelopment of parts of the city which happened later. Newly built areas, which are built in the area of previously demolished urban form are not reflected and should be interpreted accordingly.

However, even with this limitations, dataset does represent the different periods of Prague's development and there should be a significant relation.

Before doing the analysis itself, data on historic origin were spatially linked to building layer. Each building got assigned a single category of origin denoting not its own period of origin, but the first moment of the development of the area it sits in.

###### Land use patterns
Land use is determining building typology which is partially reflected in the patterns of urban form. Single-family housing is always different from industrial or commercial areas, while multi-family housing can be developed in plethora of ways, but still different from other uses. That gives us theoretical grounds for validation of proposed morphometric taxonomy using land use patterns. However, it has to be noted that such a relation will likely not be perfect, as there are mixed uses in many places. 

The data on land use in Prague capture land use to the level of individual building and plot and divides it into 123 categories. However, of those only 15 contains more than 1,000 buildings. Categories are providing detailed classification, but that does not reflect predominant tendency of land use within the area but the individual buildings. For that reason, the initial data are used to compute predominant land-use patterns within three topological steps on morphological tessellation. As predominant land-use is seen the one with the highest frequency within the *context.*

Initial land-use data are spatially linked to buildings layers to have a single value representing category per building. Then the predominant land-use is calculated based on the context. Out of resulting categories, only 5 (*Multi-family housing, Single-family housing, Villas, Industry small, Industry large*) contain more than 1% of the dataset. For that reason, these five are used and the rest is denoted as *Other*.

###### Municipal typology
Planning system of Prague is based on the concept of *localities*, small neighbourhoods [@institutplanovaniarozvojehlavnihomestaprahy2018]. Each neighbourhood has specified boundaries partially based on its morphology and partially on other aspects, from historical origin to social perception of the area. Furthermore, these neighbourhoods were qualitatively classified into one of the 10 *structural types*. This municipal typology tends to capture morphology and as such could be used as a validation method. In the ideal world, this layer would become a ground truth for the morphometric classification. However, that is not possible due to methodological flaws embedded in the typology.

The typology consists of following 10 types (loosely translated into English):

- organic structure
- perimeter block structure
- hybrid structure
- heterogenous structure
- village structure
- garden city structure
- modernist structure
- production area
- services area
- linear structure

While these types might work for planning purposes, they are conceptually incoherent mixing types based on morphology (organic, perimeter block) with those based on planning ideology (garden city, modernist), or those based on land use (production, services). Moreover, the fixation of the typology to *localities* comes with Modifiable Aerial Unit Problem [@openshaw1984], leading to the inclusion of ambiguous loosely defined hybrid and heterogenous types. 

However, the typology itself, considering above mentioned limitations, reflects what the planning authority thinks Prague is composed of and it is worth studying the relation of this qualitative typology to the proposed quantitative classification. The only adaptation which needs to be done is the exclusion of hybrid and heterogenous types from the analysis due to their MAUP-based origin and of linear structure capturing railway structures only.

The data provided as polygons represented localities are spatially joined to buildings layer and features containing excluded types are removed from the data.

#### Transferability of the method \label{transfer}

The proposed method of identification of urban tissues is validated in the context of Prague using the methods above. However, that by itself does not ensure that the method is transferable and applicable elsewhere. Different geographical contexts, bringing various types of urban tissues, and their underlying spatial logic may be challenging for a method tested in a single, no matter how heterogenous, case. The transferability of the method is a critical feature for its robustness and applicability. The method should show similar performance, in terms of identification of tissue types and a consequent taxonomy, in additional case studies.

Therefore, the method as it stands is tested on the case of Amsterdam, NL. Both Amsterdam and Prague are heterogenous cities with several historical layers, but of different planning context during their respective developments. 

##### Urban tissues of Amsterdam \label{clus_ams}
The first part of the analysis of Amsterdam is the identification of urban tissue types using the method proposed in the chapter 7. Exactly the same set of primary and contextual characters is used within Gaussian Mixture Model clustering and related BIC analysis of number of components. For the details of the method refer to the previous chapter. Similarly, method of hierarchical clustering proposed in the section 8.2.1 is applied to the resulting tissue types. 

Both results will be assessed visually on a map to understand whether the clusters alone and within their branches are interpretable and contiguous.

##### Validation of clustering in Amsterdam
The resulting clusters in Amsterdam are validated using the method proposed in section \ref{meth_validation_rel} above, using data on the historical origin of each building. In the case of the datasets obtained from @dukai2020, each building has assigned a year of its construction. Unlike in Prague, the year does not represent the data when the area/plot was first built-up, but the latest construction. Even though the data are not initially binned, only buildings constructed after year 1800 have a specific year. To ensure the compatibility of the data with those used in Prague and to avoid issues with pre-1800 periods, the origin dates are therefore binned into 11 groups following the classification of [@spaan2015]. The rest of the validation follows the method outlined in \ref{meth_validation_rel}.

#### Expandability of the classification \label{expandability}
The study of expandability of hierarchical classification is the last methodological step in the whole thesis and its role is to understand whether results of morphometric study from one case study can be related to another case study. expandability of the classification is crucial for further expansion of the database of urban tissue types. Even though clusters and hierarchical classification may work in individual cases, the question is whether we can combine the results to  a single taxonomy. It tests the compatibility of results and a potential issue of clustering being tied to a single context. The optimal situation would mirror the biological world, where a newly discovered species can be usually embedded into an existing taxonomy. However, to get to the stabilised situation where a taxonomy is not substantially changed by a discovery of a new species, we first need a critical mass of species to be included. That is certainly not the case in newly built taxonomy of urban form and it is expected that it could be relatively unstable in the beginning and stabilise by inclusion of more cases.

The method can be considered extensible, if the taxonomy of tissue types from Prague and Amsterdam combined does not substantially change the interpretative value of dendrograms.

The generation of the combined taxonomy is a straightforward process. All clusters from both cases are combined into a single pool and used as an input of Ward's hierarchical clustering. The resulting dendrogram is then compared to the initial individual dendrograms and their structures are compared. That reflects whether resulting branches capture similar tissues in both contexts. The results are then visually assessed using branches mapped on to the urban form of both cities alongside.

The final step is an interpretative analysis of the reshuffle of clusters between individual dendrograms and a combined one. In the ideal case, tissue types which are in a single branch in an individual tree should stay within a single branch in a combined one. However, as mentioned above, it is expected that some degree of reshuffle may happen when a classification structure is not yet saturated.

The following section applies the methods and presents their results.

\newpage

## Case studies - continuation of Prague, Amsterdam \label{case8}
This section presents results of the methods proposed in the previous one. It starts with the continuation of the work on Prague presented in previous chapter, developing hierarchical clustering of initially identified urban tissue types. Further it presents the indirect validation of the results using non-morphological data. The second part presents an inclusion of Amsterdam case study, as delineation of tissue types, taxonomy and validation using historical origin. Final section discuss expandability of the proposed method testing its ability to form a methodological foundation of a general atlas of urban form.

### Hierarchical clustering
The centroid values of each cluster, obtained as a mean value of each morphometric character, are used taxonomic characters within Ward's hierarchical clustering. The resulting relationship between centroids, representing the relationship between identified urban tissues, is illustrated on the dendrogram on figure \ref{fig:prg_dendrogram}. The horizontal axis represent each individual cluster, while vertical axis capture the cophenetic distance, i.e. the similarity between observations. The lower the connection between two branches is, the more similar the tissues represented by these branches tend to be. The values under each connection represent the actual cophenetic distance of a connection and number of observations which belong to the link. The different branches of the tree are coloured to ease the interpretation of the tree itself and to provide the visual link between the dendrogram and the resulting spatial distribution of branches.

![Dendrogram representing the results of Ward's hierarchical clustering or urban tissue types in Prague. The y axis shows a cophenetic distance between individual clusters, i.e. their morphometric similarity. Branches are interpretative coloured - the colours are then used on maps illustrating spatial distribution of these branches.](source/figures/ch8/200507_dendrogram.pdf "Dendrogram representing the results of clustering in Prague"){#fig:prg_dendrogram width=100%}

The dendrogram shows several major bifurcations on different levels of cophenetic distance, indicating several distinct groups of urban tissues. However, the exploration and interpretation of each branch require the projection of the results into the geographical space. To allow that, each cluster is coloured according to the branch of the dendrogram it belongs to, using different lightness of the same hue to distinguish between individual clusters. The spatial distribution of hierarchically represented cluster in the whole Prague is illustrated on the figure \ref{fig:PRG_hierarchical_clusters} and the detail of the city centre is shown on the figure \ref{fig:PRG_hierarchical_clusters_detail}.


![Spatial distribution of different branches of dendrogram. Each tissue type is coloured according to a branch it belongs to, with a minor differences in colour intensity to allow for distinguishing of individual clusters.](source/figures/ch8/PRG_hierarchical_clusters.png "Spatial distribution of different branches of dendrogram"){#fig:PRG_hierarchical_clusters width=100%}


\newpage
\thispagestyle{empty}
\newgeometry{left=2cm,bottom=2cm,top=3cm,right=2cm}
\begin{figure}[h]
	\makebox[\linewidth]{
		\includegraphics[width=\textwidth]{source/figures/ch8/PRG_hierarchical_clusters_detail.pdf}
	}
	\caption[Spatial distribution of branches in the city centre]{Spatial distribution of different branches of dendrogram zoomed to the central area of Prague. Each tissue type is coloured according to a branch it belongs to, with a minor differences in colour intensity to allow for distinguishing of individual clusters.}
	\label{fig:PRG_hierarchical_clusters_detail}
\end{figure}
\restoregeometry

Examining the dendrogram, we can highlight the different branches to understand their spatial distribution. Starting from the top of the dendrogram, from the bifurcation with the higher cophenetic distance (43.53), we can divide Prague's urban form into two major taxa. The right side of the tree represent urban form we could call *organised city* and is illustrated on figure \ref{fig:PRG_hierarchical_branch_7}. It consists of areas of mixed origin, spanning from historical core to modernist and contemporary developments. The common characteristic is predominantly residential nature of all tissues.

![Spatial distribution of clusters within a branch representing organised city. We can see a relative contiguity in the city centre but scattered discontinuous areas in the periphery.](source/figures/ch8/PRG_hierarchical_branch_7.png "Spatial distribution of clusters within a branch representing organised city."){#fig:PRG_hierarchical_branch_7 width=100%}

On the other side lies an *unorganised city*. It contains both industrial and fringe areas as well as contemporary office parks. The apparent shared logic is a relative disorder of patterns and high heterogeneity. 

![Spatial distribution of clusters within a branch representing unorganised city, located mostly on the outer ring of the city.](source/figures/ch8/PRG_hierarchical_branch_12.png "Spatial distribution of clusters within a branch representing unorganised city."){#fig:PRG_hierarchical_branch_12 width=100%}

Going deeper into the right side of the dendrogram, we reach another major bifurcation happening at distance 30.40 dividing the branch into two, representing mostly the intensity of the development. Left side, illustrated on figure \ref{fig:PRG_hierarchical_branch_6} captures urban tissues which could be characterised by single-family housing of all sorts, spanning from villages to garden city-like neighbourhoods. To illustrate the density, the mean floor area ratio of the branch is 0.38.

![Spatial distribution of clusters within a branch representing low density, organised development.](source/figures/ch8/PRG_hierarchical_branch_6.png "Spatial distribution of clusters within a branch representing low density, organised development."){#fig:PRG_hierarchical_branch_6 width=100%}

The other side of this branch represents the *dense city* of all sorts (figure \ref{fig:PRG_hierarchical_branch_3}), from medieval core, through historical perimeter block tissues to modernist housing estates. All these share the high volumetric density (mean floor area ratio of the branch is 1.76).

![Spatial distribution of clusters within a branch representing high density, organised development. It is capturing two distinct phases of development of Prague - historical period in the central areas and modernist development (mostly) in the periphery.](source/figures/ch8/PRG_hierarchical_branch_3.png "Spatial distribution of clusters within a branch representing high density, organised development"){#fig:PRG_hierarchical_branch_3 width=100%}

Further reading of the branching shows the bifurcation dividing medieval city from the rest (c.d. 25.84) and further one splitting *ordered grid-like city* from disordered one (figure \ref{fig:PRG_hierarchical_branch_1}), composed of fringe areas adjacent to *ordered city* and modernist housing estates.

![Spatial distribution of clusters within a branch representing high density, organised development with a fringe-like disorder in their patterns.](source/figures/ch8/PRG_hierarchical_branch_1.png "Spatial distribution of clusters within a branch representing high density, organised development with a fringe-like disorder in their patterns."){#fig:PRG_hierarchical_branch_1 width=100%}

This basic description of branching shows that the top-level structure of the taxonomy reflects the spatial logic of the structure of Prague to a high degree of interpretability. As the key aim of this study is not to provide deep insight into Prague's structure but to develop the method itself, this section does not go into a further details. However, the rest of the maps of individual branches is available as an Appendix 8.1. 

\newpage

### Validation
Validation results are divided into several sections. The first one focuses on relation of delineation of urban tissue types and their taxonomic branches, and additional data, which should have the ability to reflect the differences in built-up patterns. That entails historical origin, land use patterns and municipal typology of urban form, all in the context of Prague. The second section outlines the results of cluster analysis and subsequent hierarchical classification of Amsterdam. To validate Amsterdam case itself, local tissue types are assessed against data of historical origin. The third and last section focuses on results of combined taxonomy and potential of the expandability of the method and potential future development of the taxonomy of urban form.

#### Relation to additional data
Relation to additional data reflects the results of clustering and of hierarchical classification compared to the historical origin, land use patterns and qualitative municipal typology of urban form. All these are assessed based on contingency table and visual assessment of spatial distributions. Contingency table is used to calculate Chi-square statistic and Cramér's V, and to examine the composition of each cluster.

##### Origin
Data for historical origin are illustrated on figure \ref{fig:PRG_origin}. There are some significant patterns which should be reflected in the clustering, notably historical core and modernist belt. However, not all differences in origin have their counterparts in differences in clustering, as there are patterns which are consistently built across time frames (e.g., low-density single family housing).

![Spatial distribution of different periods of historical origin.](source/figures/ch8/PRG_origin.png "Spatial distribution of different periods of  historical origin."){#fig:PRG_origin width=100%}

Contingency table \ref{cont_hist} shows the distribution of buildings within clusters and time periods. It is clear that there is a relation, especially when it comes to the larger historical grouping into pre-WW2 and post-WW2 macro groups. 

|   cluster |   1840 |   1880 |   1920 |   1950 |   1970 |   1990 |   2012 |
|----------:|-------:|-------:|-------:|-------:|-------:|-------:|-------:|
|         0 |    251 |    110 |   2004 |   9310 |   2602 |    542 |    501 |
|         1 |    171 |     41 |     90 |    425 |    523 |    431 |    233 |
|         2 |    461 |    241 |    952 |   4585 |   3668 |   1816 |    224 |
|         3 |      6 |     16 |     27 |   1625 |    439 |   1217 |    749 |
|         4 |    302 |    208 |    728 |   1332 |   1359 |    842 |    299 |
|         5 |    752 |   1707 |   2522 |    926 |     11 |      2 |      1 |
|         6 |   1146 |    406 |    763 |   3193 |   2040 |   1870 |    729 |
|         7 |    244 |    150 |    281 |    834 |    639 |   1188 |    594 |
|         8 |    107 |    255 |    923 |   5125 |    636 |    287 |    509 |
|         9 |   3048 |    516 |    912 |   1766 |    581 |    421 |    573 |
|        10 |    825 |   1284 |   2630 |   2034 |    279 |     66 |     52 |
|        11 |   2097 |      9 |     17 |     26 |      0 |      0 |      1 |
|        12 |     42 |      7 |     85 |    255 |    919 |   5220 |    290 |
|        13 |   1028 |    234 |   1021 |   6227 |   2611 |   1284 |   2472 |
|        14 |    868 |    656 |   1179 |   1466 |    345 |    139 |    189 |
|        15 |   1514 |    880 |    468 |    171 |      5 |      4 |      5 |
|        16 |    417 |    214 |    337 |   1002 |    601 |    571 |    288 |
|        17 |    740 |    354 |   1298 |   6229 |   1959 |    925 |    576 |
|        18 |   1346 |    204 |    544 |   2887 |   1686 |    719 |   1178 |
|        19 |      1 |      0 |     20 |    356 |    412 |    620 |    198 |

Table: Contingency table showing the counts of features per historical origin within individual clusters. \label{cont_hist}

Reported results of a Chi-square test, based on the contingency table, assessing whether there is a significant relationship between two variables (origin and clustering), are $\chi^{2} (104, N=140315) = 106700.51, p < .001$, which indicates significant relationship.‌ Cramérs-V assessing the strength of the relationship is 0.358, indicating moderate association. Since we cannot expect complete match because the data as the theoretical relation is only partial, both results are indicating high performance of cluster analysis.

Looking at the composition of each cluster extracted from the contingency table (figure \ref{fig:PRG_cluster_origin_subplot}), we can see the relationship in a more interpretative way. Where the relationship is expected based on literature, there is clear association (historical core, modernism) with majority even falling into a single category. The striking difference between structure of pre-WW2 and post-WW2 urban patterns partially confirms previous results reported by @dibble2017 and @porta2014a.

![Illustration of composition of selected representative clusters from the perspective of historical origin.](source/figures/ch8/PRG_cluster_origin_subplot.pdf "Illustration of composition of selected representative clusters from the perspective of historical origin."){#fig:PRG_cluster_origin_subplot width=100%}

Branches of the local taxonomy show similar relation (where is feasible to expect one), especially regarding the tendency of significant changes of development patterns after the Second World War (figure \ref{fig:PRG_branch_origin_subplot}). However it is important to note that unlike other European cities, Prague was not significantly damaged during the Second World War and the difference then cannot be interpreted as post-war regeneration and redevelopment.

![Illustration of composition of selected representative branches from the perspective of historical origin.](source/figures/ch8/PRG_branch_origin_subplot.pdf "Illustration of composition of selected representative branches from the perspective of historical origin."){#fig:PRG_branch_origin_subplot width=100%}

Spatial distribution tells us what does all these statistical values mean on the ground and how good is the coincidence there. Historical core of Prague on the figure \ref{fig:PRG_cluster_11_origin_map} captures the relation if cluster 11 to the historical origin. However, due to the limitation in data grouping all development build pre-1840 into a single category, some differences need to be explained. Jewish quarter, the area which is pre 1840 but not part of the cluster on the north of the centre, has been demolished and rebuilt  in early 1800. Therefore it is not of medieval original and is correctly excluded from the cluster. 

![Illustration of the overlap between cluster 11 representing historical core and periods of historical origin. Colours represent period and the saturation the extent of the cluster.](source/figures/ch8/PRG_cluster_11_origin_map.png "Illustration of the overlap between cluster 11 representing historical core and periods of historical origin"){#fig:PRG_cluster_11_origin_map width=100%}

Cluster 5, the one we can call a compact dense city was built according to the same principle over the years, but generally tends to coincide with relevant origin categories as shown on the figure \ref{fig:PRG_cluster_5_origin_map}. Notice the split in historical origin in the central part into 1880 and 1920 categories. Similar split has been identified by sub-clustering in section 7.2.3.4.1 shown on figure 7.59. However, the reasons behind the similarity may be two - one is the historical period and the other topography, as the areas shown in green are mostly built on slopes.

![Illustration of the overlap between cluster 5 representing historical compact development and periods of historical origin. Colours represent period and the saturation the extent of the cluster.](source/figures/ch8/PRG_cluster_5_origin_map.png "Illustration of the overlap between cluster 5 representing historical compact development and periods of historical origin"){#fig:PRG_cluster_5_origin_map width=100%}

Major part of the modernist housing belt around the city (cluster 12) was built between 60s and early 90s, which is very nicely shown by the overlaps of distributions as well as on the figure \ref{fig:PRG_cluster_12_origin_map_zoom} below. 

![Illustration of the overlap between section of cluster 12 representing modernist development and periods of historical origin. Colours represent period and the saturation the extent of the cluster.](source/figures/ch8/PRG_cluster_12_origin_map_zoom.png "Illustration of the overlap between section of cluster 12 representing modernist development and periods of historical origin"){#fig:PRG_cluster_12_origin_map_zoom width=100%}

Looking at the combination of different branches, if we focus on a sample of the ordered part of dense city branch, we see almost perfect overlap with pre-1950s development. 

![Illustration of the overlap between branch representing dense compact development and periods of historical origin. Colours represent period and the saturation the extent of the branch.](source/figures/ch8/PRG_cluster_compact_origin_map_zoom.png "Illustration of the overlap between branch representing dense compact development and periods of historical origin."){#fig:PRG_cluster_compact_origin_map_zoom width=100%}

As far as it is possible to link these two aspects of form, origin and patterns, there is a significant connection validating the results of clustering and classification.

##### Land use
Patterns of predominant land use are illustrated on figure \ref{fig:PRG_land_use}.The large areas of the city are covered by single family housing and multi-family housing. The latter spans from historical development in central areas to large developments during the second half of 20th century, covering both dense compact development and modernist housing typology. There are only minor areas denoted as villas in the obtained land-use classification, mostly located in north-west of the city. Moreover, the patches of industry are often mixed with *other* land use categories, which indicates that the need to be cautious during the interpretation of results as this reflects the limitation of the data.

![Spatial distribution of predominant land use categories.](source/figures/ch8/PRG_land_use.png "Spatial distribution of predominant land use categories."){#fig:PRG_land_use width=100%}

Contingency table \ref{cont_lu} shows even more evident patterns than in the previous example.

|   cluster |   Multi-family housing |   Single-family housing |   Villas |   Industry small |   Industry large |   other |
|----------:|-----:|------:|------:|------:|------:|--------:|
|         0 |   91 | 14412 |   819 |     0 |     0 |      15 |
|         1 |   30 |   304 |     2 |    72 |   287 |    1343 |
|         2 | 6019 |  5426 |   487 |     3 |     3 |      78 |
|         3 |  201 |  3817 |     0 |     0 |     0 |     115 |
|         4 |  312 |  1065 |     1 |   733 |   546 |    2624 |
|         5 | 5905 |     0 |     0 |     0 |     0 |      25 |
|         6 | 2176 |  7038 |   255 |   214 |   146 |     500 |
|         7 | 2489 |   573 |    15 |   221 |   151 |     691 |
|         8 |  287 |  7321 |   236 |     0 |     0 |       1 |
|         9 |  191 |  7292 |   160 |    73 |    20 |     126 |
|        10 | 6609 |   389 |   196 |     1 |     1 |       7 |
|        11 | 1461 |     0 |     0 |     0 |     0 |     706 |
|        12 | 6684 |   199 |     0 |     0 |     0 |       2 |
|        13 |    6 | 14794 |   130 |     8 |     0 |      54 |
|        14 | 3775 |   281 |    59 |   104 |    64 |     701 |
|        15 | 2731 |     0 |     0 |     0 |     6 |     323 |
|        16 |  431 |  2632 |    78 |    49 |    97 |     261 |
|        17 |  505 | 11127 |   466 |    11 |     2 |      34 |
|        18 |   42 |  7384 |    61 |    41 |     6 |    1230 |
|        19 |   18 |    31 |     0 |    27 |   706 |     874 |

Table: Contingency table showing the counts of features per predominant land use within individual clusters. \label{cont_lu}

Reported Chi-square results, based on the contingency table, assessing whether there is a significant relationship between two variables (land-use and clustering), are $\chi^{2} (95, N=140315) = 176165.83, p < .001$, which indicates significant relationship. Cramérs-V value is 0.501, indicating high association, higher than in the previous case. The land use typology is known to be related to the form, even though not always in the same manner (see compact blocks vs modernism being in the came class). The results demonstrate that the clustering does reflect the similar subdivision as land-use presumes, hence indicate the validity of the classification.

Detail of the composition of individual clusters (figure \ref{fig:PRG_cluster_landuse_subplot}) shows in even more straightforward way the clear relationship between both variables. Cluster 11 (historical core) has a higher proportion of *other* uses caused by its central position where parts of historical core are used as central business district, therefore bringing different land uses to the same area.

![Illustration of composition of selected representative clusters from the perspective of predominant land use.](source/figures/ch8/PRG_cluster_landuse_subplot.pdf "Illustration of composition of selected representative clusters from the perspective of predominant land use"){#fig:PRG_cluster_landuse_subplot width=100%}

Similarly high degree of relation is present when we assess branches instead of individual clusters (figure \ref{fig:PRG_branch_landuse_subplot}). What can be seen as the highest rate of imprecision is 0.09 ratio of single family housing in industrial city branch, which shows that the actual precision is more than 90%.

![Illustration of composition of selected representative branches from the perspective of predominant land use.](source/figures/ch8/PRG_branch_landuse_subplot.pdf "Illustration of composition of selected representative branches from the perspective of predominant land use"){#fig:PRG_branch_landuse_subplot width=100%}

Illustration of spatial distribution tells the same story and it is not necessary to go into the details. The same branch of dense city (figure \ref{fig:PRG_cluster_branch0_landuse_map}) as above shows what is already explained in numbers, i.e. the high level of overlap between land-use and clustering. 

![Illustration of the overlap between branch representing dense compact development and predominant land use. Colours represent land use and the saturation the extent of the branch.](source/figures/ch8/PRG_cluster_branch0_landuse_map.png "Illustration of the overlap between branch representing dense compact development and predominant land use"){#fig:PRG_cluster_branch0_landuse_map width=100%}

The results of validation of clustering and taxonomy based on land use data show even higher levels of similarity between the variables than in the case of historical origin, clearly indicating that the morphometric tissue types can be relevant.

##### Municipal typology
Comparison of the clusters and the qualitative municipal typology is the last validation using additional proxy data. As described in the section 8.2.2.1.2.3, there are certain limitations when it comes to the municipal typology itself which results in the necessity to drop a fraction of features (20960 are dropped, therefore 119355 features are used) before the actual analysis. The data used for the analysis and their respective types are illustrated on figure \ref{fig:PRG_structure}. The types are clearly distinguished and in a sense reflect the combination of origin and land-use categories. 

![Spatial distribution of individual classes of qualitative municipal typology in Prague.](source/figures/ch8/PRG_structure_sample.png "Spatial distribution of individual classes of qualitative municipal typology in Prague"){#fig:PRG_structure width=100%}

Contingency table \ref{cont_loc} shows even more evident patterns than in the previous examples.

\small

|   cluster | organic | perimeter block |    village |    garden city |    modernism |    production |   services |
|----------:|-----:|-----:|-----:|-----:|-----:|-----:|----:|
|         0 |    0 |    0 | 5158 | 9386 |    3 |    0 |   0 |
|         1 |    0 |    0 |  252 |   87 |    0 |  960 |  92 |
|         2 |    0 |  305 |  965 | 3802 | 3600 |   13 |  49 |
|         3 |    0 |    0 |  381 | 1338 |  616 |    0 |  51 |
|         4 |    1 |   31 |  660 |  269 |   59 | 1997 | 543 |
|         5 |  375 | 5350 |    0 |    7 |    0 |    0 |   0 |
|         6 |    0 |  207 | 2551 | 3050 | 1042 |  445 | 283 |
|         7 |    0 |  158 |  178 |  174 | 1331 |  479 | 434 |
|         8 |    0 |    0 | 1941 | 4655 |  101 |    0 |   0 |
|         9 |    0 |    2 | 5659 | 1569 |    3 |    0 |   0 |
|        10 |  115 | 5248 |   70 |  853 |   46 |    2 |   3 |
|        11 | 2137 |    0 |    0 |    0 |    0 |    2 |  11 |
|        12 |    0 |    6 |   79 |  101 | 6540 |    4 |  13 |
|        13 |    0 |    0 | 8805 | 5640 |    2 |    2 |   5 |
|        14 |  174 | 2825 |   22 |  258 |  102 |  294 | 269 |
|        15 | 1283 | 1734 |    0 |    0 |    0 |   10 |   9 |
|        16 |    0 |    3 | 1198 | 1103 |  129 |  257 |  53 |
|        17 |    0 |    8 | 3538 | 6300 |  301 |   25 |  15 |
|        18 |    0 |    0 | 4327 | 3153 |   34 |   34 |  59 |
|        19 |    0 |    0 |    6 |    1 |    1 | 1461 |  73 |

Table: Contingency table showing the counts of features per municipal typology classes within individual clusters. \label{cont_loc}

\normalsize

Reported Chi-square results, based on the contingency table, assessing whether there is a significant relationship between two variables (municipal typology and clustering), are $\chi^{2} (114, N=119355) = 325595.20, p < .001$, which again indicates significant relationship.‌ Cramérs-V value is 0.674, indicating high association, the highest of all tested datasets. That is no surprise, as both layers (clusters and municipal typology) are trying to describe the same aspects of the city. Considering the MAUP-related imprecision of municipal dataset and error margin of clustering, the results offer a strong indication of the validity of the clustering output.

The relation is also clearly present in composition of each cluster (figure \ref{fig:PRG_cluster_structure_subplot}) with only difference of distinction between village and garden city typology. That is poorly specified in the original dataset and the difference is unclear as it mixes historical origin and ideology with the morphological description. So the difference between the two should be taken with care as it might just be misleading.

![Illustration of composition of selected representative clusters from the perspective of municipal typology.](source/figures/ch8/PRG_cluster_structure_subplot.pdf "Illustration of composition of selected representative clusters from the perspective of municipal typology."){#fig:PRG_cluster_structure_subplot width=100%}

Branches are combining different groups of municipal typology in a similar manner they combine clusters (figure \ref{fig:PRG_branch_structure_subplot}). We can see some deviations, but general tendency is clear and tells very similar story as taxonomy itself.

![Illustration of composition of selected representative branches from the perspective of municipal typology.](source/figures/ch8/PRG_branch_structure_subplot.pdf "Illustration of composition of selected representative branches from the perspective of municipal typology"){#fig:PRG_branch_structure_subplot width=100%}

Single illustration of spatial distribution on the branch of historical dense city shows almost precise overlap with municipal typology (figure \ref{fig:PRG_branch0_strucuture_map}). The differences, e.g. the areas marked as *perimeter blocks* in municipal typology not captured by clusters, are mostly incorrectly classified in the typology itself due to MAUP (Dejvice University Campus in north-west, Industrial belt of Holesovice in north).

![Illustration of the overlap between branch representing dense compact development and municipal typology. Colours represent classes of typology and the saturation the extent of the branch.](source/figures/ch8/PRG_branch0_strucuture_map.png "Illustration of the overlap between branch representing dense compact development and municipal typology."){#fig:PRG_branch0_strucuture_map width=100%}

Municipal typology shows the highest similarity with the morphometric urban tissue types from the all three proxy layers. This layer should be similar as it tries to capture similar perspective of the city. The fact that it does shows such high significance tells that clustering method and classification does deliver results capturing meaningful results.

The aim of the section was to validate the results of clustering using additional data. The clusters would be seen as validated if they shown significant relationship to all tested layers. The results of the validation shows significance and moderate (origin) to high association (both land-use and municipal typology) based on the employed tests. These results clearly indicate that the method of identification of urban tissue types proposed in the previous chapter and related hierarchical classification of urban tissues are both reflecting the morphological reality and could be seen as a valid method of urban morphology analysis.

\newpage

#### Transferability to other places
Even though the method is valid in the context of Prague, it is unclear whether it is transferable to other contexts. It was designed with universality in mind, so the it is assumed that it should be able to capture similar level of information in other geographic and historical contexts. To test this hypothesis, the whole methodology is applied to the case study of Amsterdam, including one layer of validation using historical origin data.

Amsterdam dataset tests not only the transferability of the method, but also its scalability. The number of buildings on the input of clustering is 252,385 compared to 140,315 buildings in Prague. 

The results of morphometric characters are not presented in the main body of the text and their distributions are available as Appendix 8.2. Since the method is following the steps defined in sections 7.1 and 8.2.1, results report the selection of optimal number of components, results of clustering and hierarchical classification.

##### Clusters
Bayesian Information Criterion shows different curve than we have seen in Prague case as it does not culminate to indicate the optimum (figure \ref{fig:AMS_bic}). That is a situation which may happen with BIC and indicates overfitting of the model, which BIC is unable to correct.

![Bayesian Information Criterion score for the variable number of components. Shaded area reflects .95 confidence interval.](source/figures/ch8/AMS_bic.pdf "Bayesian Information Criterion score for the variable number of components."){#fig:AMS_bic width=75%}

In cases like this, it is recommended to follow a different principle of identification of optimal number of components derived from the gradient of the curve (figure \ref{fig:AMS_bic_gradient}). The resulting number is then the smallest value on the stabilised gradient. Once it flattens, i.e. the change starts to become more linear, it is not expected that larger number of components will significantly improve the classification. For that reason, the number of components used for identification of clusters in Amsterdam is derived from gradient curve as 30.

![Gradient of Bayesian Information Criterion score for the variable number of components. Shaded area reflects .95 confidence interval. Red line marks the culmination of gradient at about 30 components.](source/figures/ch8/AMS_bic_gradient.pdf "Gradient of Bayesian Information Criterion score for the variable number of components"){#fig:AMS_bic_gradient width=75%}

Results of the cluster analysis are shown visually on figures \ref{fig:AMS_clusters} and \ref{fig:AMS_clusters_detail}. Spatial distribution on the next two pages (full extent of the case study and the detail of the city centre) show potentially meaningful clusters. Especially clusters in the city centre show high degree of legibility initially seems to reflect different phases of the development of Amsterdam. From this first perspective it looks promising and there is no reason to think that the method identification of clusters is not transferable yet.

![Spatial distribution of 30 clusters as identified by GMM based on morphometric data.](source/figures/ch8/AMS_clusters.png "Spatial distribution of 30 clusters as identified by GMM based on morphometric data."){#fig:AMS_clusters width=100%}

![Detail of spatial distribution of 30 clusters as identified by GMM based on morphometric data.](source/figures/ch8/AMS_clusters_detail.pdf "Detail of spatial distribution of 30 clusters as identified by GMM based on morphometric data."){#fig:AMS_clusters_detail width=100%}

Consider cluster 29 on previous figure. It, with some margin of error, captures the original historical core of Amsterdam. The next concentric belt is captured as cluster 13. The difference between dark blue (11) and grey/pink areas (4, 18) reflect the change in the planning paradigm with the rise of New Amsterdam School [@panerai2004], captured especially by grey cluster 18. On the other hand, the the results in peripheral parts of the city show a certain degree of fuzziness, which again can be a sing of potential overfitting, indicating that the actual number of clusters might need to be smaller. However, that may be resolved by taxonomy, by linking individual clusters together to branches and assessing the urban form via branches.

It is important to tests the method in additional geographical contexts than initial Prague case study, to ensure that it is transferable. Applying the method on the case of Amsterdam, NL, first results indicate that the method is transferable. However, the case also raised questions regarding the stability of the method of determination of number of components for Gaussian Mixture Model clustering as BIC curve did not culminate. That should be further explored in the further research and additional ways of identification of the optimal number might have to be introduced.

##### Hierarchical tree
The hierarchical tree (figure \ref{fig:AMS_dengrogram_n30}) derived from morphometric data of Amsterdam  shows similar characteristics as we have seen in Prague, with the significant bifurcation into two branches distinguishing predominantly industrial and housing tissues and then consequent bifurcations lower in the tree distinguishing different rules of organisation.

![Dendrogram representing the results of Ward’s hierarchical clustering or urban tissue types in Amsterdam. The y axis shows a cophenetic distance between individual clusters, i.e. their morphometric similarity. Branches are interpretative coloured - the colours are then used on maps illustrating spatial distribution of these branches.](source/figures/ch8/200507_dengrogram_n30.pdf "Dendrogram representing the results of Ward’s hierarchical clustering or urban tissue types in Amsterdam"){#fig:AMS_dengrogram_n30 width=100%}

Spatial distribution shows what the branches actually mean. See the whole case study and its detail coloured according to the dendrogram on figures \ref{fig:AMS_clusters_hierarchical} and \ref{fig:AMS_clusters_hierarchical_detail}. Again, each cluster has a different shade of the same colour when it belongs to the same branch.

![Spatial distribution of different branches of dendrogram in Amsterdam. Each tissue type is coloured according to a branch it belongs to, with a minor differences in colour intensity to allow for distinguishing of individual clusters.](source/figures/ch8/AMS_clusters_hierarchical.png "Spatial distribution of different branches of dendrogram in Amsterdam"){#fig:AMS_clusters_hierarchical width=100%}

![Detail of spatial distribution of different branches of dendrogram in Amsterdam. Each tissue type is coloured according to a branch it belongs to, with a minor differences in colour intensity to allow for distinguishing of individual clusters.](source/figures/ch8/AMS_clusters_hierarchical_detail.png "Detail of spatial distribution of different branches of dendrogram in Amsterdam"){#fig:AMS_clusters_hierarchical_detail width=100%}

The first bifurcation is analogous to one identified in Prague and divides the city to the organised (figure \ref{fig:AMS_hierarchical_branch_6}) and unorganised (figure \ref{fig:AMS_hierarchical_branch_10}) parts. Organised is composed of predominantly residential use. It entails the whole historical core, and major parts of residential housing. However, there are major gaps in between contiguous areas caused by the high presence of all sorts of industry and other uses. After all, Amsterdam is historically a port city. 

![Spatial distribution of clusters within a branch representing organised city in Amsterdam. Although there are significant gaps, the overall distribution of tissues seems to be more contiguous than in Prague.](source/figures/ch8/AMS_hierarchical_branch_6.png "Spatial distribution of clusters within a branch representing organised city in Amsterdam"){#fig:AMS_hierarchical_branch_6 width=100%}

![Spatial distribution of clusters within a branch representing unorganised city in Amsterdam. Similarly to the previous figure, clusters belonging to this branch tend to form either contiguous areas or follow main roads in between.](source/figures/ch8/AMS_hierarchical_branch_10.png "Spatial distribution of clusters within a branch representing unorganised city in Amsterdam"){#fig:AMS_hierarchical_branch_10 width=100%}

The branch comprising the organised city splits into high density and low density in a similar manner as Prague's case does. High density is mostly historical core \ref{fig:AMS_hierarchical_branch_0}, in this case the one of Amsterdam and also Weesp on the east side if the city. Moreover, parts of the modern development on former port sites tends to show similar characteristics. Further bifurcation within lower density development is readable and follows sorts of the compactness and homogeneity of patterns, so we have organised residential areas, their more heterogenous counterparts and fringe areas around compact high density areas (figure \ref{fig:AMS_hierarchical_branch_4}). The tree also resolves the initial fuzziness of individual clusters (notice that light blue, red and pink branches are very similar to each other).

![Spatial distribution of clusters within a branch representing high density, mostly historical development of in Amsterdam.](source/figures/ch8/AMS_hierarchical_branch_0.png "Spatial distribution of clusters within a branch representing high density, mostly historical development of in Amsterdam."){#fig:AMS_hierarchical_branch_0 width=100%}

![Spatial distribution of clusters within a branch representing low density development in Amsterdam.](source/figures/ch8/AMS_hierarchical_branch_5.png "Spatial distribution of clusters within a branch representing low density development in Amsterdam."){#fig:AMS_hierarchical_branch_4 width=100%}

Hierarchical taxonomy shows very similar character as was observed in Prague and visually works in a coherent way. It seems safe to conclude that the proposed method behaves in both cities in a similar way, which indicates its universality and transferability.

##### Validation using historical origin
To further assess the validity of clustering in Amsterdam, one layer of validation based on additional data, historical origin, is used as a proxy. The initial input data are illustrated on figure \ref{fig:AMS_origin}. 

It should be noted that it captures the origin of individual buildings, not the time when the plot was first built as in Prague. As with the data on origin for Prague, we can expect certain degree of association, but not full as not all patterns are time dependent. The test will be done using the same method based on contingency table, chi-squared and Cramér's V.

![Spatial distribution of different periods of historical origin in Amsterdam.](source/figures/ch8/AMS_origin.png "Spatial distribution of different periods of historical origin in Amsterdam."){#fig:AMS_origin width=100%}

|   cluster |   1800 |   1850 |   1900 |   1930 |   1945 |   1960 |   1975 |   1985 | 1995 |   2005 |   2020 |
|----------:|------------:|---------------:|---------------:|---------------:|---------------:|---------------:|---------------:|---------------:|---------------:|---------------:|---------------:|
|         0 |         827 |              4 |           3012 |           2560 |            484 |            154 |             86 |            311 |            471 |           1048 |            854 |
|         1 |           2 |              1 |             23 |            752 |            748 |           5678 |           5841 |           2048 |           5582 |           2136 |           3210 |
|         2 |         761 |             10 |            625 |           2307 |            839 |            431 |            207 |            495 |            593 |            590 |            181 |
|         3 |          14 |             21 |            116 |            584 |            251 |            381 |            546 |            385 |            337 |            460 |            328 |
|         4 |          38 |              0 |            526 |           5743 |           2771 |             75 |              6 |              6 |             20 |             23 |              5 |
|         5 |          80 |             52 |            698 |           4214 |           2126 |           2132 |           2034 |           1208 |            932 |            920 |            763 |
|         6 |           6 |              4 |             83 |            821 |            490 |            679 |           1521 |            693 |           1993 |           1365 |           1287 |
|         7 |           0 |              0 |              1 |              0 |              7 |            604 |           5455 |           3455 |           3282 |            503 |            367 |
|         8 |          29 |              6 |             50 |             38 |             36 |            149 |            449 |            360 |            442 |            516 |            399 |
|         9 |           4 |              6 |            136 |           3151 |           4444 |           5095 |           1579 |            578 |           1154 |            791 |           1279 |
|        10 |           1 |              0 |             13 |            498 |            340 |           5379 |           3086 |            839 |           2949 |           1940 |           1796 |
|        11 |         980 |              0 |           3526 |           4324 |            272 |             38 |             50 |            200 |            452 |            204 |             58 |
|        12 |           2 |              0 |             35 |            272 |            114 |            252 |            630 |            178 |            718 |           1582 |           1267 |
|        13 |        2815 |             41 |            287 |            462 |            170 |             42 |             57 |             68 |            124 |            121 |             23 |
|        14 |          35 |             14 |            165 |           1525 |            911 |           2398 |           4149 |           1916 |           2511 |           1529 |           1305 |
|        15 |          12 |              9 |            154 |            498 |            209 |            302 |            408 |            369 |            390 |            375 |            354 |
|        16 |           0 |              0 |             23 |             19 |              0 |            277 |            321 |            171 |            136 |             65 |             93 |
|        17 |          50 |             19 |            225 |            553 |            238 |            691 |           1578 |            998 |           1197 |           1228 |            962 |
|        18 |          33 |              0 |            312 |           8359 |           3280 |            573 |             45 |            357 |            344 |            102 |             34 |
|        19 |          14 |              0 |             16 |            270 |             37 |            208 |            499 |            504 |            560 |              9 |            145 |
|        20 |           3 |              0 |              3 |             30 |             19 |             77 |           2031 |           4203 |           1475 |            325 |            167 |
|        21 |          18 |             11 |             96 |            323 |             94 |            207 |            340 |            228 |            219 |            243 |            165 |
|        22 |           1 |              0 |             83 |            152 |            317 |           1901 |           1108 |           1160 |           1023 |            709 |           1143 |
|        23 |           0 |              0 |             11 |             10 |              2 |             12 |             51 |             84 |            158 |            158 |            117 |
|        24 |           0 |              0 |              0 |           2696 |            942 |           2457 |            932 |            107 |           3806 |            768 |            624 |
|        25 |          46 |             14 |            142 |           1459 |            796 |            632 |           1112 |            597 |            675 |            692 |            609 |
|        26 |           1 |              1 |             38 |            229 |            164 |            344 |            569 |            315 |            329 |            371 |            228 |
|        27 |          48 |             16 |            128 |            687 |            319 |            336 |            421 |            308 |            325 |            638 |            309 |
|        28 |           0 |              0 |             31 |            255 |            155 |            685 |            859 |           2430 |           2032 |           1453 |            402 |
|        29 |        2971 |             62 |            367 |            703 |            233 |             48 |             65 |            145 |            279 |             92 |             50 |

Table: Contingency table showing the counts of features per historical origin within individual clusters in Amsterdam \label{cont_ams}

The contingency table \ref{cont_ams} is shown above. Reported Chi-square results, based on the contingency table, assessing whether there is a significant relationship between two variables (origin and clustering), are $\chi^{2} (290, N=252385) = 312903.31, p < .001$, which indicates significant relationship.‌ Cramérs-V value is 0.353, indicating moderate association. The value is almost the same as reported in Prague, indicating that the relationship of clustering to historical origin is consistent across both cases and it is not case-dependent. The further exploration of contingency table is excluded here as it is only illustrative and the numerical values are significant.

Results of morphometric cluster analysis, consequent taxonomy and validation using historical origin data in the case of Amsterdam, NL, indicate the transferability of the method to other geographical and planning contexts, at least within the European region. The results are consistent with what was reported above for Prague, leading to the conclusion that the method can be seen as valid even from the perspective of transferability.

\newpage

#### Expandability and compatibility
The last question which remains to be answered is whether these two cases are compatible with each other. On other words, whether we can build combined taxonomy and further extend it by adding other cases. 

The extension is tested in a relatively simple way. Identified tissue types from both cased are mixed to form a single pool of clusters, all represented as cluster centroids and used as an input of hierarchical clustering. That means that while the first step, the cluster analysis is done locally for each city independently on the other, the second, taxonomy is combining them. Hence, the resulting hierarchical taxonomic tree should identify the similarity of urban tissue types across both cities.

The dendrogram from combined pool of clusters (figure \ref{fig:AMSPRG_dengrogram_mixed}) shows similar structure as both individual have, with a major bifurcation dividing unorganised/industrial areas from the organised city. Further bifurcation of organised city splits into dense, compact city and the rest and then further into sub-types of development.

![Dendrogram representing the results of Ward’s hierarchical clustering or urban tissue types from a combined pool of Prague and Amsterdam. The y axis shows a cophenetic distance between individual clusters, i.e. their morphometric similarity. Branches are interpretative coloured - the colours are then used on maps illustrating spatial distribution of these branches.](source/figures/ch8/200505_dengrogram_mixed.pdf "Dendrogram representing the results of Ward’s hierarchical clustering or urban tissue types from a combined pool of Prague and Amsterdam"){#fig:AMSPRG_dengrogram_mixed width=100%}

Spatial distribution of resulting branching (figures \ref{fig:AMSPRG_clusters_mixed_H_PRG_detai} and \ref{fig:AMSPRG_clusters_mixed_H_AMS_detail}) tells the same story as individual classifications in both Prague and Amsterdam. What is important here is the ability to compare similar tissue types across cities and as shown in the dendrogram, there are some which are really close to each other.

![Detail of spatial distribution of different branches of a the combined dendrogram in Prague. Each tissue type is coloured according to a branch it belongs to, with a minor differences in colour intensity to allow for distinguishing of individual clusters.](source/figures/ch8/AMSPRG_clusters_mixed_H_PRG_detail.png "Detail of spatial distribution of different branches of a the combined dendrogram in Prague"){#fig:AMSPRG_clusters_mixed_H_PRG_detail width=100%}

![Detail of spatial distribution of different branches of a the combined dendrogram in Amsterdam. Each tissue type is coloured according to a branch it belongs to, with a minor differences in colour intensity to allow for distinguishing of individual clusters.](source/figures/ch8/AMSPRG_clusters_mixed_H_AMS_detail.png "Detail of spatial distribution of different branches of a the combined dendrogram in Amsterdam"){#fig:AMSPRG_clusters_mixed_H_AMS_detail width=100%}

We can further look into the spatial distribution of the same major branches in both cities (figures \ref{fig:AMSPRG_clusters_mixed_H_PRG_branch_10}, \ref{fig:AMSPRG_clusters_mixed_H_AMS_branch_10}, \ref{fig:AMSPRG_clusters_mixed_H_PRG_branch_11}, \ref{fig:AMSPRG_clusters_mixed_H_AMS_branch_11}). It is a great tool to study their structure and compare them. One clear outcome of this first comparison is the observation that industrial areas are much larger in Amsterdam due to its port nature compare to traditionally mercantile Prague, but such an analysis could be done in a very detailed manner. However, that is not within the scope of this study.

![Spatial distribution of clusters within a branch representing organised city in Prague, derived from a combined dendrogram.](source/figures/ch8/AMSPRG_clusters_mixed_H_PRG_branch_10 "Spatial distribution of clusters within a branch representing organised city in Prague, derived from a combined dendrogram."){#fig:AMSPRG_clusters_mixed_H_PRG_branch_10 width=100%}

![Spatial distribution of clusters within a branch representing organised city in Amsterdam, derived from a combined dendrogram.](source/figures/ch8/AMSPRG_clusters_mixed_H_AMS_branch_10 "Spatial distribution of clusters within a branch representing organised city in Amsterdam, derived from a combined dendrogram."){#fig:AMSPRG_clusters_mixed_H_AMS_branch_10 width=100%}

![Spatial distribution of clusters within a branch representing unorganised city in Prague, derived from a combined dendrogram.](source/figures/ch8/AMSPRG_clusters_mixed_H_PRG_branch_11 "Spatial distribution of clusters within a branch representing unorganised city in Prague, derived from a combined dendrogram."){#fig:AMSPRG_clusters_mixed_H_PRG_branch_11 width=100%}

![Spatial distribution of clusters within a branch representing unorganised city in Amsterdam, derived from a combined dendrogram.](source/figures/ch8/AMSPRG_clusters_mixed_H_AMS_branch_11 "Spatial distribution of clusters within a branch representing unorganised city in Amsterdam, derived from a combined dendrogram."){#fig:AMSPRG_clusters_mixed_H_AMS_branch_11 width=100%}

However, there are some differences in branching. The resulting tree reshuffled few of the clusters and slightly reorganised branches. This will likely happen when we add more cases until the taxonomy will get more saturated. As shown on figure \ref{fig:flows}, the reshuffle is, however, relatively minimal and clusters which were associated to the same branch in individual dendrograms tend to stay together in the combined one as well. Furthermore, the overall structure of the dendrogram and the relationship between different branches remains relatively consistent.

![Diagram illustrating the flow of clusters between branches of individual dendrograms and the combined one.](source/figures/ch8/200505_dengrogram_flows-02.pdf "Diagram illustrating the flow of clusters between branches of individual dendrograms and the combined one."){#fig:flows width=100%}

There are a few differences worth noting. The Prague clusters 6 and 16 has moved from the unorganised city branch to organised. Both clusters are capturing mostly single family housing built on the steeper hills causing the disruption of a standard pattern. The similar shift happened to Amsterdam clusters 27 and 35, composed of low-density development around roads. All are now classified among other single family tissue types, which seems to be a more appropriate place. Prague's cluster 10 (fringe-like edges of compact development) is now closer to the homogenous compact development making together more reasonable branching. There is a reshuffle in low-density branches of Amsterdam, but as these are generally similar it is not a big issue. The inclusion of Prague's low-density cluster most likely caused new regrouping based on additional information. Generally, it looks that those few reshuffles are actually making the taxonomy more robust and eliminate the potential issues due to small number of OTUs in a single case study.

As shown by the results above, there does not seem to be any issue with combining morphometric tissue types identified independently of each other into a singular taxonomy. The differences are expected as the current number of tissue types, i.e. OTUs for derivation of taxonomy is still low and the taxonomy itself is not yet saturated. However, it is assumed that further expansion of the pool of case studies could eventually lead to the stabilisation.

\newpage

## Summary of taxonomy and validation \label{conclusion8}
This chapter, the last of the core chapters, focused on the development of a method able to derive a taxonomy of urban form and validation of the whole morphometric assessment proposed in this research. 

The development of taxonomy takes form of Ward's hierarchical clustering of initial morphometric tissue types defined in Chapter 7, represented by their centroids (i.e. mean values of contextual morphometric characters). The results show a very meaningful identification of relationships between individual tissue types and allows rich analysis of the structural composition of the city of Prague. 

The validation of the morphometric assessment was done in three steps. The first one compares the spatial distribution of clusters and taxonomic branches to additional proxy data which are known to partially reflect the patterns of urban development. This research used data on historical origin, predominant land use patterns and finally qualitative municipal typology of urban form. Data on all three showed significant relationship between them and identified clusters, indicating that from the perspective of ability of classification to reflect expected patterns of these proxy layers, morphometric urban tissue types are a valid concept.

The second validation step was the application of the whole method on the case study of Amsterdam, NL, which on one hand shares morphological richness of Prague and on the other was built in a different planning context. The resulting urban tissue types and their taxonomy tend to behave in a similar manner as was observed in Prague, indicating that the method could be transferable from one context to the other.

The final part of the chapter is assessing the proposed method from the perspective of its expandability and compatibility of results from Prague with those from Amsterdam. In other words, it tested whether it can become a methodological foundation of taxonomy of urban form. The combined taxonomy of tissue types shows the high degree of consistency if compared to individual ones. Furthermore, the certain reshuffle which happened mostly reflected the previous misalignment of tissue types, rendering the final taxonomy more robust than those done independently.

The chapter 9 will discuss what are implication of these results and where the research should head next.
