\setcounter{chapter}{1}

\tableofcontents

# Existing approaches to classification of urban form

_link back_
*The aim and key interest of this research as outlined in the introduction is classification of urban form.*

_aim of the chapter_
*Aim of this chapter is to understand various models of classification from theoretical perspective and review how they have been applied to urban form to date.* 
*focus on quantitative morphology (link to introduction), but some detours are necessary to give a full picture*

_structure of the chapter_
*- theory of classification*
*- optimal classification model*
*- spectrum of classification models used in literature*
	*- recurring concepts*
	*- from city to plot scale variety*
	*- close work*
*- the gap*
*- ==1) what is the classification?, 2) how should it look like?, 3) how was it done so far?, 4) what is missing?==

## Making sense of the world
- *Why is classification important, what can it bring to the table, why should we bother doing it.*

### Classification as a method
Before we can talk about classification, it is necessary to declutter and define the term itself, as it is used in literature in multiple meanings. In his overview of the whole concept and its meanings, @bailey1994 defines classification as "*the ordering of entities into groups or classes on the basis of their similarity*" (p.1). At the same time, he notes that "*classification is both process and an end result*" (p.2). This can cause terminological confusion as in some situation ti might be unclear whether we refer to the resulting systematics or the procedure which generates one. This polysemic nature of the term itself is even VETSI if we explore the definition offered by Oxford English Dictionary (OED), as it comes with three relevant options:

- "*A systematic distribution, allocation, or arrangement of things in a number of distinct classes, according to shared characteristics or perceived or deduced affinities.*"
- "*The action of classifying or arranging in classes, according to shared characteristics or perceived affinities*"
- "*‌A category to which something is assigned; a class.*" REF

While first two coincide with the definition offered by @bailey1994, the last adds one more option - a class. To minimise the confusion, this research will refer to classification as process and end result, following Bailey's approach, always trying to specify which meaning is used. The last definition offered by OED will not be used within this research.

Classification systems vary and can be systematised based on the different aspects of the resulting structure and on the method used in the process. The first distinction can be done based on the number of dimensions to *unidimensional* and *multidimensional*. Dimensions can be both numerical and categorical variables, where unidimensional numerical classification is also known as *binning* REF. ==EXAMPLE== The scope of this work is in multidimensional classification as single dimension does not have the explanatory power to describe the complexity of urban form.

Looking at the structure of the classification results, we can talk about *flat* and *hierarchical* models. Flat models generally define all classes as equal and do not specify the relationship between them, either because it could not be specified or because the model does not focus on such aspect. And example is general land use classification, which is flat in the nature (residential use, commercial, industrial etc.) and relationship between different classes is conceptually complicated to define. Hierarchical models specify, either numerically or conceptually, relationship between different classes and hence offer certain level of flexibility of classification as their structure can be interpreted on multiple levels of resolution. That allows division of elements into two macro classes or multiple micro classes within the same system. Typical example is biological taxonomy of species, where different levels of resolution are represented by domains, kingdoms, families or species. Typical hierarchical classification is, compared to flat models, computationally or conceptually more challenging, but the flexibility which it brings (where applicable) is usually valuable. 

Methodologically, we can distinguish two key approaches - one is conceptual and other is numerical, or in other words, one is *typology* and the other is *taxonomy*. Typology is a conceptual classification, where resulting classes represent concepts, not empirical cases [@bailey1994; @marradi1990]. Which means that typologies can be seen as *qualitative classifications*, because there is generally no statistics involved. The land use case mentioned above is a good example of a typology. On the other side is taxonomy, which is quantitative classification, with classes being empirical entities [@bailey1994; @sneath1973]. As with the term classification, taxonomy is also used to describe both process and end result. Specific position has *numerical taxonomy* [sokal and sneath 1963], which is quantitative, algorithmic classification (more on numerical taxonomy is in section XXX==link ch4==). Conceptually, literature knows three terms for quantitative classification based on statistical analysis. One is mentioned numerical taxonomy. The other is term *cluster analysis*, describing the process of classification. As @bailey1994 points out, the methods of numerical taxonomy can generally be classified as clustering algorithms, making the numerical taxonomy in a sense of a process and cluster analysis "*virtually synonymous*" (p.7). To complicate things further, machine learning area uses term *unsupervised classification* for cluster analysis, but these two (together with *clustering*) are equal. Within this research, term taxonomy will be used to describe the end result only, while cluster analysis, clustering and unsupervised classification may be used interchangeably. \footnote{Since we are talking about unsupervised classification, it is worth noting that supervised classification is a bit different concept and it technically is rather labelling or classing. It is a tool to sort features into pre-defined categories, unlike all above, which encompass the determination of categories as well. Again, this is terminological issue, but because it is not used in this work, we can leave it out.}

The reasons why is classification useful has @bailey1994 summarised in ten fundamental advantages, which are all transferable to urban morphology and classification of spatial structure of cities. A classification is a tool for *description* (1), giving an overview of all classes within data, based on the same criteria. The classified data has *reduced complexity* (2) to a manageable extent. We cannot deal with all individual animals on Earth, but we can work with their taxonomy, significantly reducing the amount of information to deal with. Classification can be used to identify *similarities* (3) and *differences* (4) among cases. Identification of similarities allows us to treat all individuals of a single class of similar classes equally (e.g. *be aware of snakes* or *go shopping to commercial district*). On the other hand, we can distinguish subtle differences between rather similar entities (e.g. difference between venomous and non-venomous snakes is quite helpful). A classification, if done properly, is defined by *an exhaustive list of dimensions* (5) on which different classes are based. In such a case, the resulting classification can be very comprehensive, while capturing the relationships between classes and dimensions, which is useful for further analysis and profiling of classes. That allows quick, straightforward *comparison* (6) of classes from different parts of classification structure. Complete list of classes can serve as the *inventory* (7) for management purposes and allows the study of *relationships* (8) among dimensions, relative to the structure of the classification. Moreover, classes can be used as *criteria for measurement* (9), where one class is the criterion and assessed according to similarity with the criterion (e.g. *how close is snake A to a python?* or *how similar is neighbourhood A to Manhattan?*). Finally, classification may be very *versatile* (10), as it can represent both individual units under scrutiny and their location within property space, but also describe the whole sample of units. (pp.12 - 14).

==might need some ending?==

### Optimal classification model
Classification model can follow multitude of pathways and can be defined based of various aspects for a plethora of purposes. However, the aims and scope of each research should drive the classification. Since this research aims to develop a data-driven method, its methodological nature should be a taxonomy. The *optimal classification model (OCM)* for the purpose of this research can be then defined based on following set of rules derived from definitions presented in the previous sections. Each of the existing models present in literature and outlined in the next section is then related to OCM. Furthermore, the specification of the model used within this study (see section ==XXX==) should directly reflect the rules in its fundamental design.

The optima classification model of urban form should be:

1. Exhaustive
2. Mutually exclusive
3. Empirical
4. Hierarchical
5. Comprehensive
6. Detailed
7. Scalable

Exhaustive model covers all entities within the set, meaning that there should not be unlabelled cases in the resulting taxonomy. Mutual exclusivity ensures that no entity is at the same time member of more than one class to minimise ambiguities. Empirical nature ensures the data-driven nature of the classification limiting the potential bias in the derivation of *concepts* and dependency on the expert knowledge to assess each entity. Structurally, the model should be hierarchical to allow flexibility of its reading, unavailable for flat options. Comprehensiveness entails the number of dimensions, or descriptors, used to cluster entities. The selection of dimensions can be easily biased and negatively influence the resulting taxonomy. By implementing the large number of dimensions (trying to be as inclusive as possible), such a possibility can be effectively minimised [@sneath1973]. The classification of urban form should also be detailed in terms of spatial granularity, meaning that labels should be assigned to individual plots or buildings rather than districts or cities. Finally, the model should be scalable. This is both technical and conceptual requirement, which should ensure that the same model can be used to classify small town and large metropolitan areas.

## Spectrum of classification models
- *There are two main branches of science focusing on urban form classification, which are surprisingly separated from each other - remote sensing and urban morphology. The diffusion between approaches is minimal, even thought conceptually focus on the same questions. ==explain scope ignoring purely qualitative methods==*

### Recurring concepts
- *Few concepts are quite established and worth exploring their characteristics.*

- ==link those to the definitions above==

#### Urban Structural Types
*The concept of Urban Structural Types firstly used in 1960s REF, then reintroduced in 1992 REF is covering various methods. Despite its popularity in remote sensing, it is quite inconsistent. ==define==*
*various methods if their identification, from qualitative heuristics based on visual assessment () to ML models ==give examples==*
- popular in remote sensing, but inconsistent
- "diverse understanding of subject and implementations" Lehner p.2
- "defined by specific spatial characteristics, e.g., the morphology and the spatial relationships between urban artefacts such as buildings, streets, trees, lawns"  Lehner p.2
- Mostly typology, few examples of taxonomy
- "there are only a few that use the same USTs for more than one city in terms of definition, description and derivation" Lehner p.7
- often flat
- different scales
- Lehner proposes generic UST framework, which is hierarchical typology. But since it is generic and typological it does not fulfil conditions above either.

*In relation to the OCM requirements it is complicated to assess the concept as a whole due to its internal inconsistency, but USTs are mostly typologies.*

#### Land Cover
*Related concept focuses on land cover only, again based on remote sensing. It usually aims to classify all areas, not only urban.*
- urban form as a part of wider classification of land
- Corine = continuous x discontinuous, industrial/commercial, ports, airports
	- level 1, level 2, level 3 - hierarchical
- Copernicus urban atlas
	- added density on top of continuity
- Pauleit Duhme - 10 UF types
*issues*
- *comes as Typology first, then data are being labelled*

#### Local Climate Zones
*Local climate zones mix both structure and land cover into typology*
- typology of 10 built types and 7 land cover types
- quite generic, so it covers everything
- still top-level
- used in RS field on a large scale
- flat classification
- numerically defined classes, but still capturing conceptual division
*lcz*
*issues*
*The example of typology, and inherits its limitations.*

==mention issues along the way==
==link those to the definitions above==
*apart from these, there is a wide spectrum of models*

### From city to plot level
*Apart from recurring concepts, wide range of classification methods was proposed in urban morphology, ranging from typologies to taxonomies and from city to building scales.*

*go from city scale to building scale ==always say the relation typology/taxonomy and OCM requirements==*
*most of these methods are typologies*


### Multiple Fabric Assessment and Chalmers School
*there are two recent notable works which are closest to the OCM requirements, and that is Multiple Fabric Assessment proposed by Araldi and Fusco and typology of plot systems, street network systems and --- by Berghauser Pont ...*

*Araldi focus on street segment... describe, issues (limited number of characters, assumption of homogeneity, no hierarchy, applied to local cases with no cross-comparison framework*

*Chalmers developed typology based on empirical cases. Three different typologies, not really combined. Limited amount of characters. Data requirements.*

## The gap in the systematic classification
*As shown, none of existing models is all empirical, hierarchical, comprehensive, detailed and scalable. Some are close, but none fits all criteria.*
- lack of systematic classification based on the small-scale unit
- gap in taxonomy (empirical cluster analysis)
- gap in detailed classification (i.e. number of classes)


## Conclusion
*Classification is polysemic term. This work focuses on a specific way of doing it, taxonomy, with specific requirements defining the optimal model.*

*Existing models vary, from remote sensing models to typo-morphological, but none fulfils the all criteria. Some are close, but the gap is clear and wide.*