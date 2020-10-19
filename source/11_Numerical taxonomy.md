\setcounter{chapter}{2}

\tableofcontents

# Numerical taxonomy

_link back_

_aim of the chapter_

_structure of the chapter_

## Learning from biology
From a conceptual point of view, this research builds on the previous of @dibble2017 (parts also published as @dibble2015 and dibble2016), which established the theory of urban morphometrics and made the first link between numerical taxonomy - a classification method used in primarily in biology - and urban morphology. Both morphometrics and numerical taxonomy have a long and rich history outside urban sciences and the core idea behind the Dibble's work, which is also applied to this research, is that urban form can be in its own way perceived as group of individual entities which can be consistently measured and numerically classified. In @dibble2017 authors demonstrated that the idea is viable and that the potential of urban morphometrics should be explored further.

Researcher is biology did a lot of work setting the scene for morphometrics and we should learn from it to avoid reinventing the wheel, where the key principles hold.

### Morphometrics as a descriptive tool
Very generally speaking, morphometrics is a quantitative analysis of form, i.e. size and shape REF. In biology that usually refers to a size and shape of an individual, in which case morphometrics, as a descriptive tool has the ability to determine the level of resemblance of different individuals, either of the same species or of different species REF. Literature knows several branches of morphometrics, all conceptually similar, used for the similar purposes but based on different principles of what to measure and how. The two main approaches are traditional and geometric morphometrics.

Traditional or multivariate morphometrics is based on "the application of multivariate statistical methods to sets of variables" [@rohlf1993, p.129]. The variables used within the analysis normally represent widths, lengths and angles of features or distances between specific landmarks [@rohlf1993], hence containing little information about the actual geometry if the structure (REF Zelditch et al. 2004). The recreation of the original shape is not possible based on the used set of variables (REF Adams et al. 2004). Among the statistical techniques used within traditional morphometrics @rohlf1993 list principal component analysis, discriminant functions of canonical variate analysis. An example of measurements used within traditional morphometrics are shown on figure \ref{fig:morphom_fish}.

![Example of the application of multivariate morphometrics. Overview of different morphometric measurements investigated in S.panijus (Siddik et al., 2016)](source/figures/ch4/morphom_fish.png "Example of the application of multivariate morphometrics"){#fig:morphom_fish width=75%}

The typical application of traditional morphometrics is *allometry*, the study of change of the shape with the change of the size. However, in biology, this method has certain limitation mostly related to the normalisation of the shape values affected by size [@breno2011].

The second major branch of morphometrics, which tries to overcome some limitations of the previous one is geometric morphometrics  [@rohlf1993], which focuses on the position of landmarks and semi-landmarks on the grid and its deformation (figure \ref{}). The description of both size and shape is though the series of coordinates either on 2D plane or in 3D space. 

![Example of the application of geometric morphometrics. Locations of the landmarks on a dorsal view of the skull and the relevant distortion of the grid.](source/figures/ch4/geom.png "Example of the application of geometric morphometrics"){#fig:morphom_fish width=75%}

Geometric morphometric is heavily dependent on the shared landmarks features between individual in a study. Hence its possible application in urban context is difficult due to the complexity of urban form and the variety of patterns, making the definition of such shared landmark features very limited.

Similar to geometric morphometric is an outline analysis, which is trying to fit mathematical functions to points sampled along the outline of the studies shape, an approach which has already been applied in urban morphology either to study the shape of settlements [@batty1987] or different aspects of street scape [@cooper2003; @cooper2005]. Furthermore, there are other branches of morphometrics (tissue morphometrics [@bodenstein1987growth], geomorphometrics [@coblentz2014quantitative], neuroimaging [@wang1994morphometric]) which are applying the same principles in their respective fields.

All these approaches and methods can inform the development of *urban* morphometrics.

### Numerical taxonomy as a classification tool \label{taxonomy_tool}
*classification system based on morphometric data and numerical methods of systematisation. "The grouping by numerical methods of taxonomic units into taxa on the basis of their character states."*
*developed by Sneath and Sokal*
*distinction between phenetics (form-based classification) and cladistics (evolutionary branching)*
"A basic attitude is strict **separation** of **phylogenetic** speculation from taxonomic procedure. ... The separation of overall similarity (phenetics) from evolutionary branching sequences (cladistics) is and important advance in taxonomic thinking." (p.9-10)
*part of computational phylogenetics*

One of the specific application of morphometric is the usage of measurements in classification of species, for which @sneath1973 use the term *numerical taxonomy* and define it as "*the grouping by numerical methods of taxonomic units into taxa on the basis of their character states*" [@sneath1973, p.XXX]. In biology, this requires a distinction between *phenetics* (overall similarity) and *cladistics* (evolutionary branching sequence).

The key principle of numerical taxonomy is that it is a classification which is operational and empirical. As further explained by @sneath1973, "*operationalism implies that statements and hypotheses about nature be subject to meaningful questions; that is, those that can be tested by observation and experiment (p.17)*". That further assumes that numerical taxonomy as a method has a potential to be reproducible and replicable.

@sneath1973 define seven key principles of numerical taxonomy:

1. *The greater the content of information in the taxa of a classification and the more characters on which it is based, the better a given classification will be.*

Selection of morphometric characters which is used for classification is inherently biased. To limit such a bias as much as possible, we should employ as large number of characters as is possible (and meaningful) as long as it does not violate any other rule.

2. *A priori, every character is of equal weight in creating natural taxa.‌* 

Some of the classification models apply weighting, which means that character A is seen as more important than character B. However, this decision often introduces bias into the selection because the rules defining the weighting are often arbitrary. Furthermore, we do not a priori know which character will have the highest discriminatory power.

3. *Overall similarity between any two entities is a function of their individual similarities in each of the many characters in which they are being compared.*

In other words, when measuring similarity between two entities, all characters needs to be taken into account.

4. *Distinct taxa can be recognised because correlations of characters differ in the groups of organisms under study.*

Taxa, i.e. classes of numerical taxonomy, represent different groups of organisms or other entities under scrutiny. The relations between morphometric values within such taxa are different than relations to other taxa.

5. *Phylogenetic inferences can be made from the taxonomic structures of a group and from character correlations, given certain assumptions about evolutionary pathways and mechanisms.*

Phenetic information used to build a taxonomy is not able to reflect phylogeny entirely, but the difference between the true evolutionary development of species and that observed in phenetic taxonomy is often minimal. In an urban environment, that means that we might be able to, to a degree, trace historical origin in numerical taxonomy of urban form. 

6. *Taxonomy is viewed and practiced as an empirical science.*

Conceptual assumptions about observations should have no role in the taxonomy.

7. *Classifications are based on phenetic similarity.*

Phenetic similarity represented by the relations (e.g. correlation) between morphometric characters is the only aspect taken into account when building a classification.

While the scope of this work is not to give a detailed overview of biological numerical taxonomy, there are four crucial concepts which needs to be understood before the application of numerical taxonomy to urban form - Operational Taxonomic Unit (OTU), taxonomic characters, taxonomic resemblance and taxonomic structure.

##### Operational Taxonomic Unit
OTU is the lowest ranking taxa employed in a given study. In biology that is usually species representing by an individual (e.g. a single bird specimen). In some cases  OTUs can be species if the aim is to develop higher order taxa or other entities. Generally, OTU should be the fundamental unit in a large majority of instances. To ensure consistency and rigour, @sneath1973 suggest that in the case of biology, *"a taxonomic unit at any level should be based on individuals." (p.69)* Naturally, urban form does not offer a simple definition of individual and the question of optimal OTU needs to be studied.

##### Taxonomic characters
Taxonomic character are in essence morphometric character used to derive numerical taxonomy. For the use in biology, it can be defined as "*a characteristics (or feature) of one kind of organism that will distinguish it from another kind; or any attribute of a member of a taxon by which it differs or may differ from a member of a different taxon*" [@sneath1973, p.71] For application on urban form, the term *organism* will refer to a set OTU.

The critical step in the design of numerical taxonomy is the selection of taxonomic characters. The set of characters which is used can significantly affect the results of the analysis, therefore an extensive set of rules of selection should be defined and followed. The general principle should be driven by inclusivity - all available kinds of characters should be used. Furthermore, all characters which may bring a new information should be employed, the set should not follow a limited set of conventionally used analytical variables. The advice given by @sneath1973 says *"take as many characters as is feasible and distribute them as widely as is possible over the various body regions, life history stages, tissues, and levels of organisation of organisms" (p. XXX)* - again, the terminology refers to biology, but the principle should be translated to urban morphology. 

##### Taxonomic resemblance and structure
Taxonomic resemblance, the similarity between OTUs, is determined using cluster analysis based on the resemblance matrix. Resemblance matrix consists of all morphometric values and all OTUs in the study. As a results, clusters, i.e. higher order taxa, are based on phenetic resemblances in an objective manner. 

The optimal interpretable outcome of numerical taxonomy is a hierarchical dendrogram merging lower order taxa into the higher order (fig. \ref{fig:dendrogram}). However, the methods of cluster analysis vary, even thought the tendency is to employ hierarchical methods. \footnote{That does not necessarily mean that flat clustering methods like K-means are not used. Although if the final output should be captured in a dendrogram, single layer of K-means clustering is not enough and other steps should be introduced.}

![Example of dendroram using Ward’s method classification of 39 species of Mallomonas. (Feng and Xie, 2013)](source/figures/ch4/dendrogram.jpg "Example of dendroram using Ward’s method classification of 39 species of Mallomonas."){#fig:dendrogram width=50%}

Of a high relevance for urban form is a *mixture problem*. That happens "*when taxonomist assumes that sampled populations consist of a mixture that he first wishes to decompose into separate populations, which are then investigated further or are used as OTU's*" [@sneath1973, p.XXX]. If the OTU in place will be an aggregation was Sanctuary area in case of @dibble2017 or urban tissue, the sample may be composed of individual buildings which need to be first assigned into their respective SA/tissue. In that case, the OTU for taxonomy itself will be the *population of buildings* composing a morphological aggregation. ==link to chapter7. This is underlying theory.==


### Criticism of morphometrics and numerical taxonomy
*"**Four major problems** of phenetic classification:*
1. *Incongruence between classifications based on different parts of the body or different life history stages*
2. *Differences in estimates of relationships produced by different similarity coefficients.*
3. *Differences in interpreting relationships produced by different clustering methods*
4. *The possible effect of parallelism and convergence on taxonomic judgements based on estimates of phenetic relationships."*

*phyletic vs phenetic taxonomy*
*whether a chosen sample of characters is sufficient p.423*

## Transferability of concepts into urban morphology

### Review of principles and their applicability
#### Morphometrics
==once written, match the key concepts==

#### Taxonomy
==once written, match the key concepts==


##### Principles
###### Operational Taxonomic Unit
*OTU could be …*
*direct link to chapter 2*

*Generally, OTU for taxonomy on the level of specimen is individual. We face the problem defining what is individual in cities. One may argue, that SA, but as we can see from the example above, it is at least very problematic. If we try to define an individual we’ll find following:*
* *a single person or thing, especially when compared to the group or set to which they belong (Cambridge Dictionary)*
* *a single organism capable of independent existence. (Bilogical from Dictionary.com)*
* *a member of a compound organism or colony. (Biological from Dictionary.com)*
* *a particular being or thing as distinguished from a class, species, or collection (Merriam-Webster)*
* *a single organism as distinguished from a group (Merriam-Webster)*
* *a single, separate organism (animal or plant) distinguished from others of a same kind. (Biology-online.org)*

*The fact that settlements can grow from one building, and are composed of buildings as (one of) fundamental elements (Moudon, 1997) leads me to the idea of building being an individual in the city. Therefore, taxonomy of urban form is not examining the lowest taxa (buildings), but higher ranks. It means that we should look at it in a similar way as biologists are looking at taxonomy at the level of population (put aside the fact that population in the case of cities still needs to be defined) or species level (rather than individual level forming species).*

*Problem of species definition*
* *Phenetic species - a taxonomic species based on morphologically similar populations located in a definite geographic area and morphologically distinct from other populations assigned to different species. Such a species is essentially a phenetic one.*
* *Biological species - groups of actually interbreeding populations which are reproductively isolated from other such groups; a community of cross-fertilising individuals linked together by bonds of mating and isolated reproductively from other species by barriers to mating.*
	* *All of them are based on potential of interbreeding, a concept which is scientifically non-transferable to cities. The imitation doesn’t seem to be analogical enough.*
	* *Moreover, those concepts are in practice nonoperational.*
*The desirable fundamental taxonomic unit for taxonomy at the level of population would seem to be the phenetic species. (Sneath and Sokal, p.365)*

*Phenetic definition can result from two alternatives.*
*Species is*
1. *The smallest (most homogenous) cluster that can be recognised upon some given criterion as being distinct from other clusters*
2. *a phenetic group of a given diversity somewhat below subgenus category, whether or not it contains distinct sub-clusters*
* ***it indicates the smallest distinct kind***
*The worker who wishes to employ numerical taxonomic methods at population level will be inclined to use the first alternative (smallest distinct homogenous cluster) when sampling OTU’s to be employed in the study.*

*Isn’t the taxonomical study of urban form actually analogy to taxonomy at population level? Aren’t cities populations of buildings as individuals? Therefore, the OTU for taxonomy of urban form should be the smallest distinct homogenous cluster.*

*So, what should be used as OTU? It’s currently under investigation, but at this moment I propose use of the **smallest distinct physiognomically homogenous cluster (DHC)**. In short, DHC is formed by clustering method based on measurable characteristics.*

*SA's Jacob used are basically DHC's as well, due to their homogeneity.*

###### Taxonomic characters
*direct link to chapter 3*
==make link from chapters 7 and 8==

*as shown in the previous chapter, there is a wide range of potential for morphometric characters*
*their nature is different, but the essence is the same*
*the key homologous characters need to be found etc.*

###### Taxonomic resemblance and structure
*==pick methods from literature ch2==*

*determination of resemblance have been done before, even in the structural way (dibble, Serra)*
*none very methodological and widely applicable though, all have some issues.*


### Critical assessment of preceding work

*Proposed further research*
- case study expansion
	- he wanted more SA's I argue that it needs to be able to analyse whole fabric
- metrics expansion
	- completely agree
- challenging SA

#### Sanctuary area as OTU
*non-homogeneity of SA*
*Why Sanctuary Area is not OTU?*

*The existing approach of using Sanctuary Areas as an OTU is not viable. The SAs used in previous research were ideal cases, but cities are not composed on these ideal cases. The principal task of the systematics should be to recognise what are cities composed of, different characters, different urban forms. In the case of non-homogenous SA, which is substantial portion of SAs, the results would be misleading. The widely accepted fundamental elements of urban form are plots, block, streets (+ open spaces). Then why should we pretend that there is nothing below the level of SA?*

*Look at the example below. It’s a case of small town composed of few SAs. Thy hypothesis is, that it’s composed of several classes, as shown on figure below (the identification is currently purely perceptional, non-objective, but at the same time I’d say valid). In case of using SAs as an OTU, the distinction between different urban forms within this town would be impossible as these SAs are far from homogeneity. The problem with SAs is that their definition and identification is phylogenic process, its based on the process of development of settlement. The rest of the process is, however, the systematisation is based on purely phenetic attributes.*

*Therefore, I argue that Sanctuary Area doesn’t fit into the definition of an OTU ( [Taxonomic Evidence](evernote:///view/4164843/s38/cff90452-ea48-4c15-8f69-9a3d92fa274d/cff90452-ea48-4c15-8f69-9a3d92fa274d/) ), because an OTU is not taxa on any level of systematisation, and shouldn’t be used for general analysis outside safe selection of the best examples. In some cases, however, SA can be used as a validation of different method.*

*Use of SA as OTU assumes that whole cities are in fact ideal according to ‘Emergent Neighbourhood Model’ (Mehaffy et al). Even the authors states that they are not (e.g. the three pathologies). While the concept of SA in this model perfectly works, in case of taxonomy it doesn’t.*

#### Selection of taxonomic characters
*collinearity of characters*

*There is no assessment of collinearity of characters.*

#### Limitation of the model
*missing some aspects*
*hierarchical model of urban form based on SA is ignoring some aspects of urban form and hence could not be seen as comprehensive by default.*


### Unresolved questions
- OTU
*we do not know what the optimal OTU should be*
*define key characteristics of such optimal OTU*

- model
*we do not have comprehensive model of urban form*
*define key characteristics of such a model*

- characters
*we do not know what should be measured*

*"There are as yet no criteria for any absolute measure of taxonomic rank. We do not know how to decide whether a family of birds, for example, is equivalent phonetically to a family of insects." For cities, there should be independent taxonomic ranks. Origin of taxa is too different to use same.*


## Conclusions
