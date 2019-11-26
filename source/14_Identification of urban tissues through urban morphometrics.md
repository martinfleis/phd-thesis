# Identification of urban tissues through urban morphometrics

~~* Scales~~
~~* Measurable elements~~
~~* Characters~~
~~* Measuring framework~~
~~* Test~~
~~* Validation~~

## What needs to be captured 190110
To identify urban tissue within urban fabric we have to capture complex description of each tissue. It has to be inclusive in terms of scales, because city is composed of nested complexities as well as categories of characters. [bullshit]

###### Strategy for character selection
Set of taxonomic characters should:

1a. **Capture structural complexity by covering all categories of characters**
	- dimensions
	- shapes
	- spatial distributions
	- intensity
	- connectivity
	- diversity
1b. **Across all fundamental elements**
	- building
	- street
	- cell
2. **Capture scalar complexity by covering all topological scales**
	- single/small
	- medium
	- large
	- extralarge

I. To fulfil these conditions, we have to first **define subsets as combinations of all three rules listed above**.
II. Then we have to **identify characters for each subset** by following selection process:

1. **Extract all characters found in literature** (477 in total). This database worked as the main source of taxonomic characters. Due to its extent, it is expected that the majority of possible characters is included.
2. **Select those characters using data intended to be used within each subset** . ~~Large portion of characters identified in the first steps is using data sources which are not widely available. Because this research is aiming to be as universal as possible, it is using only two data layers. The characters relying on other inputs were excluded from the selection.~~
3. **Adapt characters to fit the framework** Some characters needs to be adapted to fit the framework, mostly as a translation of alto-based characters into cell-based and metric-based into topology-based.
4. **Eliminate logical correlations** (full correlations as well as partial, where possible). Logically correlated characters should be omitted, otherwise the feature which is causing the correlation would distort the resulting taxonomy and clustering. Fully correlated characters (in terms of causality) have to be excluded and only one should be kept, partial logical correlations should be limited, but in case of urban form, we are not able to fully avoid them.
5. **Eliminate ineffective characters** (axial maps, topological skeleton). Due to the nature of the analysis, working with large-scale data or even big data in some cases, the process of measuring has to be computationally effective. Some of the characters are not easily measurable, and it has to be evaluated whether the value of the characters would balance the difficulty of coding and / or computational demand. 
6. **Add characters where are clear gaps** (diversity, plot-level Voronoi cell). Because I am using Voronoi cells the smallest scale spatial unit in a scope previously unused, there is a range of characters which had to be adapted from original plot-based to cell-based. The database of characters also showed imbalance of different categories and gaps in the measuring of diversity. New taxonomic characters have to be implemented to cover those gaps and provide coherent description of urban form. This part of the research is still ongoing.
7. **Exclude invariant characters**. Some characters might be invariant over the entire sample of OTU's. Those should not be included as they are not bearing any taxonomic value. However, this exclusion is an ongoing process, because it depends on actual measured values.
8. **Limit empirical correlation*** When we have the evidence that more than one factor affects two correlated characters within a study, regardless of whether this evidence comes from within study or from outside, we would include both characters; otherwise we would employ only one. We assume that at least some independent sources of the variation in any empirical correlation, unless we have reason to believe otherwise.
9. **Exclude characters which does not have the ability to capture patterns**. Test capability of each character to capture spatial patterns by measuring spatial autocorrelation. Those without sufficient level of autocorrelation should be excluded as they do not bear any value in the process of identification of DHC.
10. **Balance scalarity and uniqueness of values**. The set of taxonomic characters has to be balanced regarding the scale as well as *uniqueness* of values. Some of the initially identified characters are possible to measure on different scales (street, block, vicinity). Due to the logical correlations between them, only one has to be used. The selection is trying to use the most appropriate in terms of the meaning of the character (which might be more suitable to street edge than block of vicinity for example). It also aims to limit the characters with limited uniqueness of values. Because the values are always stored on the smallest scale, the values of characters measured on the block scale are shared among all elements in the block. The intention is to limit those characters to minimum.

(Based on Sneath and Sokal, 1973)

###### Notes based on Jacob’s thesis 190117
He stated “These characters of urban form, at this point, are only hypothesised to be valid. Although certain characters utilised in this Methodology are quite simple and relate to non-abstract concepts, such as area and length, there is no preconception of the relative importance of the characteristics of urban form.“
- lets make a general test of reliability of characters via spatial autocorrelation. Characters are valid and valuable when they capture some patterns, hence spatial autocorrelation has to be present. It can work as a validation (of capability not completeness) of set of characters.

###### Scales for categorisation of characters for definition of DHC
Scales are selected to capture characters of urban tissues on all relevant levels of complexity. At the same time, it is trying to be as compatible with MoRE as possible, but naturally it is not the same. I am not using Sanctuary Areas or any other qualitatively stated characters (street hierarchy). 


**Plot**
Scale of a plot as the smallest element of urban form covers characters deductible from a single plot, building (or buildings) on the plot and their interrelations.

###### Plot
- In urban morphology, plot is usually seen as one of the fundamental elements of urban form.(Moudon 1997, Kropf) However, its definition and employability in the analysis is far from ideal as Kropf 2018 identified. 
- Cadaster is not equal to morphological plots
- Physical boundaries are not always present
- There is no data source which could be used in algorithmically quantitative analysis
- The level of plot is still the important one, so there must be another solution how to capture the smallest scale
- While Schirmer and Axhausen propose what they call 'influence zone' defined by topological skeleton of unbuilt space, Hamaina et al (2012, 2014) use Voronoi tessellation. Both approaches are giving very similar results, but I believe that Voronoi tessellation is algorithmically easier to achieve. 
- Voronoi cell can be used as a substitute of plot in some cases like covered area ratio and similar. The hypothesis states, that characters based on Voronoi cells generated from building footprints have similar information values as characters based on plots. However, it is practically impossible to test this hypothesis. (There would be option to use Gorbals and compare, because Ale have plots in Gorbals)

**Street** (Edge, Frontage) (Plot series?)
Minimal set of plots forming coherent structure. Characters can be based on one street edge or a street itself (composed of 2 street edges facing each other). What about the situations where it is complicated to identify street edge? Like modernist structures. This scale expects to have some king of frontage, or plots series present. There could be cases where street edge (plot series) will be the same as the block. How to resolve this situation? Use the same value for both? Might be the solution.

**Block** 
Enclosed group of street edges (plots) forms block. Characters are capturing values reflecting attributes of blocks as structural units of urban form. Definition of block is not easy, Conzen, as well as Cannigia, didn’t use it. There are some reasons, but Kropf (2014) is proposing some solutions. Definition just by streets is simplistic, figure ground pattern deny its structural connections to urban tissue.

**Vicinity**
Literature usually use the term neighbourhood for scale larger than block, however the definition of neighbourhood is unclear especially in terms of its physical structure. Therefore, it is usually used fixed euclidean or walking distance to simulate the neighbourhood scale (Song and Knaap, 2007; Schirmer and Axhausen, 2015; Song et al., 2013). In our case, term vicinity is used to avoid misunderstanding. The exact distances (either euclidean or walking) will be investigated later, but it is expected something like 400m, (which also reflects the usual size of SA). Kropf (2017) uses term urban tissue on this scale, but it doesn’t make sense to use this term while trying to identify urban tissues :). Moreover, tissues defined as DHC might have quite variable size. 
*Modifiable Areal Unit Problem*
"The buffer definition does not avoid the Modifiable Areal Unit Problem (MAUP) but it enables us to focus on the neighbourhoods around newly developed single-family parcels, which are most consistent with individual behaviour (Handy, 2004), and makes it possible to compute the following unique measures for each of the 6788 single-family houses. There are other limitations of using buffers, particularly for parcels located near the edge of residential subdivision and parcels near natural barriers. The 1/4-mile radius method could potentially include a large amount of surrounding land of different characteristics. However, as the intention is to capture features of each house’s immediate neighbourhood, it is thus only claimed that the buffer is a convenient unit of analysis and illustrates the effects the study sought to capture.
“ (Song and Knaap, 2007)

   
    400 metres radius (Alterations in scale, Urban Nuclei, Neighbourhood unit- UDSU) - seems to be working even for street network analysis (local)
    400 - 600 metres radius (Towards an urban renaissance - Task Force)
    
    Schirmer and Axhausen use 300 metres radius and then approx 1km reachable area
    
Let’s use 400m at the moment and if needed adapt later according to characters. Question is whether use only one radius or whether use more (for different characters, otherwise there should be dependency).

180919
There should be also sub-chapter discussing the use of topology based distance and euclidean. (Kane and Kim 2018, Van Eggermond and Erath 2015)

Topology based method is trying to simulate walkability, e.g. how many destinations (and their characters) can be reached within certain distance. It is a question, whether walkability based area of vicinity is the one we are aiming for. It is rather scale attempting to capture the immediate context of the area no matter the street network, which is measured separately. In case of topology based characters, we might find that the results are heavily affected by the connectivity of network which might skew the results. Moreover, topology based characters capturing 'accessibility of buildings and floorspace' are specificied individually. Topology is useful in modelling a journey from A to B, less for capturing the context of of the element.

**Urban area**
The aim is to identify urban tissues, so the scale of settlement might seem strange, but it should be used for street network analysis (at least). The results of this kind of assessment is granular to the level of street, so the results are effectively usable on smaller scale.
Def.: an aggregation or continuous network of urban communities (Merriam-Webster)

There is a question whether measures on sub-metropolitan scale (e.g. district) should be used, probably in the same form of fixed distance as locality. It will be further investigated. 

While thinking about those scales, it is important to understand that all values from all characters no matter the scale will be assigned to plot/building and all the clustering etc will be conducted on this smallest scale.


**181203** Every element has inherent relation to elements of other type. There is always relation *building-cell-street-block*. As such, characters using building-cell relation are using topological distance 0, because the relation is always present

###### Cross-scale measuring system / explanation
* Measuring will cover relevant scales, to capture different levels of complexity of urban form
* Values from measuring will be stored at the plot level, no matter the original measuring scale
* Different scales have different methods of measuring affecting the uniqueness of values derived for each plot (illustrated in the figure below - each colour represents unique value and shows how plots share them).

###### Selection of taxonomic characters
- 'characters should be distributed as widely and evenly as possible over the organism studied. Colles (1969c) advocates a deliberate policy of stratified sampling from various organs' (Sneath and Sokal,p.103)
- 'A systematic survey of all known characters, or the inclusion of all characters the investigator has been able to observe, should prevent bias of this sort.'(SS, 96) [bias in choosing the characters]
- there is no real benchmark assessing the selection of characters. Theory say, that if you include all possible characters, it should be okay. (Kinda weak I must say)
- the aim is to cover relevant scales as well as different aspects of complexity of form
- characters are identified across 5 scales (plot, street, block, vicinity, urban area)
- characters are identified across 6 categories (dimension, shape, distribution, intensity, connectivity, diversity)
- the base for the selection is content analysis s presented in chapter 03. It generated list of almost 500 characters used in previous studies, but naturally a lot of them are overlapping or using different sets of data than I intend to. 
- the database of existing research was then used to select appropriate set using only basic elements of form without any information on hierarchy or uses.
- it generated around 260 unique characters
- some of the characters were logically or partially logically correlated, hence were omitted. Also the characters describing most of the simple dimensions of derived elements were left out and used only as an input for more complex characters.
- further omission of characters was lead by the intention to eliminate possible doubling - if one use same metric for street and then block level, there is clear and relatively strong partial logical correlation, so following the principle of applying more fine grained data the smaller scale will stay and character on higher will go. 
- approximately half of the characters were excluded due to some logical correlations or based on existing research assessing the quality of characters (e.g. shape indicators)
- existing database was not well balanced, for example characters capturing diversity were in only few examples

###### Shape
- I have identified high number of characters assessing the shape of the object, but applying them all would shew the results towards shape itself.
- Some of them are correlated, then only one was applied
- some of them are designed to capture complexity. In that case, selection is based on Basaraner and Centinkaya (2017) who assessed shape complexity characters.
- characters based on topological skeleton and centreline (Schirmer and Axhausen, 2015) are omitted for two reasons - it is expected that their input is already covered by another characters and it is algorithmically complicated (REF)

###### Diversity
- new characters capturing diversity has to be introduced
- Dibble was using statistical values (min, max, stdev...) to capture diversity within the subsets. But the applicability is limited, therefore it is better to use more complex calculations focusing directly on diversity
- the most frequently used measurement of diversity is Simpson's diversity index, but it has one major drawback. It is necessary to identify all subsets of character before calculation. It means, for example, that to measure Simspon's index of plot size, one first have to come up with categories of those sizes and those will necessarily be arbitrary and specific for each case (as in Bobkova 2017). I argue that while most of the characters are linear values, categorising them means loosing the information and adding unnecessary bias into the dataset.
- I am proposing the use of Gini coefficient as a measurement of difference between equal and real (statistical) distribution. Gini index in urban morphology was used by Thai 2005 and power law distribution (which can be captured by Gini) by Louf and Barthelemy 2014 as well as Salat 2017, Gielen (2017)(index of concentration) and Feliciotti (2018).
- Another approach proposed again Tsai 2005 and later Caruso, Hilal and Thomas (2017). That is use of Local index of spatial autocorrelation (LISA). In my case, Local Moran's I or Geary's C autocorrelation coefficient are in fact capturing homogeneity of distribution of values, capturing *homogeneity in heterogeneity* - if the locality is heterogeneous in its key values, the LISA-based character will remain similar across the area and allow us to identify this heterogeneity as typical description of that locality and therefore identify it as DHC. 
- Both Gini and LISA are employed in previously unused range (X and X characters).
- LISA
	- "Moran’s index is somewhat equivalent to Geary’s coefficient and they can be substituted for one another. However, in practice, Moran’s index cannot be replaced by Geary’s coefficient and vice versa due to a subtle difference of statistical treatment. Compared with Geary’s coefficient, Moran’s index is more significant to spatial analysis." (Chen 2013 p. 2)
	- Let's work with Local Moran's I

###### Selection strategy in points
1. List all characters found in literature (470)
2. Select those using data intended to be used within this research (building footprints w. heights, street network)
3. Eliminate logical correlations (full as well as partial)
4. Eliminate ineffective characters (axial maps, topological skeleton)
5. Add characters where are clear gaps (diversity, plot-level Voronoi cell)
6. Balance scalarity and uniqueness of values
7. Add - meaningless, invariant, empirical correlation

###### Data preprocessing
To minimise errors, it is crucial to run momepy analysis on preprocessed data set. UK OS data (building layer, all of them) are not ready for analysis as they are often split into more elements e.g. one building consists of more shapes and I have no idea what to tell the script to resolve this issue, because different parts of the buildings doesn't even have a common attribute (like Vienna for example) so it is not possible to easily dissolve shapes. In order to prepare this data layer for analysis, some change of topology has to happen, but I have no clue what should be the process. Poor quality of cadastral layer excludes its use (which could be great). To partially overcome this issue, it might be necessary to work with non-uk data (Prague, Vienna...).

##### Generating blocks
Blocks are generated based on the street network and morphological tessellation. Because the street network obtained from open data portal is capturing car-based network, it sometimes does not connect where it should. This should be fixed.

In the case of Prague, using original street network I have generated 9428 blocks, out of which 1839 were "unusual". (19.5%)

	bdkSec > 500 or bskCom < 0.2 or bskCon <0.76 or bskERI < 0.7 or bskShI <0.5  

After that I fixed the street network so it snapped to itself and closed gaps in street network - if the 20m extension of line intersects street network - snap. If the 70 extension of line intersects boundary of built-up area (defined by tessellation), snap. 

The result gave me 9800 blocks and 1092 unusual (11%). 10% of unusual blocks are randomly selected and assessed whether they are correct blocks or incorrect. Based on that, the approximate error is estimated.

Out of 109 randomly selected blocks, 76 were marked as correct representation of block, 33 as incorrect. Based on that, the **estimated error is 3.4%**. That includes blocks which were incorrect before the network snapping as well as blocks which were falsely identified by the snapping.

Additionally, there should be a subchapter talking about exceptions which momepy is not able to capture (Krizikova, Karlin, Nabrezi Karluv most).

###### Problem with blocks in modernist structure
As block is defined by street, it is expecting that street is major divider of space and was there first. In modernist structures, street is often designed as a way though the area, in the middle of what we could see as morphological piece (or block). We are effectively trying to define something which does not exist. **WHAT IS THE CONSEQUENCE OF THIS???**

##### DHC recognition
Instead of straightforward cluster analyisis, we might identify significant clusters based on spatial autocorrelation. DHC could be identified as a specific combination of those significant clusters???


### orientation
Duchêne et al. [5] summarized five measures (Fig. 2), including ‘longest edge,’ ‘weighted bisector,’ ‘wall average,’ ‘statistical weighting,’ and ‘smallest minimum bounding rectangle (SMBR),’ and concluded from their experiments that the SMBR is the most appropriate one. (Yan, 2007)
