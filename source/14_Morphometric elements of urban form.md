# Morphometric elements of urban form

_link back_

_aim of the chapter_

_structure of the chapter_

## Analytical representation of urban form

_introduction to elements and models_

_more paras_

## Elements of urban form in urban morphology

### fundamental elements

_RESEARCH NEEDS TO BE DONE HERE_

#### Building

#### Plot
In traditional Urban Morphology, such unit of analysis is often the *plot*, considered to be the smallest meaningful unit of spatial subdivision and a fundamental component to understand the spatial structure of the ordinary fabric of urban settlements [@panerai2004; @porta2014] and their processes of formation and transformation in time [@whitehand1981]. 

#### Street

_plus more_

#### Up to tissue as a unit of urban form
_Refer back to chapter 2 and discuss the reason why tissue is optimal_
- _it reflects unconstrained morphological unit_
- _tissue as OTU (link to Ch4 and Ch5)_

### Models of urban form

_RESEARCH NEEDS TO BE DONE HERE_

#### Hierarchical

#### Kropf

#### Space Syntax

#### Metric vs configurational

_more_

### Elements of urban form in urban morphometrics

#### Requirements 

#### Issue of availability

#### Issue of plot
_option of tessellation (Hamaina)_
_unexplored_

However, despite its significance, the plot remains a problematic construct. At *ontological* level, there is no agreement on *what exactly a plot is*: indeed, it has been variously defined as “*a land-use unit defined by boundaries on the ground*” [@conzen1969, p. 128], *a module* of the urban tissue constituted by a built-up area and its open pertinent area [@caniggia1979], a piece of property, subject to subdivision and amalgamation as a result of successive patterns of occupation [@moudon1986], or again, according to @bobkova2017a, as “*a basic unit of control*”, “*a fundamental link between spatial and non-spatial medium*”, “*a connection between built space and space of movement*” and “*the framework for building evolution over time*” (p. 47.5). And crucially, more often than not, these definitions may represent very different entities on the ground “*potentially leading to misinterpretation and so a somewhat obscured picture of the dynamics of urban form*” [@kropf1997, p.1].

The second problem has to do with relevance and applicability of the plot to different urban contexts. In literature, plots have been predominantly used to study and characterise traditional urban tissues that having evolved incrementally at the plot level [@bobkova2017a; @conzen1969], are quintessentially plot-based [@panerai2004]. This is however not the case for urban forms that came about after the Second World War, which appear to respond to substantially different rules of organisation [@dibble2016; @feliciotti2018]. For these tissues, “*plots no longer have a structuring role*” [@levy1999 p.83], and hence can hardly be a suitable unit of analysis. While the process of identifying plots in traditional tissues is somewhat less controversial, the same is not true in contemporary ones (figure \ref{fig:glasgow}). 

![Comparison of traditional (left) and modernist (right) urban tissues in Glasgow. Plots are clearly better identifiable—even just visually—in the former, where distinction of public and private space is clear-cut, than in a modernist housing estate, where the transition between public and private is blurred. Source: Ordnance Survey MasterMap, January 2019 (EDINA Digimap Service)](source/figures/ch6/glasgow.pdf "Comparison of traditional and modernist urban tissues in Glasgow"){#fig:glasgow width=100%}

In addition to this issue, the identification of plots in the urban fabric also poses a series of *analytical* problems: given a map or a satellite image, how to consistently determine plot boundaries? And, in case of existing datasets, what do they *actually* represent? What definition of plots do they adopt? Are different datasets comparable?

Not all mapping agencies explicitly report plots and, even when they do, not all of them define or represent plots in the same way. In some spatial databases, as in the Swiss Katasterwesens, plots are represented as unitary land parcel, whilst in other cases, ownership-based plots can be made of multiple unlinked features, as in the French Cadastre, limiting comparability between different datasets. In other cases, the identification of plots from available sources is inferred by the analyst via resource-intensive manual interpretation. However, that makes the resulting procedure on one hand unsuitable for large scale analysis, and on the other potentially biased, as heavily dependent on both individual interpretation and the often uneven quality of the underlying data. Indeed, while through open-data policies [@huijboom2011] and Voluntary Geographical Information System (VGIS) [@barrington-leigh2017] the availability of free-to-use geo-data is growing dramatically, their quality, coverage and resolution is often insufficient to determine individual plots and generally limited to building footprints, street centrelines, natural features and administrative boundaries. All of this reduces considerably the reliability of the analysis and the universality of its results.

Given the aforementioned issues, and despite plots being still widely used in Urban Morphology to capture the “*pattern of human intention and activity*” [@kropf1997, p.5], they are ill-suited as basic unit for UMM applications.


## QUESTION AND HYPOTHESIS (FIND TITLE)
_is mt good unit?_
_how to build a model based on that and relations, which is not strictly hierarchical?_

_HYP_
_tessellation is good subsititute of plot_
_We can use MT to build a relational model based on aerial contiguity & network configuration, limiting the data requeirements at the same time._

## METHOD

### test tessellation as a unit
_ZURICH_

#### Voronoi tessellation in urban form: a state of the art
At the core of the proposed MT lies the *Voronoi tessellation* (VT), a method of geometric partitioning that from a planar set of *‘seeds’* generates a series of polygons, known as *Voronoi Cells* (VC). Each VC encloses the portion of the plane that is closer to its seed than to any other (figure \ref{fig:voro}), ideally representing its ‘*influence zone*’\footnote{The term Voronoi Tessellation can be used to describe both the process of partitioning space (method) and the geometric mesh it generates (output). In this text, the two meanings are used interchangeably.}.

![Voronoi tessellation based on randomised seeds. Each colour represents the area of one tessellation cell (influence zone). Dashed lines end in infinity](source/figures/ch6/voro.png "Voronoi tessellation based on randomised seeds"){#fig:voro width=50%}

VT has been already used in relation to urban form, in the context of spatial clustering algorithms [@dogrusoz2007] and built-form geometry generalisation techniques [@ai2007; @basaraner2004; @li2004; @liu2014], or as input for image-based pattern recognition [@yu2017]. In recent years, VT was used to study the micro-scale properties of the urban fabric [@hamaina2012a; @hamaina2013] in order to produce a reliable method for urban form patterns’ recognition, which pioneered the generation of VC from building footprints. Later, Schirmer and Axhausen [-@schirmer2015; -@schirmer2019] devised a method to define “*influence zones*” around buildings using a “*topological skeleton*” of unbuilt space that is mathematically similar to VT. In parallel, Usui and Asami [-@usui2013; -@usui2017; -@usui2019] included the street network as an additional input alongside the building footprint to the VT algorithm, to mimic the plot structure of traditional Japanese urban fabrics.  Whilst the generated mesh shows remarkable similarity to the plot pattern, its main limitation is the inability to capture the spatial pattern of modernist (post WWII) urban tissues and the highly variable distance between building and street that is typical of such fabrics. On a similar vein, Araldi and Fusco [-@araldi2017; -@araldi2019] developed an approach based on VT and street segments to define a spatial unit based on the pedestrian point of view.
In all these cases, the use of Voronoi tessellation helped to rigorously and reliably cluster components according to their configuration although, as pointed out by @usui2019, the relationship between VC and ‘conventional’ plots has never been directly tested to date. In this sense, the MT approach is to be intended as a continuation of this line of works, insofar it too utilises the VT procedure. However, unlike previous studies, this paper aims to provide a fully operational and replicable method by examining the details of the tessellation process and its parameters, and testing the similarity of morphometric characters as measured on both MC and plots through direct comparison.

#### Morphological Tessellation: the method 
Whenever observing a map or a satellite view of a city, the eye of the observer is caught by the existence of a fundamental relationship between buildings – their geometry and spatial configuration – and the plot pattern. This ‘*intuitive*’ relationship is the reason why approaches based on VT appear to *‘make sense*’ when applied to the urban form of cities: by partitioning the space into cells, they capture the way buildings relate to each other in space and, more precisely, give a spatial meaning to the “*morphological influence*” that each building exerts on its immediate spatial context [@usui2017]. This, in turn, implicitly captures how spatial configuration affects visibility, light penetration, ventilation, movement, etc. around each and every building [@hamaina2012].

The main advantage of methods based on VT is the capacity to derive objective spatial partitions that are applicable to every type of urban tissue in a way independent from the researcher’s subjective interpretation. In addition, most of these methods [@hamaina2012a; @hamaina2013] require minimum data input, as they fundamentally rely on the polygon that describes the footprint of a building. Similarly, the proposed MT method only requires a polygon layer representing building footprints (figure \ref{fig:mt_method}a). From this, MT moves forward in five steps:

1.	*Inward offset from building footprint* (figure \ref{fig:mt_method}b). The offset is necessary to avoid overlaps between boundaries of adjacent buildings and generate a gap between adjacent geometries which will later define the boundaries of the cell. 
2.	*Discretisation of polygons’ boundaries into points* (figure \ref{fig:mt_method}c). As VT can only be generated from point features, the polygonal shape of the building footprint needs to be approximated as series of points to be placed at regular intervals along its boundary, where generated points retain the ID of the building they belong to.
3.	*Generation of Voronoi cells* (figure \ref{fig:mt_method}d). VC are generated around each of the points representing the building footprint. Again, the original ID of the building is preserved in the resulting VC.
4.	*Dissolution of Voronoi cells* (figure \ref{fig:mt_method}e). All VCs sharing the same building ID – and hence generated from the same building – are dissolved in unitary geometries. This step provides a preliminary boundary of the MC.
5.	*Clip of preliminary tessellation* (figure \ref{fig:mt_method}f). As a geometrical construct, VCs tends to infinity as the boundaries of each cell are only defined by proximity with adjacent *‘seeds’*. However, when applied to the analysis of urban form, for obvious reasons no cell can tend to infinity. To avoid this, it is necessary to limit the maximum spatial extent of the tessellation by setting defined study area boundaries.

![The proposed MT method. Grey polygons represent building footprints, while red lines show the edges of tessellation at each step. 3a) Building shapes within boundary of study area (blue); 3b) inward offset from building footprint polygon; 3c) discretisation of  boundaries of polygons into points; 3d) generation of VCs around points: at this stage, the edges of cells (red) tend to infinity; 3e) dissolution of Voronoi cells based on original building ID; 3f) clip of preliminary tessellation by study area.](source/figures/ch6/tesdiag.png "The proposed MT method"){#fig:mt_method width=100%}

Three of the five steps listed above, namely inward offset distance (step 1), discretisation interval (step 2) and clipping method (step 5), require setting parameters that can have a significant effect on the resulting tessellation. As such these need to be evaluated in greater detail. More specifically, in the case of inward offset distance (step 1), the selection of too large values may cause the collapse of narrow parts of building shapes and loss of detail, while too small ones may generate unwanted “*saw-like*” geometries between adjacent buildings. Similarly, a large discretisation interval (step 2) may produce the same “*saw-like*” geometry issue, whilst the opposite would increase exponentially computational demand (figure \ref{fig:sawdiag}). Additionally, since the two parameters are interlinked, their individual effect on the shape of each cell is not independent: as such, their combined effect needs to be balanced to generate geometries with insignificant shape deviation and minimum computational burden. Finally, the adoption of a clipping method for the tessellation (step 5) also requires considerations in order to appropriately limit the focus of the analysis to the urbanized footprint and exclude large open un-built spaces while limiting potential MAUP effects [@openshaw1984]. Due to the importance of correctly setting these parameters, Section _4.2REF_ will discuss the adopted method for the determination of inward offset distance (step 1), discretisation interval (step 2) and method.

![Illustration of the effect of improper combination of inward offset distance and discretisation interval causing “saw-like” geometry on the boundary bethween adjacent buildings (b) compared to ideal combination (a).](source/figures/ch6/sawdiag.pdf "Illustration of the effect"){#fig:sawdiag width=70%}

The conceptual sequence described in this section, was translated into a Python code, building its key parts on the capability of SciPy [@jones2001], Shapely [@gillies2007] and GeoPandas [@jordahl2019]. Computation was run on Ubuntu Bionic 18.04 running at Amazon Web Services EC2. _The resulting Python script is released as part of the open source Python package named “momepy: Urban Morphology Measuring Toolkit"._

#### Morphological Tessellation and plots: data and comparison method
##### The dataset
_add reasoning why Zurich is here while everything else is done on Prague_
The MT method and the informational value of MCs compared to plots were tested within the administrative area of Zurich (figure \ref{fig:extent}). This was chosen for its historically characterised and heterogeneous urban fabric as well as for the availability of the ‘_Amtliche Vermessung_’ dataset, a freely-accessible resource containing high-quality information on cadastral plots and building footprints. Before generating the MT, data was cleaned as follows:

1. From the *cadastral layer*, which covers the 100% of study area, all features not containing buildings (e.g. streets or large open spaces) were removed, as they do not represent built-up form;
2. From the *building layer*, features smaller than 30 m^2^ were filtered out, as such smaller objects are likely ancillary structures rather than actual buildings.

![The selected study area, defined by the administrative boundary of the Zurich Kanton (left); the Langstrasse area in Zurich (right) was selected for testing the tessellation algorithm parameters: the red-line boundaries follow the street centerlines.](source/figures/ch6/extent_cases.png "Illustration of the effect"){#fig:extent width=100%}

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


### test tessellation contiguity as aggregation
_ISUF_
_zuirch_
By the same token, it should be pointed out that the MCs do offer added values that are relevant on their own, regardless to their similarity to the plots. These have to do with the potential innovations – yet largely unexplored – which are triggered by the very nature of this geometry. For example, unlike other methods of urban form partitioning, the MT covers uniformly the totality of space within the set study area, allowing to capture the topology of contiguous space at the plot-level. Indeed, since all MCs are determined by adjacency, by using MT it is possible to think in terms of topological distance (set number of topological steps between cells) rather than geographic distance (set metric distance around elements, either “as the crow flies” or along the street network). Moreover, thinking in terms of topological distance as opposed to metric, the MT can be used to define new aggregated analytical units that are able to capture the immediate area of influence of a building on its surrounding fabric and, at the same time, of the surrounding fabric on the building. Indeed, since the size of each MCs depends on the granularity of the urban structure, the spatial representation of a set topological distance would be far smaller for a MC located in a fine-grained built-up area than for the same located in a coarse one (figure \ref{fig:contiguity_diagram}). Crucially, this is a kind of information that would not be possible to access with plots alone, which allows to reframe the very idea of ‘proximity’ by rethinking the relationship between scale and spatial meaning, thereby enhancing the ability to capture the context in UMM analysis.

![Relationship between morphological cells of topological distance 2: the red geometry represents the adjacency network of neighbouring elements (buildings, MC) at topological distance 1 (adjacent neighbour of first order), while blue geometry represents the boundary of the aggregated analytical unit of topological distance 2 for each of the highlighted buildings. In the image, a fabric characterised by fewer and sparser buildings (b) generate larger cells and aggregated units compared to a denser and more compact fabric (a).](source/figures/ch6/contiguity_diagram.png "Relationship between morphological cells of topological distance 2"){#fig:contiguity_diagram width=100%}

## RESULTS

### test tessellation as a unit
_ZURICH_

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

![Example of LISA patterns of Frequency measured on the MT shows Moran Local Scatterplot LISA clusters and actual distribution of values.](source/figures/ch6/100_frequency.png "xample of LISA patterns of Frequenc"){#fig:100_frequency width=100%}

The analysis of patterns with LISA (figure \ref{fig:100_frequency}) captures differences across measured characters; however, given the dissimilarity of the datasets due to multi-building plots, the accuracy scores are not expected to reach values close to 1. Highest pattern similarity is recognised for the *Frequency* character (~0.78, corresponding to an almost 80% match) (figure \ref{fig:accu}), followed by *Orientation* and *Diversity* characters (Gini Index of Area and Gini Index of CAR) and CAR (0.74 – 0.66), while *Dimension* characters are around ~0.5 depending on the sample considered (single- or multi-building plots). *Shape* characters are consistently the ones providing lowest accuracy, apart from *Reach Centrality*, due to the single-building vs. multi-building deviation in the datasets. Overall, the difference between samples is relatively consistent, with single-building plots reaching values between 0.1 and 0.2 higher than multi-building plots. While none of the values indicates an equality of both datasets, some are close enough to be considered as proxies of each other. The effect of buffer distance confirms already observed pattern and the stability of the 100m buffer.

![LISA accuracy of cadastral values and each of the selected buffers of tessellation based on the whole dataset  (figures for single and multi-building plots are found in the Appendix XXX).](source/figures/ch6/accu.pdf "LISA accuracy of cadastral and MT values"){#fig:accu width=100%}

\begin{longtable}[]{@{}lllll@{}}
\caption{aLISA for the whole dataset, single-building plots and multi-building plots at 100m buffer.} \label{tab:accu_results} \\
\toprule
Category & Character & All &
Single & Multi\tabularnewline
\midrule
\endhead
Dimension & Area & 0.5938 & 0.64475 & 0.5090\tabularnewline
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
& Gini Index of CAR & 0.65858 & 0.6742 & 0.6423\tabularnewline
Connectivity & Reach & 0.4007 & 0.3363 & 0.4644\tabularnewline
\bottomrule
\end{longtable}

#### Discussion of results

Our results suggest that the proposed method contributes to resolve some of the limitations associated with using the plot as unit of UMM analysis. However, the picture resulting from testing the similarity between cadastral plots and MCs is rather complex. 
Notably, the significance of similarity between plots and MCs varies considerably depending on the morphometric character selected: this is generally high for all Intensity characters (*Frequency, CAR*, whilst Shape characters (*Rectangularity, Circular Compactness, Shape Index*, and *Fractal Dimension*) report a comparatively poorer performance and a higher deviation. This means that if, for several of the morphometric characters assessed, MT is able to retain plot-level information which is comparable to that provided by the cadastral layer, for other characters MCs are less efficient proxies of plots and capture comparatively different information. 

It is also evident that the similarity of datasets is higher across all measured characters for single-building plots compared to multi-building plots. Considering that the former ones are predominantly found in pre-industrial urban tissues while the latter are more typical of modern and contemporary development, it is suggested that MT might be a *better proxy* of plots in the context of traditional fabrics than it is in modernist and contemporary ones.

Overall, there appears to be substantial scope for the MC to be utilised as basic unit of UMM analysis, given its ability to capture meaningful patterns of urban form at the plot scale, the degree of reliability and universality of the underlying method and the wide accessibility of the data required to generate it. Indeed, while the recognition of plots can be very troublesome and resource intensive, morphological tessellation is consistent throughout, since it is only based on building footprint information which is equally present in all kinds of urban areas. Moreover, by using morphological tessellation instead of traditional methods relying on buildings, street networks and plots, data dependency is reduced by a third as the tessellation is generated from the building layer alone. 

#### Limits of morphological tessellation
Whilst MT and MC appear to be promising new addition to the tools available for UMM applications, a first limit of this work is that the cadastral parcels in Zurich, which we have loosely treated as ‘plots’, are solely based on land-ownership. That causes discrepancy between the generated tessellation and the cadastral layer which includes multi-building plots. However, as only 21% of plots are affected and results are reported for both groups, we believe that the presented method is robust enough to provide relevant results.
Second, whilst it is true that a MT can be generated directly from a building layer alone, it cannot be created from any building layer, as this needs to comply to certain quality requirements. Notably, since the method sees every feature of GIS layer as an individual input for tessellation, it is important not to have buildings composed of multiple features each representing, for example, different heights or different parts of the same (as in the case of British Ordnance Survey). Similarly, it is important not to have different independent buildings collapsed into a single simplified feature (as in the case of vast portions of Open Street Maps).


### test tessellation contiguity as aggregation
_ISUF_

## THEORY Relational model of urban form
_Relational model of urban form, DISCUSSION_
_Also mention block = Generating blocks appendix_

## CONCLUSIONS

_zurich_
Plots are commonly seen as the ideal spatial division for morphological analysis, but they also have their drawbacks, causing the limited applicability of plot-based methods and, more importantly, the reduced reliability of results obtained by employing them. The aim of this work is to address some of the issues characterising the definition of plot and plot boundaries, the availability and accessibility of plot data and the labour intensiveness of manually extracting reliable plot-level information, aspects that limit the potential of Urban Morphometrics. The need to objectively define a unit of analysis able to capture the smallest and arguably most fundamental level of spatial subdivision, and to develop a reliable and replicable method to generate and measure it, is the rationale behind the *Morphological Cell* (MC) unit and the *Morphological Tessellation* (MT) method. 

The universal and algorithmic nature of the proposed MT has the potential to scale up UMM analysis with minimum effort to the large scale , while significantly reducing the interpretative input of the analysts along the process. This latter property of MT appears to be particularly relevant to making large scale UMM analysis viable and take full advantage of big data in the GIS area. The robustness of the proposed method and the validity of the proposed spatial unit of analysis is verified through the assessment of 12 representative morphometric characters and the application of three different *quantitative* comparative methods, Spearman’s correlation, NRMSD and accuracy of LISA, aimed at evaluating the similarity of information between MCs and cadastral plots.  

The MT method, as tested and presented in this paper, offers a different approach to spatial division whilst still capturing a level of quality of information on urban form that is similar to that conveyed by the plot. Findings presented in this paper indicate that there is overlap between the information derived from cadastral plots and the one derived from morphological tessellation. The degree of this overlap depends on the category of morphometric characters and the type of urban context, but for certain types of morphologic analysis it is large enough to consider MCs reliable proxies of plots. At the same time, MCs cannot fully *replace* plots in the understanding and analysis of urban form patterns.
