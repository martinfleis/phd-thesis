\setcounter{chapter}{5}

\tableofcontents


# Morphometric elements of urban form

_link back_
- we know what ppl did
- we have general method outlined
- let's move towards operationalising it

_aim of the chapter_
- what are the elements
- how do we combine them together
- introduce tessellation

_structure of the chapter_


## Analytical representation of urban form

_introduction to elements and models_

_more paras_

- this chapter will talk **only** about the analytical measurable representation of UF
	- talk about the elements
	- talk about the models

### Elements of urban form in the context of urban morphometrics

- we have fundamental elements
- we have their aggregations
	- the way we aggregate them matters

*there are three fundamental and a range of other elements. Fundamental are abc, other are defghi.*

- there are different levels of specificity (kropf)
	- relate to Dibble's CUEs
		- Dibble used detailed specific CUEs

	- open spaces
		- polygons - can be on the level of plot
	
	- intra-building elements
		- rooms, structures, materials

	- Issue of availability
	*the first issue *
	==**problem** data are not available, we need to use as small number of resources as possible to keep morphometric method applicable==


#### Fundamental morphometric elements
Urban morphology knows three fundamental elements of urban form. Both [@moudonUrbanMorphologyEmerging1997] and later [@kropf2017] agree on buildings, streets and plots as features representing three fundamental aspects of human behaviour: *sleep*, happening in shelter, i.e. building, *movement*, first reflected in tracks and today in streets and roads and *local activity*, initially happening in a core territory, which can be today seen as a plot [@kropf2017]. 

Fundamental *morphometric* elements are based on fundamental morphological elements and their goal is to reflect the same phenomena. However, the difference between morphological and morphometric elements is that the latter are operational, measurable and represented as (usually vector) GIS data. Hence we can talk about three layers of data: building footprints, street networks and plots as smallest spatial units.

##### The quality of data and its pre-processing
It is fundamental to ensure that the actual data are good enough to represent morphometric elements. That could be an issue for all  types of elements, so there are cases when the data needs to be prepared for morphometric analysis. The pre-processing can be in some cases automatised, in other, unfortunately, manual or at least semi-manual to have the data in the correct shape in the end.

While each dataset coming from a different source is specific; hence the cleaning procedure needs to be tailored to each source, there are some common issues which are not unique to specific datasets. The following section presents all fundamental morphometric elements and outlines these common issues and ways of resolving them or at least minimising the error under a significant level. We cannot expect data to be perfect all the time (they are never perfect). This limitation has to be taken into account during the design of any morphometric analysis, which needs certain level of robustness to accommodate for potentially erroneous data.

##### Building footprint
Building footprints are polygon-based representation of building shapes, orthogonally projected to the ground. Depending on the required detail, building can be represented as 2D footprint, 2.5D footprint with height attribute or 3D model, where the patter is not seen as fundamental as it brings additional detail for architectural scale more than urban pattern. Well-known application of building footprints is for example figure ground plan.

==illustration==

Having data layer representing building footprints correctly and consistently is the first condition for successful morphometric analysis. There are several aspects which need to be fulfilled - topological correctness, consistency in detail, representation of individual buildings and building height attribute presence. Overall, it is expected to have a building data representing Level of Detail 1 (LoD1) [@biljecki2016].

==lod illustration==

Topological correctness ensures that geometry represents the actual relationship between buildings on the ground. There are characters measuring continuity of a perceived wall in a joined buildings or shared walls ratio which require building polygons to be correctly snapped together when two buildings touch. In that case, it is expected that neighbouring polygons will share vertices and boundary segments. There should not be a gap between polygons when there is none in reality and vice versa. Also, polygons must not overlap at any case as that could cause significant disruption of analysis.

The building detail should be consistent across the dataset and represent an optimal approximation of building shape based on LOD specification as proposed by @biljecki2016. The approximation should represent LOD1.1 (no details, but the shape is kept) or LOD 1.2 (minor details), building shapes should not be overly detailed nor overly simplified. In the case of inconsistency, simplification of more detailed shapes needs to be done before morphometric assessment.

Each polygon should represent a single building. There are datasets (often of remote sensing origin) capturing all structures which are joined by any means as a single polygon. Such data do not represent the morphological truth on the ground. Their pre-processing is complicated as it requires splitting of existing geometries according to an additional dataset. The second extreme is the opposite situation, when a single building is represented by multiple polygons. These usually represent different height levels, through routes or similar features. If these polygons, representing parts of buildings, have a common ID which allows joining them together to get a single polygon representing a single building, the pre-processing of such a data is only a simple dissolution. However, there are many cases when this ID is missing, and correct pre-processing require either clever algorithms to understand which polygon belongs to which or laborious manual work.

A number of morphometric characters uses building height attribute, which, in that case, has to be present in the original input dataset. The resolution should be able to capture the distinction between floor levels; further detailing is usually not significant.

##### Street network
Street network represents street, but that itself can be, form the data perspective, defined as multiple things. We can understand it as a movement, as an area or as a network. Furthermore, an important aspect of street (network) is also junction - node. Therefore, within this study, street is represented as street network consisting of edges representing centrelines and nodes representing junctions. Both can be abstracted to a simple polyline geometry.

==illustration==

Similar pre-processing situation as with building layer is with a street network. Incorrectly drawn street network may cause significant errors in morphometric results and consequently in clustering. There are three most important cases which need to be checked before the analysis - topological correctness, morphological correctness and consistency in classification.

Topological correctness ensures that each street segments is represented by a single `LineString` geometry, that neighbouring segments share end vertex and that geometry is not split if the segments intersect only on the projected plane and not in reality (typically multilevel communications, when one is on the bridge across the other so that projected intersection is not real intersection).

Moreover, street networks have to be morphologically correct, which means that geometries represent morphological connections, not other, usually transport-focused. That often mean simplifications of networks to eliminate transport geometries like roundabouts or similar types of junctions, or dual lines representing dual carriageways. In certain cases, networks have to be snapped together, because due to traffic-calming measures, some junctions might not be connected when they should be.

Finally, the network needs to be consistently drawn in terms of inclusion of different levels of network hierarchy. Hence the definition of what is considered as a street is a minor connection is crucial for comparability of results and should be included in any research.

As per data availability, networks are widely availably. However, geometries mostly represent transport network and often do not follow ideal topological rules. The pre-processing to ensure that all three points above are fulfilled is hence necessary and can be partially automatised either using `momepy.network_false_nodes` or using methodology outlined by @krenz2018, using conventional GIS tools. However, there might be cases when more complicated procedures should be employed, either to ensure that the algorithm is more precise or to include manual steps.

##### Spatial unit
The identification of a reliable, significant and universal spatial unit of analysis is of crucial importance. However, the situation with traditionally used plot is complicated.

###### Plot
In traditional Urban Morphology, the *plot*, is considered to be the smallest meaningful unit of spatial subdivision and a fundamental component to understand the spatial structure of the ordinary fabric of urban settlements [@panerai2004; @porta2014] and their processes of formation and transformation in time [@whitehand1981]. 

However, despite its significance, the plot remains a problematic construct. At *ontological* level, there is no agreement on *what exactly a plot is*: indeed, it has been variously defined as “*a land-use unit defined by boundaries on the ground*” [@conzen1969, p. 128], *a module* of the urban tissue constituted by a built-up area and its open pertinent area [@caniggia1979], a piece of property, subject to subdivision and amalgamation as a result of successive patterns of occupation [@moudon1986], or again, according to @bobkova2017a, as “*a basic unit of control*”, “*a fundamental link between spatial and non-spatial medium*”, “*a connection between built space and space of movement*” and “*the framework for building evolution over time*” (p. 47.5). And crucially, more often than not, these definitions may represent very different entities on the ground “*potentially leading to misinterpretation and so a somewhat obscured picture of the dynamics of urban form*” [@kropf1997, p.1].

The second problem has to do with relevance and applicability of the plot to different urban contexts. In literature, plots have been predominantly used to study and characterise traditional urban tissues that having evolved incrementally at the plot level [@bobkova2017a; @conzen1969], are quintessentially plot-based [@panerai2004]. This is however not the case for urban forms that came about after the Second World War, which appear to respond to substantially different rules of organisation [@dibble2016; @feliciotti2018]. For these tissues, “*plots no longer have a structuring role*” [@levy1999 p.83], and hence can hardly be a suitable unit of analysis. While the process of identifying plots in traditional tissues is somewhat less controversial, the same is not true in contemporary ones (figure \ref{fig:glasgow}). 

![Comparison of traditional (left) and modernist (right) urban tissues in Glasgow. Plots are clearly better identifiable—even just visually—in the former, where distinction of public and private space is clear-cut, than in a modernist housing estate, where the transition between public and private is blurred. Source: Ordnance Survey MasterMap, January 2019 (EDINA Digimap Service)](source/figures/ch6/glasgow.pdf "Comparison of traditional and modernist urban tissues in Glasgow"){#fig:glasgow width=100%}

In addition to this issue, the identification of plots in the urban fabric also poses a series of *analytical* problems: given a map or a satellite image, how to consistently determine plot boundaries? And, in case of existing datasets, what do they *actually* represent? What definition of plots do they adopt? Are different datasets comparable?

Not all mapping agencies explicitly report plots and, even when they do, not all of them define or represent plots in the same way. In some spatial databases, as in the Swiss Katasterwesens, plots are represented as unitary land parcel, whilst in other cases, ownership-based plots can be made of multiple unlinked features, as in the French Cadastre, limiting comparability between different datasets. In other cases, the identification of plots from available sources is inferred by the analyst via resource-intensive manual interpretation. However, that makes the resulting procedure on one hand unsuitable for large scale analysis, and on the other potentially biased, as heavily dependent on both individual interpretation and the often uneven quality of the underlying data. Indeed, while through open-data policies [@huijboom2011] and Voluntary Geographical Information System (VGIS) [@barrington-leigh2017] the availability of free-to-use geo-data is growing dramatically, their quality, coverage and resolution is often insufficient to determine individual plots and generally limited to building footprints, street centrelines, natural features and administrative boundaries. All of this reduces considerably the reliability of the analysis and the universality of its results.

Given the aforementioned issues, and despite plots being still widely used in Urban Morphology to capture the “*pattern of human intention and activity*” [@kropf1997, p.5], they are ill-suited as basic unit for UMM applications.

###### Morphological tessellation
One of the few alternatives of plots proposed in the literature [@hamaina2012a; @hamaina2013, @schirmer2015; @schirmer2019] is Morphological Tessellation (MT). A method of deriving a spatial unit of analysis, the Morphological Cell (MC), which is able to convey reliable, universal and meaningful plot-scale information and, at the same time, to minimise manual labour, subjective interpretation and data dependence. Hence it is proposed to use MT as a substitute of plot in urban morphometrics.

At the core of the proposed implementation of MT lies the *Voronoi tessellation* (VT), a method of geometric partitioning that from a planar set of *‘seeds’* generates a series of polygons, known as *Voronoi Cells* (VC). Each VC encloses the portion of the plane that is closer to its seed than to any other (figure \ref{fig:voro}), ideally representing its ‘*influence zone*’\footnote{The term Voronoi Tessellation can be used to describe both the process of partitioning space (method) and the geometric mesh it generates (output). In this text, the two meanings are used interchangeably.}.

![Voronoi tessellation based on randomised seeds. Each colour represents the area of one tessellation cell (influence zone). Dashed lines end in infinity](source/figures/ch6/voro.png "Voronoi tessellation based on randomised seeds"){#fig:voro width=50%}

VT has been already used in relation to urban form, in the context of spatial clustering algorithms [@dogrusoz2007] and built-form geometry generalisation techniques [@ai2007; @basaraner2004; @li2004; @liu2014], or as input for image-based pattern recognition [@yu2017]. In recent years, MT was used to study the micro-scale properties of the urban fabric [@hamaina2012a; @hamaina2013] in order to produce a reliable method for urban form patterns’ recognition, which pioneered the generation of VC from building footprints. Later, Schirmer and Axhausen [-@schirmer2015; -@schirmer2019] devised a method to define “*influence zones*” around buildings using a “*topological skeleton*” of unbuilt space that is mathematically similar to MT. In parallel, Usui and Asami [-@usui2013; -@usui2017; -@usui2019] included the street network as an additional input alongside the building footprint to the VT algorithm, to mimic the plot structure of traditional Japanese urban fabrics.  Whilst the generated mesh shows remarkable similarity to the plot pattern, its main limitation is the inability to capture the spatial pattern of modernist (post WWII) urban tissues and the highly variable distance between building and street that is typical of such fabrics. On a similar vein, Araldi and Fusco [-@araldi2017; -@araldi2019] developed an approach based on VT and street segments to define a spatial unit based on the pedestrian point of view.
In all these cases, the use of Voronoi tessellation helped to rigorously and reliably cluster components according to their configuration although, as pointed out by @usui2019, the relationship between MC and ‘conventional’ plots has never been directly tested to date. In this sense, the MT approach is to be intended as a continuation of this line of works, insofar it too utilises the VT procedure. However, unlike previous studies, this research aims to provide a fully operational and replicable method by examining the details of the tessellation process and its parameters, and testing the similarity of morphometric characters as measured on both MC and plots through direct comparison.

Yet, the potential and applicability of morphological tessellation is still largely unexplored.

\newpage

#### Analytical aggregations

Since morphological as well as morphometric analysis mostly aims to capture patterns of urban form, they must describe single elements as well as their spatial configurations and relationships. To do so, larger analytical units must be identified. Generally, we can distinguish two approaches of aggregation of fundamental elements into larger units: area-based and location-based [@berghauserpont2014].

##### Area-based
==be super careful with critique Re MAUP here==
 Area-based approaches divide space into preselected units, i.e. administrative boundaries [@gielen2017], abstract projected boundaries (typically grid) [@galster2001], or larger morphological structures such as a block [@gil2012] or a Sanctuary Area [@dibble2017]. However, such methods face two connected issues, together named “Modifiable Areal Unit Problem” (MAUP) [@openshaw1984]: scale issue (how big the area of aggregation should be) and aggregation issue (where should we draw its boundaries). Area-based approaches are prone to both of them, particularly the latter: a change of the boundary, for example the voting district, might affect the analysis’ results.

*keeping in mind the issues, there is a significant scope to study morphological aggregations*

*going from the plot scale, we recognise street edge, block, street, resulting in either urban tissue if we follow one definition or in SA if we follow Mehaffy.*

*smallest aggregation is street edge, defined as ...*
- illustration

*then we have block, which Kropf calls plot series*
- illustration
	_The above highlights that while the block can unequivocally be defined as an aggregate of plots surrounded on all sides by street spaces, it is ambiguously related to those street spaces when taken as an isolated entity. A block can be either (1) the result of combining several plot series, each connected with a different single street, or (2) an aggregate of plots that may be connected to two or more streets. One way or the other, the block occupies the same level as the plot series in the generic structure, but as a resultant form (for this reason ‘blocks’ is set in square brackets in the diagrams)._ ==Kropf p.47==


*then we can have street - various definitions*
- illustrations

*urban tissue could be seen as the largest form-related aggregation and literature focuses on this concept from several perspectives. We have tissue/fabric, morphological region and UST. While SA can sometimes overlap, it by definition captures different concept.*
- ==morphological region (Vitor's paper), Kropf p.15, Araldi, etc.==
- ==link back to classification ch2==
- illustration

*while some are perfectly meaningful and MAUP is tiny (edge, block), some are suboptimal (SA).*

##### Location-based
Location-based approaches generate analytical units independently for each source-element as a unique aggregation around it, typically at walking or driving distance, where distance is measured either along the street network (network distance) or an approximation of it (for example: as a crow flies). Therefore, the aggregated values are uniquely and consistently generated for each source-element (e.g. building), and the effect of arbitrary data aggregation is minimised, resolving MAUP’s aggregation issue. For this reason, literature, including the research presented in this work, prefers location-based analytical units, as their nature partially resolves MAUP. The scale problem part of MAUP is present also in location-based methods, and it is up to the methodology adopted on a case-by-case base to limit its effect to a minimum.

Currently, morphological literature relies on a few methods to define an aggregation of units in a location-based manner. The most straightforward is based on simple Euclidean (as-crow-flies) distance from the elements of analysis (typically radius of 400 metres around a building) [@schirmer2015]. However, such an approach does not reflect the actual morphological situation on the ground. In some instances, such as in in traditional compact urban tissues, it can capture hundreds of buildings within 400 metres, but only a few in sparse modernist urban tissues, leading to fundamental differences in the amount of information captured, causing issues of comparability of such information.

Excluding effect of certain morphologies from the definition of aggregations overcomes method based on metric reach. Following street network or axial map of urban form [@berghauserpont2014; @marcus2017], it captures the area which is possible to reach within a set distance (mostly metric). As a location-based method, reach is useful because it reacts to unequal morphologies, but only through constrains that limit accessibility to space, rather than through a detection of a difference in urban form itself. The logic is based on the cognitive experience of cities but limited to accessible open spaces, excluding the intra-block relationships. It can generate situations of two buildings facing each other across the block (hence directly influencing each other) not being aggregated together, ignoring their relationship.

Both Euclidean distance and metric reach methods cannot capture the change in the granularity of urban tissues, hence effectively measuring different information in granular than sparse tissues. In the case of reach, the distance could be defined topologically as a number of steps on the network (represented by the graph) [@berghauserpont2014], allowing to recognize the change in the pattern of aggregations, but it still does not eliminate the issue of intra-block relationships. On top of that, network-based methods faces issues in data availability - street networks usually need significant adaptations before they can be used, as they are typically drawn for traffic purposes, not morphological ones; axial maps are scarcely available, and their generation needs a very specialised type of morphological knowledge limiting the applicability of such method.

The third method present in literature is K-nearest neighbour (KNN) analysis, which is also based on Euclidean distance but using it differently. It defines aggregation as a set number of nearest neighbours, defined via as-crow-flies distance. Whilst only scarcely used in urban morphology [@liqiang2013], it has potential as such an approach might reflect changes in the granularity of urban tissues. However, due to the Euclidean definition of nearest neighbours, it cannot react to the detail of some spatial configurations (e.g., be able to detect linear patterns with natural boundaries between as features across the boundary might be closer than those within the pattern). Theoretically, KNN could be used together with reach analysis, joining both the ability to capture morphology represented by networks and scalability of KNN, but we are not aware of any research using this concept so far. However, it would still not resolve the issue of intra-block relationship.

It should be pointed out that the MCs do offer added values that are relevant on their own in the context of aggregation, regardless to their similarity to the plots. These have to do with the potential innovations – yet largely unexplored – which are triggered by the very nature of this geometry. For example, unlike other methods of urban form partitioning, the MT covers uniformly the totality of space within the set study area, allowing to capture the topology of contiguous space at the plot-level. Indeed, since all MCs are determined by adjacency, by using MT it is possible to think in terms of topological distance (set number of topological steps between cells) rather than geographic distance (set metric distance around elements, either “as the crow flies” or along the street network). Moreover, thinking in terms of topological distance as opposed to metric, the MT can be used to define new aggregated analytical units that are able to capture the immediate area of influence of a building on its surrounding fabric and, at the same time, of the surrounding fabric on the building. Indeed, since the size of each MCs depends on the granularity of the urban structure, the spatial representation of a set topological distance would be far smaller for a MC located in a fine-grained built-up area than for the same located in a coarse one (figure \ref{fig:contiguity_diagram}). Crucially, this is a kind of information that would not be possible to access with plots alone, which allows to reframe the very idea of ‘proximity’ by rethinking the relationship between scale and spatial meaning, thereby enhancing the ability to capture the context in UMM analysis.

![Relationship between morphological cells of topological distance 2: the red geometry represents the adjacency network of neighbouring elements (buildings, MC) at topological distance 1 (adjacent neighbour of first order), while blue geometry represents the boundary of the aggregated analytical unit of topological distance 2 for each of the highlighted buildings. In the image, a fabric characterised by fewer and sparser buildings (b) generate larger cells and aggregated units compared to a denser and more compact fabric (a).](source/figures/ch6/contiguity_diagram.png "Relationship between morphological cells of topological distance two"){#fig:contiguity_diagram width=100%}

Topology captures the information on adjacency of neighbouring elements (cells) - two cells are neighbouring if they share at least one point (so-called Queen contiguity) or one segment (so-called Rook contiguity). It defines the proximity of elements in terms of the number of steps needed to get from each element A to each element B. Topological relationships can be of two types - unconstrained, if not limited by any other element than tessellation itself, and constrained, if the step between two neighbours is impeded by constraint (a block is the maximum number of topological steps from element without the need to cross the street network, while the street network is the constraint in this case). Thus, we can define an aggregation around each element based on a number of topological steps (topological reach) on the morphological tessellation, where aggregation defined by n steps includes all morphological cells which we can reach within x <= n steps. 

### Models of urban form
*models which are linking these or some of these elements together. Does not include models based on a singular element; the key focus here on how are elements linked together.*

- the way we link fundamental elements and their aggregations matters as well

*analytical models of urban form are not often specified in literature, and mostly are only assumed.*

==_RESEARCH NEEDS TO BE DONE HERE_==

#### Hierarchical models
*two analytical models have been recently defined, Kropf's and Dibble's, both being hierarchical in nature. Which means that...*

*Kropf model has urban tissue on top and rooms on the bottom. It is based on the combination of cannigian and conzenian theory. (REF Oliveira)*

*Dibble's hierarchical model has SA on top and plot on the bottom and focuses on morphometric assessment of SAs*

#### A City is not a Tree
*Alexander points out that city does not work in a tree-like hierarchy, which is reflected in both models above, but as a semi-lattice of connections. However, none of these analytical models tends to reflect that and Alexander's own work on pattern language does not help in morphometric analysis.*

#### Relations between elements and their aggregations
*Some models focus on specific elements of urban form, but elements from different approaches are usually not linked together.*
- Node vs edge and their relation to other elements

*While literature shows that there is a wide spectrum of elements and their aggregations useful for morphometric analysis, no method links then into a singular overarching model, which would in turn take a structure of semi-lattice instead of simple tree-like hierarchy.*
==**gap** no model joins links all these approaches into a singular model==


## Theory of Relational Model of urban form
*To put things forward, this research proposes relational model of urban form for urban morphometrics. At the same time, it rejects the idea of SA as OTU and assumes that urban tissue is the optimal OTU.*

### Relational model as an analytical tool
_how to build a model based on that and relations, which is not strictly hierarchical?_

_Relational model of urban form_
*relational model acknowledges that there is an identifiable relation between all elements of urban form and their relations. As such, it accommodates all analytical aggregations into a singular model, linking all potential measurable characters to the smallest element.*
- unlike models above, RM is analytical not conceptual or structural
- the general concept of RM

_within this research, RM is operationalised based on morphological tessellation. That is not the rule, but one interpretation and the same could be done with plots and different aggregation models._


#### Tessellation-based relational model

_is mt good unit?_
_MT tested here, RM can be tested only in application, hence in next chapter ==LINK TO CH6 DISCUSSSION & INTRODUCTION==_

_HYP_
_tessellation is good subsititute of plot_ +test here (Zurich)
_H aerial contiguity is better than any other aggregation model_ +test here (ISUF)
_H network configuration is better than network reach_ +based on literature (SS)
_We can use MT to build a relational model based on aerial contiguity & network configuration, limiting the data requeirements at the same time._ +tested in practice in Ch7
_relational combination of both area-based and location-based aggregations (minimising MAUP for each)_

##### Subsets of elements
==revise==
Subsets are combination of topological scales and fundamental elements. Overlap of characters from subsets, where each subset is representing different structural unit, gives overall characteristic of each duality building - cell which is the key for identification of DHC.

Scale and subset is a set of relationships.

###### Small/Single
*topological distance 0*
In the case of building and tessellation cell it captures individual character for each cell. In case of street segment and node, it captures value for segment or node which is then applied to each cell attached to it. 
- building
- tessellation cell
- street segment
- street node

###### Medium
*topological distance 1*
In the case of building and tessellation cell it captures individual character for each cell derived from the relation to adjacent elements. In case of street segment and node, it captures value for segment or node which is then applied to each cell attached to it. 
- adjacent buildings
- neighbouring cells (queen)
- neighbouring segments
- linked nodes

###### Large
*topological distance 2-10*
In the case of cells, it captures individual character for each cell derived from the relation to cells within set topological distance. In case of joined buildings and block, it is shared values among all elements within one structural unit. In case of street segment and node, it captures value for segment or node which is then applied to each cell attached to it. 
- joined buildings
- neighbouring cells (queen 2+)
- block
- segment step neighbours 2+
- segment metric reach
- node step neighbours 2+

### Urban tissue as a unit of urban form
_Refer back to chapter 2 and discuss the reason why tissue is optimal_
- _it reflects unconstrained morphological unit_
- _tissue as OTU (link to Ch4 and Ch5)_ ==after ch4 is done==
- _morphological regionalizaition (Oliveira)_
- _heavily refer to literature which sees tissue as unit as well. Why SA is not a unit is in chapter 4_

==Hypothesis *Urban tissues can be recognised by empirical measuring of the physical structure represented by the relational analytical model of urban form in a form of homogenous clusters.*== (here or in the next chapter)

## Method of tessellation testing
*this section tests the viability of morphological tessellation as a smallest unit based on its ability to substitute plot and topological aggregation compared to other options.*

### Tessellation as a unit
*Tessellation method is first defined and then tested.*

#### Generation of Morphological Tessellation 
Whenever observing a map or a satellite view of a city, the eye of the observer is caught by the existence of a fundamental relationship between buildings – their geometry and spatial configuration – and the plot pattern. This ‘*intuitive*’ relationship is the reason why approaches based on VT appear to *‘make sense*’ when applied to the urban form of cities: by partitioning the space into cells, they capture the way buildings relate to each other in space and, more precisely, give a spatial meaning to the “*morphological influence*” that each building exerts on its immediate spatial context [@usui2017]. This, in turn, implicitly captures how spatial configuration affects visibility, light penetration, ventilation, movement, etc. around each and every building [@hamaina2012].

The main advantage of methods based on VT is the capacity to derive objective spatial partitions that are applicable to every type of urban tissue in a way independent from the researcher’s subjective interpretation. In addition, most of these methods [@hamaina2012a; @hamaina2013] require minimum data input, as they fundamentally rely on the polygon that describes the footprint of a building. Similarly, the proposed MT method only requires a polygon layer representing building footprints (figure \ref{fig:mt_method}a). From this, MT moves forward in five steps:

1.	*Inward offset from building footprint* (figure \ref{fig:mt_method}b). The offset is necessary to avoid overlaps between boundaries of adjacent buildings and generate a gap between adjacent geometries which will later define the boundaries of the cell. 
2.	*Discretisation of polygons’ boundaries into points* (figure \ref{fig:mt_method}c). As VT can only be generated from point features, the polygonal shape of the building footprint needs to be approximated as series of points to be placed at regular intervals along its boundary, where generated points retain the ID of the building they belong to.
3.	*Generation of Voronoi cells* (figure \ref{fig:mt_method}d). VC are generated around each of the points representing the building footprint. Again, the original ID of the building is preserved in the resulting VC.
4.	*Dissolution of Voronoi cells* (figure \ref{fig:mt_method}e). All VCs sharing the same building ID – and hence generated from the same building – are dissolved in unitary geometries. This step provides a preliminary boundary of the MC.
5.	*Clip of preliminary tessellation* (figure \ref{fig:mt_method}f). As a geometrical construct, VCs tends to infinity as the boundaries of each cell are only defined by proximity with adjacent *‘seeds’*. However, when applied to the analysis of urban form, for obvious reasons no cell can tend to infinity. To avoid this, it is necessary to limit the maximum spatial extent of the tessellation by setting defined study area boundaries.

![The proposed MT method. Grey polygons represent building footprints, while red lines show the edges of tessellation at each step. 3a) Building shapes within boundary of study area (blue); 3b) inward offset from building footprint polygon; 3c) discretisation of  boundaries of polygons into points; 3d) generation of VCs around points: at this stage, the edges of cells (red) tend to infinity; 3e) dissolution of Voronoi cells based on original building ID; 3f) clip of preliminary tessellation by study area.](source/figures/ch6/tesdiag.png "The proposed MT method"){#fig:mt_method width=100%}

Three of the five steps listed above, namely inward offset distance (step 1), discretisation interval (step 2) and clipping method (step 5), require setting parameters that can have a significant effect on the resulting tessellation. As such these need to be evaluated in greater detail. More specifically, in the case of inward offset distance (step 1), the selection of too large values may cause the collapse of narrow parts of building shapes and loss of detail, while too small ones may generate unwanted “*saw-like*” geometries between adjacent buildings. Similarly, a large discretisation interval (step 2) may produce the same “*saw-like*” geometry issue, whilst the opposite would increase exponentially computational demand (figure \ref{fig:sawdiag}). Additionally, since the two parameters are interlinked, their individual effect on the shape of each cell is not independent: as such, their combined effect needs to be balanced to generate geometries with insignificant shape deviation and minimum computational burden. Finally, the adoption of a clipping method for the tessellation (step 5) also requires considerations in order to appropriately limit the focus of the analysis to the urbanized footprint and exclude large open un-built spaces while limiting potential MAUP effects [@openshaw1984]. Due to the importance of correctly setting these parameters, Section _4.2REF_ will discuss the adopted method for the determination of inward offset distance (step 1), discretisation interval (step 2) and method.

![Illustration of the effect of improper combination of inward offset distance and discretisation interval causing “saw-like” geometry on the boundary bethween adjacent buildings (b) compared to ideal combination (a).](source/figures/ch6/sawdiag.pdf "Illustration of the effect of improper combination of MT parameters"){#fig:sawdiag width=70%}

The conceptual sequence described in this section, was translated into a Python code, building its key parts on the capability of SciPy [@jones2001], Shapely [@gillies2007] and GeoPandas [@jordahl2019]. Computation was run on Ubuntu Bionic 18.04 running at Amazon Web Services EC2. _The resulting Python script is released as part of the open source Python package named “momepy: Urban Morphology Measuring Toolkit"._

#### Morphological Tessellation and plots: data and comparison method
##### The dataset
_add reasoning why Zurich is here while everything else is done on Prague_
The MT method and the informational value of MCs compared to plots were tested within the administrative area of Zurich (figure \ref{fig:extent}). This was chosen for its historically characterised and heterogeneous urban fabric as well as for the availability of the ‘_Amtliche Vermessung_’ dataset, a freely-accessible resource containing high-quality information on cadastral plots and building footprints. Before generating the MT, data was cleaned as follows:

1. From the *cadastral layer*, which covers the 100% of study area, all features not containing buildings (e.g. streets or large open spaces) were removed, as they do not represent built-up form;
2. From the *building layer*, features smaller than 30 m^2^ were filtered out, as such smaller objects are likely ancillary structures rather than actual buildings.

![The selected study area, defined by the administrative boundary of the Zurich Kanton (left); the Langstrasse area in Zurich (right) was selected for testing the tessellation algorithm parameters: the red-line boundaries follow the street centerlines.](source/figures/ch6/extent_cases.png "The selected study area of Zurich"){#fig:extent width=100%}

##### Definition of MT Parameters: inward offset distance, discretisation interval and clipping method
To determine the optimal setting for inward offset distance (step 1) and discretisation interval (step 2), a test was run on a portion of the Langstrasse area in Zurich (Figure 5), a heterogeneous fabric predominantly characterised by adjacent buildings (significantly more prone to error than isolated buildings) limited by the street network . We considered several combinations of inward offset (from 0.1 to 1 meter) and discretisation interval (from 0.05 to 5 meters) and evaluated them against the most precise setting (0.1 / 0.05), which provides the highest-resolution tessellation with minimal effect on the building shape. We then assessed deviation of cell perimeter and area values for each combination, as well as its computational demand: the latter is a function of the number of discretisation points, as these directly impact on memory demand. The result of this test is presented in Section _5.1_ REF. Based on it, the optimal combination of the two parameters was adopted to generate the MT in later stages. 

Finally, in order to clip the tessellation (step 5) we adopted a definition of urban footprint aligned with Angel et al. [-@angel2007; -@angel2018], and limited the study area extent by setting a 100m buffer from the built-up area. However, to test the robustness and stability of the buffer and avoid arbitrary selection, we also tested 14 other buffers, ranging from 10 to 300 metres. The stability of the 15 buffer distances is discussed alongside the comparative analysis in Section _5.2_ REF.

##### The informational value of MT vs plots: the 12 morphometric characters
To test the informational value of the MCs compared to plots, 12 morphometric characters (table \ref{tab:chars_zurich}) grouped into the six morphometric categories (dimension, shape, spatial distribution, intensity, connectivity and diversity)  proposed in chapter 3, are selected and measured on both the cadastral layer and MT layer, at the 15 buffer distances mentioned in section _3.1_ REF. With the exclusion of Reach Centrality, which is measured using the *Urban Network Analysis (UNA) Toolbox* [@sevtsuk2012], all characters are computed using Python scripts released as part of the momepy package.

\newpage
\begin{landscape}
\begin{longtable}[]{@{}lll@{}}
\caption{Selection of morphometric characters used for comparison} \label{tab:chars_zurich} \\
\toprule
Category & Character & Formula\tabularnewline
\midrule
\endhead
Dimension & Area & \(\text{area}\)\tabularnewline
& Longest Axis Length (LAL) &
\(max\{ d_{1},\ d_{2},\ \ldots,\ d_{n}\ \}\) \tabularnewline
Shape & Circular Compactness &
\(\frac{\text{area}}{\mathrm{\text{area\ of\ enclosing\ circle}}}\) \tabularnewline
& Shape Index &
\(\frac{\sqrt{\frac{\text{area}}{\pi}}}{0.5*\mathrm{\text{LAL}}}\) \tabularnewline
& Rectangularity &
\(\frac{\text{area}}{\text{area}_{\text{MBR}}}\) \tabularnewline
& Fractal Dimension &
\(\frac{2log(\frac{\text{perimeter}}{4})}{\log(\text{area})}\) \tabularnewline
Spatial Distribution & Orientation & \(\left\{ \begin{matrix}
\text{azimuth}_{\text{MBR}},\ \ \ \ \ \ \ \ \ \ \ \ \ \ \text{azimuth}_{\text{MBR}} < 45{^\circ} \\
\text{azimuth}_{\text{MBR}} - 2(\text{azimuth}_{\text{MBR}} - 45{^\circ}),\ \ \text{azimuth}_{\text{MBR}} \geq 45{^\circ} \\
\end{matrix} \right.\ \) \tabularnewline
Intensity & Frequency & \(\sum_{dist = 1}^{400}\text{element}\) \tabularnewline
& Coverage Area Ratio (CAR) &
\(\frac{\text{are}a_{\text{building}}}{\mathrm{\text{area}}}\) \tabularnewline
Diversity & Gini Index of Area &
\(G = \frac{\sum_{i = 1}^{n}{(2i - n - 1)\text{are}a_{i}}}{n\sum_{i = 1}^{n}{\text{are}a_{i}}}\)
\tabularnewline
& Gini Index of CAR &
\(G = \frac{\sum_{i = 1}^{n}{(2i - n - 1)\text{CA}R_{i}}}{n\sum_{i = 1}^{n}{\text{CA}R_{i}}}\)
\tabularnewline
Connectivity & Reach Centrality &
\(R^{r}\lbrack i\rbrack = \parallel \{ j \in G - \{ i\}:d\lbrack i,j\rbrack \leq r\} \parallel\)
\tabularnewline
\bottomrule
\end{longtable}

\begin{small}
$d_1 \ldots d_n$ are diagonals of convex hull of element.\newline
$MBR$ is minimum bounding rectangle.\newline
$Azimuth$ is defined as orientation of axis between 1st and 3rd quadrant.\newline
“The reach centrality, $R^r [i]$, of a building $i$ in a graph $G$ describes the number of other buildings in $G$ that are reachable from $i$ at a shortest path distance of at most $r$.” [@sevtsuk2012, p.9].
\end{small}
\end{landscape}

Once all morphometric characters are calculated for cadastral plots and the 15 MT layers (at each buffer distance), the similarity of the resulting values for the two datasets is evaluated using three methods: 1) Spearman’s rank correlation; 2) Normalised root squared mean deviation (NRSMD) and 3) Accuracy of significant patterns defined by local Moran’s I indicator of spatial autocorrelation (LISA) [@anselin2010].
Spearman’s rank correlation is “*a measure of the correlation between ranks, calculated by using the ranks in place of the actual observations in the formula for the correlation coefficient r*” [@kokoska2000, p.372] (see Equation 1) and was used due to non-normality of distribution of measured values. It ranges from -1 (negative correlation) to 1 (positive correlation), with values > 0.5 or < –0.5 indicate moderately significant positive or negative correlation [@hinkle2003].

(@eq_spearman) $\r_{s}=1-\frac{6 \sum d^{2}}{n\left(n^{2}-1\right)}$,

where $d_{i}=\operatorname{rg}\left(X_{i}\right)-\operatorname{rg}\left(Y_{i}\right)$ is the difference between the rank of observed and expected value and $n$ is the number of observations [@kokoska2000].

NRSMD is a frequently used measure of “*an estimate of the standard deviation of residuals from the model*” [@alexander2015, p.5] normalised by the range (see Equation 2), and it is used to measure the difference between the expected and observed values, normalised by the range. As a ratio of deviation, it ranges from 0 to 1, where 0 means no deviation and 1 means deviation equal to the range of values. As the range is sensitive to outliers, NRSMD might not be relevant for characters of *Dimension* category.

(@eq_nrsmd) $\operatorname{NRMSD}(y, \hat{y})=\frac{\sqrt{\operatorname{MSE}(y, \hat{y})}}{y_{\max }-y_{\min }}$,

where $\operatorname{MSE}(y, \hat{y})=\frac{1}{n} \sum_{i=0}^{n-1}\left(y_{i}-\hat{y}_{i}\right)^{2}$ where $y, \hat{y}$ are observed and expected values.

Accuracy is “*closeness of computations or estimates to the exact or true values that the statistics were intended to measure*” (OECD, 2006) and is here used to measure the similarity of significant spatial clusters identified from the cadastral layer and those identified from each version of the tessellation (see Equation 3). Since studies in Urban Morphometrics are more interested in uncovering *recurrent patterns* in urban form rather than *actual values* [@feliciotti2018], this method is probably the most relevant of the three. In fact it measures whether corresponding features from both datasets (cadastral plots and morphological cells in this case) significantly fall within the same cluster (i.e. p <= 0.05), with values ranging from 0 (no match) to 1 (perfect match).

(@eq_alisa) $\mathrm{aLISA}=\frac{S C_{\text {match}}}{S C_{\max }}$,

where $S C_{\text {match}}$ is the number of the elements belonging to the same significant cluster (HH, HL, LH, LL) in both $y, \hat{y}$ and $S C_{\text {max}}$ is the number of the elements $\hat{y}$ belonging to any significant cluster. The adjacency matrix used for LISA represents 200 metres Euclidean distance from each building.

It must be noted that, for the statistical comparison of selected morphometric characters across the MT layers and the cadastral layer, these must correspond perfectly.  However, whilst there is a 1:1 match between MCs and *buildings*, the same does not apply to MCs and plots, as the latter may contain one building (single-building plots) or more than one (multi-building plot).  To resolve this issue, the building layer is used as a proxy between tessellation and cadastre and, therefore, all morphometric characters computed on both MCs and plots are associated to the building layer (i.e. each building is linked to the value of its MC and of the plot it sits on). However, to better understand the impact of ‘*single-building*’ and ‘*multi-building*’ plots (79% and 21% of all plots respectively), the three methods described above are applied to the whole dataset and, separately, for *single-building* and *multi-building* plots. In particular, we expected that *multi-building* plots, although important for their effect on the overall analysis, would hold limited comparative value for most of the assessed morphometric characters (perhaps with the only exclusion of covered area ratio and Gini index of CAR, which capture compatible concepts).


### Topological contiguity of tessellation as an aggregation model
The definition of aggregated analytical units via the topology of morphological tessellation can overcome issues of the three methods described above and provide a more consistent way to understand the relationship between adjacent elements of urban form (in the case of buildings or morphological cells). This paper is testing this hypothesis in the case of Prague, Czechia.

#### Comparing aggregation methods
The methodology of this research follows a twofold approach, analysing both small scale case studies and urban scale statistical data. Small scale case studies examine the difference between three methods extracted from literature (Euclidean distance, metric reach, K-nearest neighbour) and unconstrained topology of morphological tessellation in different types of urban form; large scale statistical analysis examines the parameters of these methods of aggregation across the whole of Prague.

Prague was selected as a case for its morphological richness of multiple historical layers still intact. The study area is limited by the administrative boundary of the city, but still extends the built-up area of the city by a large margin. The data used within this study were provided by Prague’s Institute for Planning and Development (www.geoportalpraha.cz).

We compare how each of the tested methods aggregate tessellation cells (being smallest spatial unit) within two scales: one achieved by nine topological steps, the equivalent of approximately 400 metres used in morphological analysis to represent walking distance of 5 minutes; and one achieved by 4 topological steps, representing roughly 200 metres. The number of neighbours for KNN is then derived from mean number of neighbours captured by each of the topological distance and metric reach, to keep the dimension comparable (table \ref{tab_aggr}).

| Topology of MT | Euclidean | Metric reach | KNN |
|:--:|:--:|:--:|:--:|
| 4 steps | 200 metres | 200 metres | 70 neighbours |
| 9 steps | 400 metres | 400 metres | 320 neighbours |

Table: Default topological distances and their equivalents. Values are derived from the summative analysis of topology-based aggregations defined around each morphological cell on Prague. \label{tab_aggr}


The aim of small-scale analysis is to understand how each of the four methods identifies and represent the same information across 5 types of urban form - medieval organically grown, 19^th^ century compact perimeter blocks, 20^th^ century mixed single and multi-family villas, 20^th^ century modernist housing, and 20–21th century industrial estates. It should allow to ascertain how consistently each method distinguishes variations in form and morphological behaviours.

At the urban scale we conduct statistical analysis to compare the distribution of values derived from the whole of Prague (its administrative boundary). Statistical distribution of data across whole urban area describes the spread and variance of values, which can be used to assess the ability of each method to capture the intended information across types of urban tissue. To understand the different performance of each method, we compare distributions of two descriptive variables as a proxy for the performance assessment – number of neighbours and covered area. 

The first variable is the number of neighbours captured. Neighbours represented by buildings and related tessellation cells capture most of the morphological information. For that reason, it is desirable to use method which will identify somewhat similar number of neighbours no matter the urban tissue to keep the similar essence and amount of information to maximise comparability of values, meaning that the distribution of such values should have relatively small standard deviation and be close to symmetrical distribution to have the similar positive and negative deviations from the mean.

The second variable should represent the concept of geographical extent of aggregation, as it bears the information of the scale of each type of urban tissue and therefore could describe the ability of each method to adapt to the scale. Amongst the possible measurable variables are mean distance to neighbours, maximum distance to neighbours and area covered by aggregation. Because they all represent scale and extent of aggregation of elements (buildings, tessellation cells), we use only area covered to represent them all as it is the most straightforward one and easy to understand. The statistical distribution of covered area should represent the adaptability of aggregation method. For that reason, ideal outcome should have high standard deviation and high range of values, meaning that many different options (levels of granularity of urban form) are all captured. 


## Results

### Tessellation as a unit

#### Determination of optimal parameters of the MT algorithm
The test performed on the selected inward offset ranges (from 0.1 to 1 meter) and discretisation intervals (from 0.05 to 5 meters) allowed to assess computational demand (i.e. number of discretisation points) and deviation of cell perimeter and area for each combination. In terms of computational demand, as shown in figure \ref{fig:tess_pts}, it appears that the discretisation segment length has an exponential effect on the number of generated points. For values below the mean (tail of the distribution), computational demand remains relatively stable, whilst for higher values (head of the distribution) it grows sharply, more than doubling at each step. Discretisation intervals ≥ 0.5m are therefore preferred as more computationally effective.

![Relation of discretisation segment length and number of points generated. The red line illustrates the mean value above which the number of points more than doubles at each step](source/figures/ch6/tes_pts.pdf "Relation of discretisation segment length and number of points"){#fig:tess_pts width=100%}

The effect of inner buffer and discretisation interval on the deviation of the MC’s area compared to the high-resolution tessellation is insignificant for all tested combinations (0.00 and 0.01%), showing that, no matter the parameters, results are stable. In turn, the same effect on the MC’s perimeter is more pronounced (figure \ref{fig:tess_peris}) due to the aforementioned phenomenon of “*saw-like*” geometries (see section _3.1_) with percent deviation ranging from 0.05% to 7.4%. Focusing on the 0.5 metres discretisation interval, providing the balance between the MC shape detail and computational demands, deviation values range from 0.47% to 3.1% (figure \ref{fig:tes_offset}). This suggests that the combination of 0.5m metres discretisation interval and 0.4m inward offset distance provides the optimal balance in terms of effectiveness of computation and minimisation of error. These values are hence adopted as parameters in the computation of the MT in the next stages.

![The mean deviation in percents of perimeter of each cell for each combination of inward offset distance (vertical axis) and discretisation interval (horizontal axis).](source/figures/ch6/tes_peris.pdf "The mean deviation of perimeter of each cell"){#fig:tess_peris width=100%}

![Relation of inward offset distance and error margin, showing that for 0.4 meter, the error margin reaches its minimum.](source/figures/ch6/tes_offset.pdf "Relation of inward offset distance and error margin"){#fig:tes_offset width=100%}

#### Comparison between the cadastral layer and morphological tessellation
Having determined the optimal combination of the tessellation parameters (inward offset = 0.4m and discretisation intervals = 0.5m), the MT for Zurich is computed using *“momepy*".  From a first visual inspection of the generated layer, it is already possible to appreciate how the MT is able to nicely capture variations in size, grain and compactness of buildings (figure \ref{fig:four_ex_tess}), not dissimilar what observed in a typical cadastral layer. We subsequently calculate the 12 morphological characters in _Table 1_ for cadastral plots and tessellation cells. In the next section, their correlation at each buffer of tessellation is studied.

![Morphological tessellation cells as generated across four different areas of Zurich; 4a) organic tissue of Niederdorf; 4b) compact tissue of Langstrasse; 4c) detached villas of Hottingen; 4d) mixed post-war development of Friesenberg.](source/figures/ch6/four_ex_tess.png "Morphological tessellation cells as generated across four different areas"){#fig:four_ex_tess width=80%}

##### Spearman’s rank correlation
Using Spearman’s rank correlation, we find that correlation of measured characters ranges between 0.25 (fractal dimension) to 0.89 (reach), with differences between morphometric categories and between *single-* or *multi-building* plots. Characters in the *Shape* category exhibit the worst performance, with insignificant correlation for the whole sample (~0.27) and multi-building plots (~0.09) and low significance for single-building plots (~0.42). This result was expected, due to the intrinsically different geometry of the two spatial units (MC and plots) and to the existence of multi-building plots.

*Dimension* characters inherently differ between *multi-* and *single-*building plots, showing only low significance for the former (~0.35, ~0.4) and high significance for the latter (~0.83, ~0.7). Remaining characters show moderate or high significance for all samples, with higher values for single-building plots (figure \ref{fig:spearman} and Table 2). Results for all buffers are quite consistent, with fluctuations observed only at smaller distances (< 50m), indicating stability of the selected value of 100m.  

![Spearman’s rho rank correlation between cadastral values and each of the selected buffers of tessellation based on the whole dataset (figures for single and multi-building plots are found in the Appendix XXX).](source/figures/ch6/spearman.pdf "Spearman’s rho rank correlation between cadastral and MT values"){#fig:spearman width=100%}

\begin{longtable}[]{@{}lllll@{}}
\caption{Spearman’s rank correlation of the whole dataset, single-building plots and multi-building plots at 100m buffer (emphasis reflects significance of correlation).} \label{tab:spearman_results} \\
\toprule
Category & Character & All &
Single & Multi\tabularnewline
\midrule
\endhead
Dimension & Area & \emph{0.4767} & \emph{\textbf{0.8273}} &
\emph{0.3583}\tabularnewline
& Longest Axis Length & \emph{0.4943} & \emph{\textbf{0.7055}} &
\emph{0.4073}\tabularnewline
Shape & Circular Compactness & 0.2758 & \emph{0.4203} &
0.0864\tabularnewline
& Shape Index & 0.2758 & \emph{0.4203} & 0.0864\tabularnewline
& Rectangularity & 0.2940 & \emph{0.4040} & 0.1214\tabularnewline
& Fractal Dimension & 0.2593 & \emph{0.4407} & 0.0360\tabularnewline
Spatial Distribution & Orientation & \textbf{0.6859} &
\emph{\textbf{0.7985}} & \textbf{0.5713}\tabularnewline
Intensity & Frequency & \emph{\textbf{0.7995}} & \emph{\textbf{0.9103}}
& \emph{\textbf{0.7093}}\tabularnewline
& Coverage Area Ratio & \textbf{0.6721} & \emph{\textbf{0.7649}} &
\textbf{0.5567}\tabularnewline
Diversity & Gini Index of Area & \textbf{0.6882} &
\emph{\textbf{0.7291}} & \textbf{0.6312}\tabularnewline
& Gini Index of CAR & \textbf{0.5963} & \textbf{0.6263} &
\textbf{0.5551}\tabularnewline
Connectivity & Reach & \emph{\textbf{0.8851}} & \emph{\textbf{0.9371}} &
\emph{\textbf{0.8282}}\tabularnewline
\bottomrule
\end{longtable}


##### Normalised RMSD
Overall, the RMSD test indicates a high level of similarity between datasets (figure \ref{fig:nrmsd} and Table 3), excluding *Dimension* characters which, as mentioned in Section 3.2 are heavily skewed by large outliers, hence not comparable with the rest of the data. Apart from *Orientation*, which is the worst-performing character in the set (~0.22 for the whole dataset, ~0.26 for multi-building plots and ~0.18 for single-building plots), all other characters score RMSD values lower than 0.2 (~0.15 for single-building plots and ~0.18 for multi-building plots). This suggests that, even though the spatial coverage of the morphological tessellation is different from plots, this difference is, in terms of information, only minor. Even the poorer performance of *Orientation* depends more on the way this is measured than on dissimilarity between datasets: unlike other metrics, *Orientation* is calculated as a deviation of the orientation of the longest axis of MBR from cardinal directions in degrees and, as such, it ranges from 0 to 45º. Hence, a deviation of 0.2 corresponds to a difference of only 9º.  It is worth noting that for smaller buffers (15 to 40m) results show high instability, where some characters exhibit the highest correlation values and others the lowest: this confirms that smaller buffers are unsuitable as parameters to limit the tessellation. In turn, the 100-metre buffer is confirmed as robust and stable across all characters.

![NRMSD of cadastral values and each of the selected buffers of tessellation based on the whole dataset (figures for single and multi-building plots are found in the Appendix XXX).](source/figures/ch6/nrmsd.pdf "NRMSD of cadastral and MT values"){#fig:nrmsd width=100%}

\begin{longtable}[]{@{}lllll@{}}
\caption{NRMSD for the whole dataset, single-building plots and multi-building plots at 100m buffer.} \label{tab:nrmsd_results} \\
\toprule
Category & Character & All &
Single & Multi\tabularnewline
\midrule
\endhead
Dimension & Area & 0.0213 & 0.0075 & 0.0326\tabularnewline
& Longest Axis Length & 0.0469 & 0.0162 & 0.0645\tabularnewline
Shape & Circular Compactness & 0.1545 & 0.1270 & 0.1788\tabularnewline
& Shape Index & 0.1252 & 0.1000 & 0.1479\tabularnewline
& Rectangularity & 0.1671 & 0.1563 & 0.1773\tabularnewline
& Fractal Dimension & 0.0754 & 0.0566 & 0.0970\tabularnewline
Spatial Distribution & Orientation & 0.2229 & 0.1775 &
0.2601\tabularnewline
Intensity & Frequency & 0.1862 & 0.1507 & 0.2163\tabularnewline
& Coverage Area Ratio & 0.0366 & 0.0432 & 0.1224\tabularnewline
Diversity & Gini Index of Area & 0.1618 & 0.1509 & 0.1724\tabularnewline
& Gini Index of CAR & 0.0752 & 0.0691 & 0.0838\tabularnewline
Connectivity & Reach & 0.1685 & 0.1528 & 0.1828\tabularnewline
\bottomrule
\end{longtable}

##### Recognition of significant patterns using LISA

![Example of LISA patterns of Frequency measured on the MT shows Moran Local Scatterplot LISA clusters and actual distribution of values.](source/figures/ch6/100_frequency.png "Example of LISA patterns of Frequency"){#fig:100_frequency width=100%}

The analysis of patterns with LISA (figure \ref{fig:100_frequency}) captures differences across measured characters; however, given the dissimilarity of the datasets due to multi-building plots, the accuracy scores are not expected to reach values close to 1. Highest pattern similarity is recognised for the *Frequency* character (~0.78, corresponding to an almost 80% match) (figure \ref{fig:accu}), followed by *Orientation* and *Diversity* characters (Gini Index of Area and Gini Index of CAR) and CAR (0.74 – 0.66), while *Dimension* characters are around ~0.5 depending on the sample considered (single- or multi-building plots). *Shape* characters are consistently the ones providing lowest accuracy, apart from *Reach Centrality*, due to the single-building vs. multi-building deviation in the datasets. Overall, the difference between samples is relatively consistent, with single-building plots reaching values between 0.1 and 0.2 higher than multi-building plots. While none of the values indicates an equality of both datasets, some are close enough to be considered as proxies of each other. The effect of buffer distance confirms already observed pattern and the stability of the 100m buffer.

![LISA accuracy of cadastral values and each of the selected buffers of tessellation based on the whole dataset  (figures for single and multi-building plots are found in the Appendix XXX).](source/figures/ch6/accu.pdf "LISA accuracy of cadastral and MT values"){#fig:accu width=100%}

\begin{longtable}[]{@{}lllll@{}}
\caption{aLISA for the whole dataset, single-building plots and multi-building plots at 100m buffer.} \label{tab:accu_results} \\
\toprule
Category & Character & All &
Single & Multi\tabularnewline
\midrule
\endhead
Dimension & Area & 0.5938 & 0.6447 & 0.5090\tabularnewline
& Longest Axis Length & 0.5181 & 0.6138 & 0.4028\tabularnewline
Shape & Circular Compactness & 0.4235 & 0.5061 & 0.3319\tabularnewline
& Shape Index & 0.4449 & 0.5312 & 0.3475\tabularnewline
& Rectangularity & 0.3330 & 0.3930 & 0.2761\tabularnewline
& Fractal Dimension & 0.4644 & 0.5652 & 0.3489\tabularnewline
Spatial Distribution & Orientation & 0.7389 & 0.8055 &
0.6711\tabularnewline
Intensity & Frequency & 0.7763 & 0.8240 & 0.7318\tabularnewline
& Coverage Area Ratio & 0.6610 & 0.7313 & 0.5908\tabularnewline
Diversity & Gini Index of Area & 0.7050 & 0.7333 & 0.6759\tabularnewline
& Gini Index of CAR & 0.6585 & 0.6742 & 0.6423\tabularnewline
Connectivity & Reach & 0.4007 & 0.3363 & 0.4644\tabularnewline
\bottomrule
\end{longtable}

### test tessellation contiguity as aggregation
_ISUF_
At the small scale, we studied how five urban types in Prague are represented by the four methods of aggregation. The Old Town, a tissue of a medieval origin which has grown organically, shows few differences between the four methods, with slightly larger footprints of aggregations defined by Euclidean distance and a morphological tessellation topology at both 200 (figure \ref{fig:200m}a) and 400 (figure \ref{fig:400m}a) metres distances.  Numerically, the difference is clear, but for pattern-detection this difference is not substantial, suggesting that all methods are relatively equal in this tissue for both 200 and 400 metres (and equivalents). Differences might be explained by the high granularity of the tissue, with many elements on a relatively small area (the reason for KNN being the smallest) and complex configuration amongst them (buildings have many neighbours, expressed by more extensive topological-based aggregation). 
  
![Comparison of boundaries of aggregations defined by each of the tested method for 4 topological steps and equivalents (200 metres, 70 neighbours). a) Old Town, b) Vinohrady, c) Hanspaulka, d) Jižní Město, e) Malešice](source/figures/ch6/200mmaps-01.png "Comparison of boundaries of aggregations for 4 topological steps"){#fig:200m width=100%}

In the second case, the urban tissue of 19^th^ century of compact perimeter blocks in the Vinohrady neighbourhood, results almost matches the previous case. Due to the high granularity of this urban tissue, purely Euclidean distance-based area is the largest, while K-nearest neighbour the smallest (figure \ref{fig:200m}b, figure \ref{fig:400m}b).

Overall, in these two historic tissues, the difference is not significant to conclude that one method is better than the other - simple visual comparison shows that boundaries almost overlaps for both tested distances.

The first crucial differences are noticeable in Hanspaulka, an area of 20^th^ century mixed single and multi-family villas, where the street network is becoming less dense and less connected than in the city centre, leading to the difference between the area captured by metric reach (smaller) and the other three methods, which almost overlap without any substantial distinction (figure \ref{fig:200m}c, figure \ref{fig:400m}c). This indicates that the street network plays a crucial role in the applicability of reach-based methods.

![Comparison of boundaries of aggregations defined by each of the tested method for 9 topological steps and equivalents (400 metres, 320 neighbours). a) Old Town, b) Vinohrady, c) Hanspaulka, d) Jižní Město, e) Malešice.](source/figures/ch6/400mmaps-01.png "Comparison of boundaries of aggregations for 9 topological steps"){#fig:400m width=100%}

The twentieth-century modernist housing of Jižní Město is the first example of a post-WW2 urban tissue. The planning ideology behind it comes with the radical change of scale and a distinctive approach to streets and their connectivity. This change is reflected in how each of our tested methods captures the space: while the area defined by Euclidean distance remains mostly the same as in pre-WW2 tissues, the area captured by metric reach shrinks due to the convoluted street network. In theory, both topological and KNN definitions of aggregation should be able to capture the difference in scale and up to a certain level they do. However, KNN, even though being larger than metric-based methods, lacks the ability to deal with large pavilion-like buildings with many direct neighbours, unlike the topological definition which correctly reacts to the abrupt change of scale of the granularity of urban tissue and captures the relationship between high-rise buildings and their low-rise pavilion counterparts by acknowledging that they are neighbouring (figure \ref{fig:200m}d, figure \ref{fig:400m}d).

Whilst industrial type tissues are generally not the concern of urban morphology, as classified as specialist and treated differently than more ordinary fabric, they are nonetheless large, therefore important parts of our cities and as such deserve to be studied using the same approach as the more conventional ones. Their scale is radically different. Buildings are of the size of the traditional block or larger, the plot structure is mostly unorganised, and the street network is utilitarian only, following different principles than in residential or mixed-use parts of the city.These differences are captured through the application of our four methods. The network-based method is unreliable on this tissue, capturing the only a minor area around the building due to the major drop in a granularity and connectivity. The Euclidean distance of 200 or 400 metres, which seems to capture enough information in more granular urban tissues lacks the same capacity in this case. K-nearest neighbour analysis struggles to capture the peculiarities of this particular urban tissue, which is characterized by a large amount of additional built-up structures to main buildings, leading to the identification of smaller area that make a comparison with the other cases confused. The topological definition achieved by the morphological tessellation seems to tackle all issues of the other methods, whilst capturing a similar amount of information as it did in previous cases (figure \ref{fig:200m}e, figure \ref{fig:400m}e).

Overall, the differences between methods in defining aggregation are heavily dependent on the type of urban tissue analysed. More traditional (from a European perspective) urban tissues like medieval (Old Town) or perimeter blocks (Vinohrady) indicate that in these contexts the choice of the method is purely the matter of opinion and that the resulting value offered by the four methods is mostly similar. However, once we start focusing on post-WW2 development, we often observe a change of scale of urban patterns, which makes distance-based methods (Euclidean, metric reach) unable to react to such change. The information captured is consequently different in pre- and post-WW2 urban tissues, complicating the further comparability, whilst we seek similar and consistent data. If the urban patterns change their scale, the method of capturing such extent needs to be able to adapt to it. Our results of the small-scale analysis indicate that topology of morphological tessellation is the method able to fulfil this condition adequately.
Whilst small scale analysis illustrated the capacity of the four selected methods to provide stable information, it is only at an urban scale, through statistical analysis, that we can show a full overview of how the four methods perform. 

As mentioned, neighbouring elements are bearing the primary information about urban patterns. For this reason, researchers aim to use methods capturing an equal number of neighbours across contexts. Such a method might be K-nearest neighbour, but due to the variety of urban configurations, a method needs a certain level of adaptability (which KNN with fixed number cannot provide). As figure \ref{fig:graphs_t}(a, b) shows, the statistical distribution of the number of neighbours captured is the most stable for topology of morphological tessellation, being almost perfect Gaussian distribution (the deviation in the number of neighbours is the same in both directions from the mean), with the smallest standard deviation ($\sigma$). The metric reach method to provides right-skewed distribution and Euclidean distance high deviation, which are both undesirable features in terms of stability of information.

Then, comparison of distributions of covered area aims to test the adaptability of each method. As mentioned, the changing scale of urban patterns means that the same level of information is spread to larger areas. Therefore, an ideal method should show high flexibility (the distribution of values should have large range and high standard deviation) in the area captured to fit all patterns possible. The results as shown in figure \ref{fig:graphs_t}(c, d) indicate that topology of morphological tessellation offers by a large margin the highest standard deviation out of tested methods, indicating that the change of the scale is captured successfully. Metric methods (Euclidean distance, metric reach) are the least flexible in this sense, while K-nearest neighbour might offer desired value alongside with morphological tessellation topology.

![Statistical distributions of number of neighbours a) 4 steps and equivalents, b) 9 steps; and total covered area c) 4 steps and equivalents, d) 9 steps.](source/figures/ch6/graphs_t.png "Statistical distributions of number of neighbours"){#fig:graphs_t width=100%}

Even though there are differences between smaller and larger distances (4 steps / 9 steps and its equivalents), topologically defined aggregation seems to reflect desired outcomes (i.e. stability in number of elements captured and flexibility in metric values) in both statistical comparisons better than other tested methods. This finding is in line with the one we drew from small-scale case studies, indicating that topology of morphological tessellation is a valuable approach to be employed in morphological analysis.

## Discussion
_Also mention block = Generating blocks appendix_
It is not complicated to find case studies offering the data in required quality and detail, but it is true that data of this level of precision are not available everywhere around the world. That is true, especially for building height parameters. Having all data, as outlined above, is the ideal situation, which will be tested in this research. In the real world, the situation might be less optimal than that, so pre-processing procedures have to be employed before performing the analysis itself. The case analysis using extremely sub-optimal data is available as Annexe X, outlining the work done on Grand Rapids, Michigan using building footprints not representing individual buildings and missing any height attributes.


### Teessellation in relation to plot

Our results suggest that the proposed method contributes to resolve some of the limitations associated with using the plot as unit of UMM analysis. However, the picture resulting from testing the similarity between cadastral plots and MCs is rather complex. 
Notably, the significance of similarity between plots and MCs varies considerably depending on the morphometric character selected: this is generally high for all Intensity characters (*Frequency, CAR*, whilst Shape characters (*Rectangularity, Circular Compactness, Shape Index*, and *Fractal Dimension*) report a comparatively poorer performance and a higher deviation. This means that if, for several of the morphometric characters assessed, MT is able to retain plot-level information which is comparable to that provided by the cadastral layer, for other characters MCs are less efficient proxies of plots and capture comparatively different information. 

It is also evident that the similarity of datasets is higher across all measured characters for single-building plots compared to multi-building plots. Considering that the former ones are predominantly found in pre-industrial urban tissues while the latter are more typical of modern and contemporary development, it is suggested that MT might be a *better proxy* of plots in the context of traditional fabrics than it is in modernist and contemporary ones.

Overall, there appears to be substantial scope for the MC to be utilised as basic unit of UMM analysis, given its ability to capture meaningful patterns of urban form at the plot scale, the degree of reliability and universality of the underlying method and the wide accessibility of the data required to generate it. Indeed, while the recognition of plots can be very troublesome and resource intensive, morphological tessellation is consistent throughout, since it is only based on building footprint information which is equally present in all kinds of urban areas. Moreover, by using morphological tessellation instead of traditional methods relying on buildings, street networks and plots, data dependency is reduced by a third as the tessellation is generated from the building layer alone. 

### Limits of morphological tessellation
Whilst MT and MC appear to be promising new addition to the tools available for UMM applications, a first limit of this work is that the cadastral parcels in Zurich, which we have loosely treated as ‘plots’, are solely based on land-ownership. That causes discrepancy between the generated tessellation and the cadastral layer which includes multi-building plots. However, as only 21% of plots are affected and results are reported for both groups, we believe that the presented method is robust enough to provide relevant results.

Second, whilst it is true that a MT can be generated directly from a building layer alone, it cannot be created from any building layer, as this needs to comply to certain quality requirements. Notably, since the method sees every feature of GIS layer as an individual input for tessellation, it is important not to have buildings composed of multiple features each representing, for example, different heights or different parts of the same (as in the case of British Ordnance Survey). Similarly, it is important not to have different independent buildings collapsed into a single simplified feature (as in the case of vast portions of Open Street Maps).

## Conclusions

_zurich_
Plots are commonly seen as the ideal spatial division for morphological analysis, but they also have their drawbacks, causing the limited applicability of plot-based methods and, more importantly, the reduced reliability of results obtained by employing them. The aim of this work is to address some of the issues characterising the definition of plot and plot boundaries, the availability and accessibility of plot data and the labour intensiveness of manually extracting reliable plot-level information, aspects that limit the potential of Urban Morphometrics. The need to objectively define a unit of analysis able to capture the smallest and arguably most fundamental level of spatial subdivision, and to develop a reliable and replicable method to generate and measure it, is the rationale behind the *Morphological Cell* (MC) unit and the *Morphological Tessellation* (MT) method. 

The universal and algorithmic nature of the proposed MT has the potential to scale up UMM analysis with minimum effort to the large scale , while significantly reducing the interpretative input of the analysts along the process. This latter property of MT appears to be particularly relevant to making large scale UMM analysis viable and take full advantage of big data in the GIS area. The robustness of the proposed method and the validity of the proposed spatial unit of analysis is verified through the assessment of 12 representative morphometric characters and the application of three different *quantitative* comparative methods, Spearman’s correlation, NRMSD and accuracy of LISA, aimed at evaluating the similarity of information between MCs and cadastral plots.  

The MT method, as tested and presented in this paper, offers a different approach to spatial division whilst still capturing a level of quality of information on urban form that is similar to that conveyed by the plot. Findings presented in this paper indicate that there is overlap between the information derived from cadastral plots and the one derived from morphological tessellation. The degree of this overlap depends on the category of morphometric characters and the type of urban context, but for certain types of morphologic analysis it is large enough to consider MCs reliable proxies of plots. At the same time, MCs cannot fully *replace* plots in the understanding and analysis of urban form patterns.

Existing location-based methods of aggregation of elements into larger analytical units all face some issues limiting their applicability and reliability. The alternative method presented is based on the topology of space as captured by the morphological tessellation. Such a method of partitioning space reflects the influence of each building on the space around it with the aim to overcome existing challenges and provide a context-sensitive method. Initial results of the twofold analysis of the topological ability of the morphological tessellation indicate that the type of urban tissue influences the outcome of morphological analysis, and that in the case of pre-WW2 traditional European-like urban tissues, all currently available methods of definition of aggregation are relevant and almost interchangeable. However, this is not the case with post-WW2 urban developments, as in them there has been a significant change in the scale of form’s granularity. In these cases, urban morphology needs to employ methods which are sensitive to the scale and configuration of urban form and at the same time can detect its granularity. The morphological tessellation and the topology derived from the analysis of its structure seem to be the most successful, sensitive method, suitable for general analysis.
All of the methods that have been tested partially solve one of the key issues identified in spatial analysis (MAUP), as data are aggregated independently for each element and there are no preselected boundaries in play.

No matter the results of presented analysis, methods extracted from literature have their role in morphological analysis. However, Euclidean definition and metric reach should be used in specific situations only, due to their abovementioned limitations. It is either in stable environments without abrupt changes of granularity or in a definition of larger-scale aggregations, where multiple urban tissues are included. In that case, the main benefits of the morphological tessellation — following the spatial configuration of urban patterns — is not so crucial and from certain scale does not even provide added value. 

For the analysis done on the small scale (scale of urban tissue and smaller), Euclidean definition and metric reach do not provide a stable information, unlike KNN (which always captures the same number of elements of similar informational value, but not the same relationship) and the topology of morphological tessellation. Moreover, aggregation defined via the topology of morphological tessellation may be used even on the smallest scales of one or two steps as it will always capture intended comparable information based on the relationship of elements.

Currently, tools to generate a morphological tessellation and work with its topological relations are available under a MIT license as a part of open source Python package named “momepy – Urban Morphology Measuring Toolkit”, which, together with its source code, is publicly available and is under active development.

Further research should focus on the question of the exact meaning and variation of topological distance and its definition for specific purposes. To date, the question of how many topological steps should be used for the analysis of urban form remains open. It is expected that it will vary depending on the scope of the research. 

The morphological tessellation is a step towards achieving consistency in urban morphology in both definitions of the smallest spatial unit and analytical aggregation. The advantage of morphological tessellation is that it limits the data dependency as it is based on building footprints only and allows the elimination of subjectivity in the partitioning of space. Most importantly, it is context sensitive allowing the researcher to use the same method across different types of urban tissues whilst still get comparable information, much needed for reliable results of any statistical analysis.

_as tessellation holds as a spatial unit, relational model will be used and tested in next chapters. keep going with the model to see if it holds in the actual work_
