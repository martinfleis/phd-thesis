\setcounter{chapter}{2}

\tableofcontents

# Numerical taxonomy

_link back_

_aim of the chapter_

_structure of the chapter_

## Learning from biology
*morphometrics and numerical taxonomy as two concepts which may allow overcoming issues identified in previous two chapters*
*this research aims to numerically describe urban form and classify it. Both these aims are in long term focus of biology, which uses morphometrics in description and numerical taxonomy in classification in the most advanced way. Even though current techniques like DNA sequencing bring better results, the whole concept of morphometrics and taxonomy is still valid, especially if we try to adapt it to urban form, where something like DNA sequencing is not possible.*
*biology did a lot of work setting the scene and we should learn from it to avoid reinventing the wheel where the key principles hold.*

### Morphometrics as a descriptive tool
*short introduction*
*the general definition of morphometrics is a quantitative analysis of form, i.e. size and shape (REF).*
*morphometrics is as a descriptive tool which has the ability to determine the level of resemblance of different individuals, either of the same species or of different species.*

*biology knows several morphometric methods, used for the similar purpose, each based on different principles*

- traditional morphometrics
*multivariate morphometrics. "refers to the application of multivariate statistics to linear measurements and ratios" *
*‌"Traditional morphometrics has been shown to have certain limitations when compared to geometric morphometrics. In the former, data consist of lengths, depths, and widths containing little information about the geometry of the structure being studied (Zelditch et al. 2004). Geometric relationships among the variables are not retained so that it is not possible to depict graphical representations of shape (Adams et al. 2004) In addition, overlap of variables occurs frequently, making it difficult to describe local shape changes. Within the traditional framework a formal distinction between size and shape is difficult, and little agreement is found among the many methods of size correction proposed (Klingenberg 1996, 1998; Zelditch et al. 2004).  https://academic.oup.com/jmammal/article/92/6/1395/961102"*
*"Traditional morphometrics is the study of morphological variations between or within groups using multivariate statistical tools. Shape is defined by collecting and analyzing length measurements, counts, ratios, and angles.[1][2][6] The statistical tools are able to quantify the covariation within and between samples. Some of the typical statistical tools used for traditional morphometrics are: principal components, factor analysis, canonical variate, and discriminant function analysis. It is also possible to study allometry, which is the observed change in shape when there is change in size. However, there are problems pertaining to size correction since linear distance is highly correlated with size. There have been multiple methods put forth to correct for this correlation, but these methods disagree and can end up with different results using the same dataset. Another problem is linear distances are not always defined by the same landmarks making it difficult to use for comparative purposes.[2] For shape analysis itself, which is the goal of morphometrics, the biggest downside to traditional morphometrics is that it does not capture the complete variation of shape in space, which is what the measurements are supposed to be based on.[2][6] For example, if one tried to compare the length and width for an oval and tear drop shape with the same dimensions they would be deemed as the same using traditional morphometrics.[2] Geometric morphometrics tries to correct these problems by capturing more variability in shape. https://en.wikipedia.org/wiki/Geometric_morphometrics_in_anthropology"*

- geometric morphometrics
*landmarks, semilandmarks, deformation grid*
*‌concerns the development of coordinate-based methods begun in the 1970s (Bookstein 1991; Dryden and Mardia 1998; Zelditch et al. 2004) https://academic.oup.com/jmammal/article/92/6/1395/961102"*
*"Geometric morphometrics methods capture the geometry of an object using coordinate-based data. A statistical theory of shape has been developed allowing “… the combined use of multivariate statistical methods and methods for the direct visualization in biological form” (Adams et al. 2004:6). https://academic.oup.com/jmammal/article/92/6/1395/961102"*

- outline analysis
*coefficients of mathematical functions are fitted to points sampled along the outline - link to Cooper and others*

- tissue morphometrics (Histomorphometry) and other fields, Neuroimaging, Geomorphometrics
==add some clear figures==

*these approaches and development can inform urban morphometrics*

### Numerical taxonomy as a classification tool
*classification system based on morphometric data and numerical methods of systematisation. "The grouping by numerical methods of taxonomic units into taxa on the basis of their character states."*
*developed by Sneath and Sokal*
*distinction between phenetics (form-based classification) and cladistics (evolutionary branching)*
"A basic attitude is strict **separation** of **phylogenetic** speculation from taxonomic procedure. ... The separation of overall similarity (phenetics) from evolutionary branching sequences (cladistics) is and important advance in taxonomic thinking." (p.9-10)
*part of computational phylogenetics*

#### Principles of numerical taxonomy
*base this on Sneath and Sokal*
*key principle is that the classification is operational and empirical ==explain==*
*"‌operationalism implies that statements and hypotheses about nature be subject to meaningful questions; that is, those that can be tested by observation and experiment." (p.17)*

Repeatability and objectivity as principal aims.

(Taken directly from SS p.5)

1. The greater the content of information in the taxa of a classification and the more characters on which it is based, the better a given classification will be.
2. A priori, every character is of equal weight in creating natural taxa.
3. Overall similarity between any two entities is a function of their individual similarities in each of the many characters in which they are being compared.
4. Distinct taxa can be recognised because correlations of characters differ in the groups of organisms under study.
5. Phylogenetics inferences can be made from the taxonomic structures of a group and from character correlations, given certain assumptions about evolutionary pathways and mechanisms.
6. Taxonomy is viewed and practiced as an empirical science.
7. Classifications are based on phenetic similarity.

In practice, there are four steps (again taken from SS p.5) ==make link between this and chapter 5 in chapter 5==

1. Organisms and characters are chosen and recorded.
2. The resemblances between organisms are calculated.
3. Taxa are based upon these resemblances.
4. Generalisations are made about the taxa (such as inferences about their phylogeny, choice of discriminatory characters, etc.) (Sneath and Sokal, p.5)

While the scope of this work is not to give a detailed overview of biological numerical taxonomy, there are four crucial concepts which needs to be understood before the application of numerical taxonomy to urban form - Operational Taxonomic Unit (OTU), taxonomic characters, taxonomic resemblance and taxonomic structure.

##### Operational Taxonomic Unit
"Preliminary selection of specimens; based on rather few characters.
This could be individuals, for establishing species, or species, for erecting higher taxa."
"The logical fundamental unit in a large majority of instances is the individual organism."
"At higher taxonomic levels representative specimens or averages of several individuals are employed for a taxon."
"Taxon will therefore be an individual (or an average) standing for a race, a species, a genus or even a higher ranked taxon.
Thus we shall employ taxonomic units of different categorical ranks as the entities to be grouped into more inclusive aggregates during classification.
Operational taxonomic units (OTU’s), which are the lowest ranking taxa employed in a given study.
To be totally consistent and rigorous, a taxonomic unit at any level should be based on individuals.
(Sneath and Sokal, p. 68-69)"


##### Taxonomic characters
*‌All kinds of characters are equally desirable: morphological, physiological, ethological, and sometimes even distributional ones.*
***Taxonomic character** - "a characteristics (or feature) of one kind of organism that will distinguish it from another kind; or any attribute of a member of a taxon by which it differs or may differ from a member of a different taxon"p.71*

*"Meaningful estimates of resemblance can be made once there is agreement on what characters are to be admitted as relevant in taxonomy.*
1. *Use all kinds of characters from all parts of the body and from all the stages of life cycle.*
2. *Use all characters varying within the group studied, not merely conventional diagnostic characters."*

*A systematic survey of all known characters, or the inclusion of all characters the investigator has been able to observe, should prevent bias.*

*Which characters should be chosen as a basis for estimating the similarity between OTU’s?*
1. *What biological factors do the characters represent?*
2. *Are all characters of equal value and information on providing evidence on phenetic similarity?*

*Numerical taxonomy measures similarity between the **phenomes** of OTU’s.* 
***Phenome** - the total phenetic manifestations of the genome of an organism or a taxon.*
*Cities are defined by phenotype, not genotype.*
*Characters should be distributed as widely and evenly as possible over the organisms studied.*

*Take as many characters as is feasible and distribute them as widely as is possible over the various body regions, life history stages, tissues, and levels of organisation of organisms.*

***Equal weighting** is desirable.*

*Before we can apply clustering, values has to be scaled to bear the equal weights in clustering. This scaling might be even  logarithmic*

*Effect of environment*

*The environment affects the phenotype*
*We wish to separate environmental effects on the size from the effects on the shape.*
*The phenotypic responses form a multidimensional response system*
*Is a difference along the main street, like a presence of active frontage, just a response of phenotype to environment?*

##### Taxonomic resemblance and structure

*Taxa are constructed through various techniques designed to disclose and summarise the structure of resemblance matrix (p.6)*
*Numerical methods are collectively called **cluster analysis** - methods for establishing and defining clusters of mutually similar entities from the resemblance matrix.*
*The cluster are generally based on phenetic resemblances only and have no necessary phyletic connotations.*
*These methods permit the elimination of taxonomic groups in an **objective manner**, given a matrix of coefficients relationships.*

*distribution of taxa in phenetic space*
*clusters*

**mixture problem** - *when taxonomist assumes that sampled populations consist of a mixture that he first wishes to decompose into separate populations, which are then investigated further or are used as OTU's* ==link to chapter7. This is underlying theory.==

*hierarchical clustering leading to the dendrograms*

### Criticism of morphometrics and numerical taxonomy
"**Four major problems** of phenetic classification:
1. Incongruence between classifications based on different parts of the body or different life history stages
2. Differences in estimates of relationships produced by different similarity coefficients.
3. Differences in interpreting relationships produced by different clustering methods
4. The possible effect of parallelism and convergence on taxonomic judgements based on estimates of phenetic relationships."

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
