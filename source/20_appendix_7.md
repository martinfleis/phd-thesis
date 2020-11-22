# Appendix A7: Supplementary material for chapter 7 {.unnumbered}

\renewcommand\thefigure{A7.\arabic{figure}}
\setcounter{figure}{0}
\renewcommand\thetable{A7.\arabic{table}}
\setcounter{table}{0}
\pagestyle{plain}

## 7.1 Selection of primary characters {.unnumbered}

Supplementary material for section 7.1.2.1.1. Table \ref{tab:long_chars} contains intial selection of applicable characters and reasoning behind its selection or exclusion.

\small
\begin{longtable}[]{@{}P{1.5cm}P{3.5cm}P{2.8cm}P{1.3cm}P{2.5cm}P{2cm}@{}}
\caption{Initial selection of applicable characters as an extraction from the Table of Urban Form Characters (Table A4.1.)
Selection reflects steps defined in section 7.1.2.1.1. Result indicates whether teseted character is included in
the final set of primary characters or not, alternatively specifies the reason. Characters using different data
than specified in the relational model are excluded a priori.} \label{tab:long_chars} \\
\toprule
     id &                                   index &            element & extent &      category &  result \\
\midrule
\endhead
\midrule
\multicolumn{6}{r}{{Continued on next page}} \\
\midrule
\endfoot

\bottomrule
\endlastfoot
 sdbAre &                                    area &           building &     S &     dimension &     included \\
 sdbFlA &                              floor area &           building &     S &     dimension &    collinear \\
 sdbHei &                                  height &           building &     S &     dimension &     included \\
 sdbVol &                                  volume &           building &     S &     dimension &     included \\
 sdbPer &                               perimeter &           building &     S &     dimension &     included \\
 sdbCoA &                          courtyard area &           building &     S &     dimension &     included \\
 sdbBRA &                 bounding rectangle area &           building &     S &     dimension &    collinear \\
 sdbBRW &                bounding rectangle width &           building &     S &     dimension &    collinear \\
 sbdBRL &               bounding rectangle length &           building &     S &     dimension &    collinear \\
 sdbBRP &            bounding rectangle perimeter &           building &     S &     dimension &    collinear \\
 sdbECR &                 enclosing circle radius &           building &     S &     dimension &    collinear \\
 sdbCHA &                        convex hull area &           building &     S &     dimension &    collinear \\
 sdbCHP &                   convex hull perimeter &           building &     S &     dimension &    collinear \\
 ssbFoF &                             form factor &           building &     S &         shape &     included \\
 ssbFra &                       fractal dimension &           building &     S &         shape &    collinear \\
 ssbVFR &                     volume/façade ratio &           building &     S &         shape &     included \\
 ssbCCo &                    circular compactness &           building &     S &         shape &     included \\
 ssbSCo &                      square compactness &           building &     S &         shape &    collinear \\
 ssbCon &                              convexeity &           building &     S &         shape &    collinear \\
 ssbCor &                                 corners &           building &     S &         shape &     included \\
 ssbShI &                             shape index &           building &     S &         shape &    collinear \\
 ssbSqu &                              squareness &           building &     S &         shape &     included \\
 ssbERI &            equivalent rectangular index &           building &     S &         shape &     included \\
 ssbElo &                              elongation &           building &     S &         shape &     included \\
 ssbCCD &  centroid - corners  distance deviation &           building &     S &         shape &     included \\
 ssbCCM &        centroid - corners mean distance &           building &     S &         shape &     included \\
 stbOri &                       solar orientation &           building &     S &  distribution &     included \\
 stbSAl &                        street alignment &           building &     S &  distribution &     included \\
 stbCeA &                          cell alignment &           building &     S &  distribution &     included \\
 sdcLAL &                     longest axis length &  tessellation cell &     S &     dimension &     included \\
 sdcAre &                                    area &  tessellation cell &     S &     dimension &     included \\
 sdcBRA &                 bounding rectangle area &  tessellation cell &     S &     dimension &    collinear \\
 sdcBRW &                bounding rectangle width &  tessellation cell &     S &     dimension &    collinear \\
 sdcBRL &               bounding rectangle length &  tessellation cell &     S &     dimension &    collinear \\
 sdcBRP &            bounding rectangle perimeter &  tessellation cell &     S &     dimension &    collinear \\
 sdcECR &                 enclosing circle radius &  tessellation cell &     S &     dimension &    collinear \\
 sdcCHA &                        convex hull area &  tessellation cell &     S &     dimension &    collinear \\
 sdcCHP &                   convex hull perimeter &  tessellation cell &     S &     dimension &    collinear \\
 sscCCo &                    circular compactness &  tessellation cell &     S &         shape &     included \\
 sscSCo &                      square compactness &  tessellation cell &     S &         shape &    collinear \\
 sscElo &                              elongation &  tessellation cell &     S &         shape &    collinear \\
 sscFra &                       fractal dimension &  tessellation cell &     S &         shape &    collinear \\
 sscCon &                              convexeity &  tessellation cell &     S &         shape &    collinear \\
 sscShI &                             shape index &  tessellation cell &     S &         shape &    collinear \\
 sscERI &            equivalent rectangular index &  tessellation cell &     S &         shape &     included \\
 sscElo &                              elongation &  tessellation cell &     S &         shape &    collinear \\
 stcOri &                       solar orientation &  tessellation cell &     S &  distribution &     included \\
 stcSAl &                        street alignment &  tessellation cell &     S &  distribution &     included \\
 sicCAR &                     coverage area ratio &  tessellation cell &     S &     intensity &     included \\
 sicFAR &                        floor area ratio &  tessellation cell &     S &     intensity &     included \\
 sdsLen &                                  length &     street segment &     S &     dimension &     included \\
 sdsSPW &                    street profile width &             street &     S &     dimension &     included \\
 sdsSPH &                   street profile height &             street &     S &     dimension &     included \\
 sdsSPR &       street profile height/width ratio &     street segment &     S &         shape &     included \\
 sdsSPO &                         street openness &             street &     S &  distribution &     included \\
 sdsSWD &                       setback deviation &             street &     S &     diversity &     included \\
 sdsSHD &                        height deviation &             street &   	 S &     diversity &     included \\
 sssLin &                               linearity &     street segment &     S &         shape &     included \\
 sdsAre &                            area covered &  tessellation cell &     S &     dimension &     included \\
 sisBpS &                   buildings per segment &           building &     S &     intensity &   no meaning \\
 sisBpM &                     buildings per meter &           building &     S &     intensity &     included \\
 sddAre &                            area covered &  tessellation cell &     S &     dimension &     included \\
 sddBpN &                      buildings per node &           building &     S &     intensity &   no meaning \\
 mtbSWR &                      shared walls ratio &           building &     M &  distribution &     included \\
 mtbAli &                      building alignment &           building &     M &  distribution &     included \\
 mtbNDi &                 mean neighbour distance &           building &     M &  distribution &     included \\
 mtcNei &                               neigbours &  tessellation cell &     M &  distribution &   no meaning \\
 mtcWNe &                         neigbours per m &  tessellation cell &     M &  distribution &     included \\
 mdcAre &                            area covered &  tessellation cell &     M &     dimension &     included \\
 mtsMDO &           mean deviation of orientation &     street segment &     M &  distribution &   no meaning \\
 misRea &                           reached cells &  tessellation cell &     M &     intensity &     included \\
 mdsLen &                                  length &     street segment &     M &     dimension &    collinear \\
 mdsAre &                            area covered &  tessellation cell &     M &     dimension &     included \\
 mtdDeg &                             node degree &        street node &     M &  distribution &     included \\
 mtdMDi &                  mean distance to nodes &        street node &     M &     dimension &     included \\
 midRea &                           reached cells &  tessellation cell &     M &     intensity &     included \\
 midAre &                            area covered &  tessellation cell &     M &     dimension &     included \\
 libNCo &                    number of courtyards &           building &     L &     intensity &     included \\
 ldbPWL &                   perimeter wall length &           building &     L &     dimension &     included \\
 ltbIBD &            mean inter-building distance &           building &     L &  distribution &     included \\
 ltcBuA &                      building adjacency &           building &     L &  distribution &     included \\
 licGDe &                           gross density &  tessellation cell &     L &     intensity &     included \\
 ltcWRB &                 weighted reached blocks &  tessellation cell &     L &     intensity &     included \\
 ldkAre &                              block area &              block &     L &     dimension &     included \\
 ldkPer &                         block perimeter &              block &     L &     dimension &     included \\
 ldkBRA &                 bounding rectangle area &              block &     L &     dimension &    collinear \\
 ldkBRW &                bounding rectangle width &              block &     L &     dimension &    collinear \\
 ldkBRL &               bounding rectangle length &              block &     L &     dimension &    collinear \\
 ldkBRP &            bounding rectangle perimeter &              block &     L &     dimension &    collinear \\
 ldkECR &                 enclosing circle radius &              block &     L &     dimension &    collinear \\
 ldkCHA &                        convex hull area &              block &     L &     dimension &    collinear \\
 ldkCHP &                   convex hull perimeter &              block &     L &     dimension &    collinear \\
 lskElo &                        block elongation &              block &     L &         shape &    collinear \\
 lskFra &                 block fractal dimension &              block &     L &         shape &    collinear \\
 lskCCo &              block circular compactness &              block &     L &         shape &     included \\
 lskSCo &               blocks square compactness &              block &     L &         shape &    collinear \\
 lskCon &                        block convexeity &              block &     L &         shape &    collinear \\
 lskShI &                       block shape index &              block &     L &         shape &    collinear \\
 lskERI &      block equivalent rectangular index &              block &     L &         shape &     included \\
 lskCWA &               Compactness-weighted axis &              block &     L &         shape &     included \\
 ltkOri &                 block solar orientation &              block &     L &  distribution &     included \\
 ltkNei &                        block neighbours &              block &     L &  distribution &   no meaning \\
 ltkWBN &               weighted block neighbours &              block &     L &  distribution &     included \\
 likBpB &                     buildings per block &              block &     L &     intensity &   no meaning \\
 likWBB &            weighted buildings per block &              block &     L &     intensity &     included \\
 lcdMes &                              meshedness &     street network &     L &  connectivity &     included \\
 ldsMSL &                     mean segment length &     street network &     L &     dimension &     included \\
 ldsTSL &                    total segment length &     street network &     L &     dimension &    collinear \\
 ldsCDL &                       cul-de-sac length &     street network &     L &     dimension &     included \\
 ldsRea &                           reached cells &  tessellation cell &     L &     dimension &     included \\
 lddNDe &                            node density &     street network &     L &     intensity &     included \\
 lddRea &                           reached cells &  tessellation cell &     L &     dimension &     included \\
 lddARe &                            area covered &  tessellation cell &     L &     dimension &     included \\
 lcnMND &                        mean node degree &     street network &     L &  connectivity &    collinear \\
 linPDE &                 proportion of dead-ends &     street network &     L &  connectivity &     included \\
 linP3W &       proportion of 3-way intersections &     street network &     L &  connectivity &     included \\
 linP4W &       proportion of 4-way intersections &     street network &     L &  connectivity &     included \\
 linWID &           weighted intersection density &     street network &     L &     intensity &     included \\
 licSpA &                      spatial attraction &  tessellation cell &     L &     intensity &        scale \\
 lcnSLP &                    self-loop proportion &     street network &     L &  connectivity &    collinear \\
 lcnNeC &                      network clustering &     street network &     L &  connectivity &    collinear \\
 lncWNC &             weighted network clustering &     street network &     L &  connectivity &    collinear \\
 lcnEdC &                       edge connectivity &     street network &     L &  connectivity &    collinear \\
 lcnNoC &                       node connectivity &     street network &     L &  connectivity &    collinear \\
 lcnCyC &                   cyclomatic complexity &     street network &     L &  connectivity &    collinear \\
 lcnENR &                       edge / node ratio &     street network &     L &  connectivity &    collinear \\
 lcnExC &                   external connectivity &     street network &     L &  connectivity &      no data \\
 lcnGaI &                             gamma index &     street network &     L &  connectivity &    collinear \\
 lcnDiD &                    directional distance &     street network &     L &  connectivity &  ineffective \\
 lcnGCC &           global clustering coefficient &     street network &     L &  connectivity &  meaningless \\
 lcnRed &                              redundancy &     street network &     L &  connectivity &  ineffective \\
 lcnClo &              local closeness centrality &     street network &     L &  connectivity &     included \\
 xcnSCl &                       square clustering &     street network &    XL &  connectivity &     included \\
\end{longtable}
\normalsize
\newpage

The following figures measure Spearman correlation between tested characters within each group of elements. It illustrates the reasoning behind exclusion of characters due to collinearity. From a group of collinear characters, only one is included in the final set. The selection is driven by variance, interpretability and literature.


![Correlation matrix of Spearman's rho values capturing the statistical relationship between morphometric values of tested characters based on buildings.](source/figures/a7/buildings_corr.pdf "Correlation matrix of Spearman's rho values capturing the statistical relationship between morphometric values of tested characters based on buildings."){#fig:blg_cor width=100%}

![Correlation matrix of Spearman's rho values capturing the statistical relationship between morphometric values of tested characters based on tessellation cells.](source/figures/a7/tessellation_corr.pdf "Correlation matrix of Spearman's rho values capturing the statistical relationship between morphometric values of tested characters based on tessellation cells."){#fig:tes_cor width=100%}

![Correlation matrix of Spearman's rho values capturing the statistical relationship between morphometric values of tested characters based on streets.](source/figures/a7/streets_corr.pdf "Correlation matrix of Spearman's rho values capturing the statistical relationship between morphometric values of tested characters based on streets."){#fig:stree_cor width=100%}

![Correlation matrix of Spearman's rho values capturing the statistical relationship between morphometric values of tested characters based on blocks.](source/figures/a7/blocks_corr.pdf "Correlation matrix of Spearman's rho values capturing the statistical relationship between morphometric values of tested characters based on blocks."){#fig:blo_cor width=100%}

![Correlation matrix of Spearman's rho values capturing the statistical relationship between morphometric values of tested characters based on network nodes.](source/figures/a7/nodes_corr.pdf "Correlation matrix of Spearman's rho values capturing the statistical relationship between morphometric values of tested characters based on  network nodes."){#fig:nodes_cor width=100%}

\newpage

## 7.2 Classification of primary characters {.unnumbered}

Classification of primary characters into categories. See section 7.1.2.1.2 for details.


| notation          | index                                | element                         | category     | extent   |
|:------------------|:-------------------------------------|:--------------------------------|:-------------|---------:|
| $a_{blg}$         | area                                 | building                        | dimension    | S        |
| $h_{blg}$         | height                               | building                        | dimension    | S        |
| $v_{blg}$         | volume                               | building                        | dimension    | S        |
| $p_{blg}$         | perimeter                            | building                        | dimension    | S        |
| $a_{blg_c}$       | courtyard area                       | building                        | dimension    | S        |
| $FoF_{blg}$       | form factor                          | building                        | shape        | S        |
| $VFR_{blg}$       | volume to façade ratio               | building                        | shape        | S        |
| $CCo_{blg}$       | circular compactness                 | building                        | shape        | S        |
| $Cor_{blg}$       | corners                              | building                        | shape        | S        |
| $Squ_{blg}$       | squareness                           | building                        | shape        | S        |
| $ERI_{blg}$       | equivalent rectangular index         | building                        | shape        | S        |
| $Elo_{blg}$       | elongation                           | building                        | shape        | S        |
| $CCD_{blg}$       | centroid - corner distance deviation | building                        | shape        | S        |
| $CCM_{blg}$       | centroid - corner mean distance      | building                        | shape        | S        |
| $Ori_{blg}$       | solar orientation                    | building                        | distribution | S        |
| $SAl_{blg}$       | street alignment                     | building                        | distribution | S        |
| $CAl_{blg}$       | cell alignment                       | building                        | distribution | S        |
| $LAL_{cell}$      | longest axis length                  | tessellation cell               | dimension    | S        |
| $a_{cell}$        | area                                 | tessellation cell               | dimension    | S        |
| $CCo_{cell}$      | circular compactness                 | tessellation cell               | shape        | S        |
| $ERI_{cell}$      | equivalent rectangular index         | tessellation cell               | shape        | S        |
| $Ori_{cell}$      | solar orientation                    | tessellation cell               | distribution | S        |
| $SAl_{cell}$      | street alignment                     | tessellation cell               | distribution | S        |
| $CAR_{cell}$      | coverage area ratio                  | tessellation cell               | intensity    | S        |
| $FAR_{cell}$      | floor area ratio                     | tessellation cell               | intensity    | S        |
| $l_{edg}$         | length                               | street segment                  | dimension    | S        |
| $w_{sp}$          | width                                | street profile                  | dimension    | S        |
| $h_{sp}$          | height                               | street profile                  | dimension    | S        |
| $HWR_{sp}$        | height to width ratio                | street profile                  | shape        | S        |
| $Ope_{sp}$        | openness                             | street profile                  | distribution | S        |
| $wDev_{sp} $      | width deviation                      | street profile                  | diversity    | S        |
| $hDev_{sp}$       | height deviation                     | street profile                  | diversity    | S        |
| $Lin_{edg}$       | linearity                            | street segment                  | shape        | S        |
| $a_{edg}$         | area covered                         | street segment                  | dimension    | S        |
| $BpM_{edg}$       | buildings per meter                  | street segment                  | intensity    | S        |
| $a_{node}$        | area covered                         | street node                     | dimension    | S        |
| $SWR_{blg}$       | shared walls ratio                   | adjacent buildings              | distribution | S        |
| $Ali_{blg}$       | alignment                            | neighbouring buildings          | distribution | S        |
| $NDi_{blg}$       | mean distance                        | neighbouring buildings          | distribution | S        |
| $WNe_{cell}$      | weighted neighbours                  | tessellation cell               | distribution | S        |
| $a_{cell_n}$      | area covered                         | neighbouring cells              | dimension    | S        |
| $RC_{edg_n}$      | reached cells                        | neighbouring segments           | intensity    | S        |
| $a_{edg_n}$       | reached area                         | neighbouring segments           | dimension    | S        |
| $deg_{node}$      | degree                               | street node                     | distribution | S        |
| $MDi_{node}$      | mean distance to neighbouring nodes  | street node                     | dimension    | S        |
| $RC_{node_n}$     | reached cells                        | neighbouring nodes              | intensity    | S        |
| $a_{node_n}$      | reached area                         | neighbouring nodes              | dimension    | S        |
| $NCo_{blg_{adj}}$ | number of courtyards                 | adjacent buildings              | intensity    | S        |
| $p_{blg_{adj}}$   | perimeter wall length                | adjacent buildings              | dimension    | S        |
| $IBD_{blg}$       | mean inter-building distance         | neighbouring buildings          | distribution | S        |
| $BuA_{blg}$       | building adjacency                   | neighbouring buildings          | distribution | S        |
| $GFAR_{cell}$     | gross floor area ratio               | neighbouring tessellation cells | intensity    | S        |
| $WRB_{cell}$      | weighted reached blocks              | neighbouring tessellation cells | intensity    | S        |
| $a_{blk}$         | area                                 | block                           | dimension    | S        |
| $p_{blk}$         | perimeter                            | block                           | dimension    | S        |
| $CCo_{blk}$       | circular compactness                 | block                           | shape        | S        |
| $ERI_{blk}$       | equivalent rectangular index         | block                           | shape        | S        |
| $CWA_{blk}$       | compactness-weighted axis            | block                           | shape        | S        |
| $Ori_{blk}$       | solar orientation                    | block                           | distribution | S        |
| $wN_{blk}$        | weighted neighbours                  | block                           | distribution | S        |
| $wC_{blk}$        | weighted cells                       | block                           | intensity    | S        |
| $Mes_{node}$      | local meshedness                     | street network                  | connectivity | M        |
| $MSL_{edg}$       | mean segment length                  | street network                  | dimension    | S        |
| $CDL_{node}$      | cul-de-sac length                    | street network                  | dimension    | S        |
| $RC_{edg}$        | reached cells                        | street network                  | dimension    | S        |
| $D_{node}$        | node density                         | street network                  | intensity    | M        |
| $RC_{node_{net}}$ | reached cells                        | street network                  | dimension    | S        |
| $a_{node_{net}}$  | reached area                         | street network                  | dimension    | S        |
| $pCD_{node}$      | proportion of cul-de-sacs            | street network                  | connectivity | M        |
| $p3W_{node}$      | proportion of 3-way intersections    | street network                  | connectivity | M        |
| $p4W_{node}$      | proportion of 4-way intersections    | street network                  | connectivity | M        |
| $wD_{node}$       | weighted node density                | street network                  | intensity    | M        |
| $lCC_{node}$      | local closeness centrality           | street network                  | connectivity | M        |
| $sCl_{node}$      | square clustering                    | street network                  | connectivity | L        |

Table: Classification of primary characters. Grain is S for all characters. \label{prim_chars_clas}

\newpage

References for primary characters. Characters without a reference are newly introduced or adapted to the point where it would not be correct to refer to its original implementation. See section 7.1.2.1.2 for details.


| notation          | reference           | id     |
|:------------------|:--------------------|:-------|
| $a_{blg}$         | [@hallowell2013]    | sdbAre |
| $h_{blg}$         | [@schirmer2015]     | sdbHei |
| $v_{blg}$         | [@yoshida2005]      | sdbVol |
| $p_{blg}$         | [@vanderhaegen2017] | sdbPer |
| $a_{blg_c}$       | [@schirmer2015]     | sdbCoA |
| $FoF_{blg}$       | [@bourdic2012]      | ssbFoF |
| $VFR_{blg}$       | [@yoshida2005]      | ssbVFR |
| $CCo_{blg}$       | [@dibble2017]       | ssbCCo |
| $Cor_{blg}$       | [@steiniger2008]    | ssbCor |
| $Squ_{blg}$       | [@steiniger2008]    | ssbSqu |
| $ERI_{blg}$       | [@basaraner2017]    | ssbERI |
| $Elo_{blg}$       | [@steiniger2008]    | ssbElo |
| $CCD_{blg}$       |                     | ssbCCD |
| $CCM_{blg}$       | [@schirmer2015]     | ssbCCM |
| $Ori_{blg}$       | [@schirmer2015]     | stbOri |
| $SAl_{blg}$       | [@schirmer2015]     | stbSAl |
| $CAl_{blg}$       |                     | stbCeA |
| $LAL_{cell}$      |                     | sdcLAL |
| $a_{cell}$        | [@hamaina2012a]     | sdcAre |
| $CCo_{cell}$      |                     | sscCCo |
| $ERI_{cell}$      |                     | sscERI |
| $Ori_{cell}$      |                     | stcOri |
| $SAl_{cell}$      |                     | stcSAl |
| $CAR_{cell}$      | [@hamaina2013]      | sicCAR |
| $FAR_{cell}$      | [@hamaina2013]      | sicFAR |
| $l_{edg}$         | [@gil2012]          | sdsLen |
| $w_{sp}$          | [@araldi2019]       | sdsSPW |
| $h_{sp}$          | [@araldi2019]       | sdsSPH |
| $HWR_{sp}$        | [@araldi2019]       | sdsSPR |
| $Ope_{sp}$        | [@araldi2019]       | sdsSPO |
| $wDev_{sp} $      | [@araldi2019]       | sdsSWD |
| $hDev_{sp}$       | [@araldi2019]       | sdsSHD |
| $Lin_{edg}$       | [@araldi2019]       | sssLin |
| $a_{edg}$         |                     | sdsAre |
| $BpM_{edg}$       |                     | sisBpM |
| $a_{node}$        |                     | sddAre |
| $SWR_{blg}$       | [@hamaina2012a]     | mtbSWR |
| $Ali_{blg}$       | [@hijazi2016]       | mtbAli |
| $NDi_{blg}$       | [@hijazi2016]       | mtbNDi |
| $WNe_{cell}$      |                     | mtcWNe |
| $a_{cell_n}$      |                     | mdcAre |
| $RC_{edg_n}$      |                     | misRea |
| $a_{edg_n}$       |                     | mdsAre |
| $deg_{node}$      | [@boeing2018]       | mtdDeg |
| $MDi_{node}$      |                     | mtdMDi |
| $RC_{node_n}$     |                     | midRea |
| $a_{node_n}$      |                     | midAre |
| $NCo_{blg_{adj}}$ | [@schirmer2015]     | libNCo |
| $p_{blg_{adj}}$   |                     | ldbPWL |
| $IBD_{blg}$       | [@caruso2017]       | ltbIBD |
| $BuA_{blg}$       | [@vanderhaegen2017] | ltcBuA |
| $GFAR_{cell}$     | [@dibble2017]       | licGDe |
| $WRB_{cell}$      |                     | ltcWRB |
| $a_{blk}$         | [@dibble2017]       | ldkAre |
| $p_{blk}$         | [@gil2012]          | ldkPer |
| $CCo_{blk}$       | [@schirmer2015]     | lskCCo |
| $ERI_{blk}$       | [@basaraner2017]    | lskERI |
| $CWA_{blk}$       | [@feliciotti2018]   | lskCWA |
| $Ori_{blk}$       | [@gil2012]          | ltkOri |
| $wN_{blk}$        |                     | ltkWNB |
| $wC_{blk}$        |                     | likWBB |
| $Mes_{node}$      | [@feliciotti2018]   | lcdMes |
| $MSL_{edg}$       |                     | ldsMSL |
| $CDL_{node}$      |                     | ldsCDL |
| $RC_{edg}$        |                     | ldsRea |
| $D_{node}$        |                     | lddNDe |
| $RC_{node_{net}}$ |                     | lddRea |
| $a_{node_{net}}$  |                     | lddARe |
| $pCD_{node}$      | [@lowry2014]        | linPDE |
| $p3W_{node}$      | [@boeing2018]       | linP3W |
| $p4W_{node}$      | [@boeing2018]       | linP4W |
| $wD_{node}$       | [@dibble2017]       | linWID |
| $lCC_{node}$      | [@porta2006]        | lcnClo |
| $sCl_{node}$      |                     | xcnSCl |

Table: Reference table for primary characters. Contains references to existing literature and to identifier of each character used within computational Jupyter notebooks. \label{prim_chars_ref}

\newpage

## 7.3 Sectional diagram analysis {.unnumbered}

Sectional diagrams show the distribution of measured values along the longitudinal section through the whole case study. Diagrams were generated every 1km and individually assessed to understand the effect of a different number of steps on the distribution. The overall aim is to use that number of steps which illustrate the tendency within the local area but in too smooth to disable identification of boundaries between areas of different characters. Based on the visual assessment of sectional diagrams, three topological steps are the closest option to the goal mentioned above. Figures \ref{fig:sect_full} and \ref{fig:sect_det} below illustrate one such diagram and its detail.

Note: Please refer to the electronical version of the thesis for a better clarity. Sectional diagrams are not optimised for print.

![Full sectional diagrams illustrating spatial distribution of selected values (IQM of area, ID Theil index of area, IQR of area, adjacency).](source/figures/a7/sect_full.pdf "Full sectional diagrams illustrating spatial distribution of selected values."){#fig:sect_full width=100%}

![Details of two sectional diagrams illustrating spatial distribution of selected values (IQM of area, ID Theil index of area).](source/figures/a7/sect_det.pdf "Details of two sectional diagrams illustrating spatial distribution of selected values."){#fig:sect_det width=100%}

\newpage

## 7.4 Analysis of local central tendency characters {.unnumbered}
This appendix presents results of tests of different of measuring central tendency to better understand the differences between them. The aim is to select one (or more) to be used within the cluster analysis.

**Tested characters:**

- building area
- tessellation area
- height
- building circular compactness
- building solar orientation
- cell circular compactness
- CAR
- shared walls ratio

**Tested options:**

- mean
- interdecile mean
- interquartile mean
- median

Tested on 3 topological steps.

The aim is to identify such a method which is not prone to oulier effect but at the same time reflect the best true nature of each context.

\newpage
\thispagestyle{empty}

![Distributions of values measured using each tested option to capture local central tendency.](source/figures/a7/distributions.pdf "Distributions of values measured using each tested option to capture local central tendency."){#fig:avg_dist width=80%}

\newpage
\thispagestyle{empty}

![Mean deviations of measured primary characters compared to the central tendency value. The lower the deviation is, the better reflection of central tendecy the method offers. It is clear that mean deviates the most, while IQM and median are very similar.](source/figures/a7/deviations.pdf "Mean deviations of measured primary characters compared to the central tendency value."){#fig:avg_devs width=80%}


## 7.5 Comparison of characters capturing properties of distributions {.unnumbered}
Supplementary data for section 7.1.2.2.2.4. Figures below show spatial distribution (figures \ref{fig:area1} - \ref{fig:far2})and correlation (figures \ref{fig:corrarea}, \ref{fig:corrfar}) of selected characters capturing properties of distributions.

![Spatial distribution of characters capturing properties of distributions tested on area of a building.](source/figures/a7/area_1.png "Spatial distribution of characters capturing properties of distributions tested on area of a building."){#fig:area1 width=100%}

![Spatial distribution of characters capturing properties of distributions tested on area of a building (cont.).](source/figures/a7/area_2.png "Spatial distribution of characters capturing properties of distributions tested on area of a building (cont.)"){#fig:area2 width=100%}

![Spatial distribution of characters capturing properties of distributions tested on height of a building.](source/figures/a7/height_1.png "Spatial distribution of characters capturing properties of distributions tested on height of a building."){#fig:height_1 width=100%}

![Spatial distribution of characters capturing properties of distributions tested on height of a building (cont.).](source/figures/a7/height_2.png "Spatial distribution of characters capturing properties of distributions tested on height of a building (cont.)"){#fig:a7height_2 width=100%}

![Spatial distribution of characters capturing properties of distributions tested on coverage area ratio of tessellation cell.](source/figures/a7/car_1.png "Spatial distribution of characters capturing properties of distributions tested on coverage area ratio of tessellation cell."){#fig:car_1 width=100%}

![Spatial distribution of characters capturing properties of distributions tested on coverage area ratio of tessellation cell (cont.).](source/figures/a7/car_2.png "Spatial distribution of characters capturing properties of distributions tested on coverage area ratio of tessellation cell (cont.)"){#fig:car_2 width=100%}

![Spatial distribution of characters capturing properties of distributions tested on floor area ratio of tessellation cell.](source/figures/a7/far_1.png "Spatial distribution of characters capturing properties of distributions tested on floor area ratio of tessellation cell."){#fig:far1 width=100%}

![Spatial distribution of characters capturing properties of distributions tested on floor area ratio of tessellation cell (cont.).](source/figures/a7/far_2.png "Spatial distribution of characters capturing properties of distributions tested on floor area ratio of tessellation cell (cont.)"){#fig:far2 width=100%}

![Correlation of characters capturing properties of distributions tested on area of a building.](source/figures/a7/corr_area.pdf "Correlation of characters capturing properties of distributions tested on area of a building."){#fig:corrarea width=100%}

![Correlation of characters capturing properties of distributions tested on height of a building.](source/figures/a7/corr_height.pdf "Correlation of characters capturing properties of distributions tested on height of a building."){#fig:corrhei width=100%}

![Correlation of characters capturing properties of distributions tested on coverage area ratio of tessellation cell.](source/figures/a7/corr_car.pdf "Correlation of characters capturing properties of distributions tested on coverage area ratio of tessellation cell."){#fig:corrcar width=100%}

![Correlation of characters capturing properties of distributions tested on floor area ratio of tessellation cell.](source/figures/a7/corr_far.pdf "Correlation of characters capturing properties of distributions tested on floor area ratio of tessellation cell."){#fig:corrfar width=100%}

## 7.6 Spatial autocorrelation of morphometric characters {.unnumbered}

Results of assessment of spatial autocorrelation of morphometric characters. Values which show significant autocorrelation (Moran's I) tend to capture contiguous patterns.

See sections 7.1.2.1.1 and 7.1.3 for details.

**Primary characters**

|        |         I |   p_sim |   p_norm |
|:-------|----------:|--------:|---------:|
| lcdMes | 0.85362   |   0.001 |        0 |
| lcnClo | 0.862475  |   0.001 |        0 |
| ldbPWL | 0.592621  |   0.001 |        0 |
| lddARe | 0.798202  |   0.001 |        0 |
| lddNDe | 0.577277  |   0.001 |        0 |
| lddRea | 0.736014  |   0.001 |        0 |
| ldkAre | 0.731736  |   0.001 |        0 |
| ldkPer | 0.676249  |   0.001 |        0 |
| ldsCDL | 0.709263  |   0.001 |        0 |
| ldsMSL | 0.815984  |   0.001 |        0 |
| ldsRea | 0.810434  |   0.001 |        0 |
| libNCo | 0.710798  |   0.001 |        0 |
| licGDe | 0.938796  |   0.001 |        0 |
| likWBB | 0.655763  |   0.001 |        0 |
| linP3W | 0.852988  |   0.001 |        0 |
| linP4W | 0.911839  |   0.001 |        0 |
| linPDE | 0.815483  |   0.001 |        0 |
| linWID | 0.629364  |   0.001 |        0 |
| lskCCo | 0.533229  |   0.001 |        0 |
| lskCWA | 0.65397   |   0.001 |        0 |
| lskERI | 0.562295  |   0.001 |        0 |
| ltbIBD | 0.819981  |   0.001 |        0 |
| ltcBuA | 0.918511  |   0.001 |        0 |
| ltcWRB | 0.786888  |   0.001 |        0 |
| ltkOri | 0.607896  |   0.001 |        0 |
| ltkWNB | 0.729433  |   0.001 |        0 |
| mdcAre | 0.509591  |   0.001 |        0 |
| mdsAre | 0.780909  |   0.001 |        0 |
| midAre | 0.793405  |   0.001 |        0 |
| midRea | 0.664584  |   0.001 |        0 |
| misRea | 0.642062  |   0.001 |        0 |
| mtbAli | 0.302355  |   0.001 |        0 |
| mtbNDi | 0.319068  |   0.001 |        0 |
| mtbSWR | 0.387207  |   0.001 |        0 |
| mtcWNe | 0.43183   |   0.001 |        0 |
| mtdDeg | 0.338198  |   0.001 |        0 |
| mtdMDi | 0.699161  |   0.001 |        0 |
| sdbAre | 0.0909169 |   0.001 |        0 |
| sdbCoA | 0.0101648 |   0.001 |        0 |
| sdbHei | 0.508558  |   0.001 |        0 |
| sdbPer | 0.171366  |   0.001 |        0 |
| sdbVol | 0.101862  |   0.001 |        0 |
| sdcAre | 0.244891  |   0.001 |        0 |
| sdcLAL | 0.377011  |   0.001 |        0 |
| sddAre | 0.762546  |   0.001 |        0 |
| sdsAre | 0.736197  |   0.001 |        0 |
| sdsLen | 0.63461   |   0.001 |        0 |
| sdsSHD | 0.45782   |   0.001 |        0 |
| sdsSPH | 0.738876  |   0.001 |        0 |
| sdsSPO | 0.542333  |   0.001 |        0 |
| sdsSPR | 0.700646  |   0.001 |        0 |
| sdsSPW | 0.395235  |   0.001 |        0 |
| sdsSWD | 0.357013  |   0.001 |        0 |
| sicCAR | 0.510195  |   0.001 |        0 |
| sicFAR | 0.60611   |   0.001 |        0 |
| sisBpM | 0.153048  |   0.001 |        0 |
| ssbCCD | 0.0972815 |   0.001 |        0 |
| ssbCCM | 0.246668  |   0.001 |        0 |
| ssbCCo | 0.159506  |   0.001 |        0 |
| ssbCor | 0.101771  |   0.001 |        0 |
| ssbERI | 0.0928927 |   0.001 |        0 |
| ssbElo | 0.171279  |   0.001 |        0 |
| ssbFoF | 0.267186  |   0.001 |        0 |
| ssbSqu | 0.136881  |   0.001 |        0 |
| ssbVFR | 0.251518  |   0.001 |        0 |
| sscCCo | 0.152741  |   0.001 |        0 |
| sscERI | 0.0677793 |   0.001 |        0 |
| sssLin | 0.412019  |   0.001 |        0 |
| stbCeA | 0.0993836 |   0.001 |        0 |
| stbOri | 0.540843  |   0.001 |        0 |
| stbSAl | 0.285133  |   0.001 |        0 |
| stcOri | 0.291539  |   0.001 |        0 |
| stcSAl | 0.147622  |   0.001 |        0 |
| xcnSCl | 0.466779  |   0.001 |        0 |

Table: Global Moran's I spatial autocorrelation of primary characters. Key to character IDs is available in table A7.3. \label{moran_conx}


**Contextual characters**

|                 |        I |   p_sim |   p_norm |
|:----------------|---------:|--------:|---------:|
| lcdMes_meanIQ3  | 0.955598 |   0.001 |        0 |
| lcdMes_rangeIQ3 | 0.50685  |   0.001 |        0 |
| lcdMes_simpson  | 0.689865 |   0.001 |        0 |
| lcdMes_theilID3 | 0.681572 |   0.001 |        0 |
| lcnClo_meanIQ3  | 0.959075 |   0.001 |        0 |
| lcnClo_rangeIQ3 | 0.536619 |   0.001 |        0 |
| lcnClo_simpson  | 0.726854 |   0.001 |        0 |
| lcnClo_theilID3 | 0.658432 |   0.001 |        0 |
| ldbPWL_meanIQ3  | 0.940908 |   0.001 |        0 |
| ldbPWL_rangeIQ3 | 0.772736 |   0.001 |        0 |
| ldbPWL_simpson  | 0.877407 |   0.001 |        0 |
| ldbPWL_theilID3 | 0.652227 |   0.001 |        0 |
| lddARe_meanIQ3  | 0.950351 |   0.001 |        0 |
| lddARe_rangeIQ3 | 0.630399 |   0.001 |        0 |
| lddARe_simpson  | 0.814212 |   0.001 |        0 |
| lddARe_theilID3 | 0.62819  |   0.001 |        0 |
| lddNDe_meanIQ3  | 0.907499 |   0.001 |        0 |
| lddNDe_rangeIQ3 | 0.620502 |   0.001 |        0 |
| lddNDe_simpson  | 0.810196 |   0.001 |        0 |
| lddNDe_theilID3 | 0.675864 |   0.001 |        0 |
| lddRea_meanIQ3  | 0.931665 |   0.001 |        0 |
| lddRea_rangeIQ3 | 0.543221 |   0.001 |        0 |
| lddRea_simpson  | 0.674778 |   0.001 |        0 |
| lddRea_theilID3 | 0.66969  |   0.001 |        0 |
| ldkAre_meanIQ3  | 0.928541 |   0.001 |        0 |
| ldkAre_rangeIQ3 | 0.570235 |   0.001 |        0 |
| ldkAre_simpson  | 0.788347 |   0.001 |        0 |
| ldkAre_theilID3 | 0.522912 |   0.001 |        0 |
| ldkPer_meanIQ3  | 0.918906 |   0.001 |        0 |
| ldkPer_rangeIQ3 | 0.585438 |   0.001 |        0 |
| ldkPer_simpson  | 0.777687 |   0.001 |        0 |
| ldkPer_theilID3 | 0.597642 |   0.001 |        0 |
| ldsCDL_meanIQ3  | 0.921323 |   0.001 |        0 |
| ldsCDL_rangeIQ3 | 0.60509  |   0.001 |        0 |
| ldsCDL_simpson  | 0.810959 |   0.001 |        0 |
| ldsCDL_theilID3 | 0.534048 |   0.001 |        0 |
| ldsMSL_meanIQ3  | 0.944622 |   0.001 |        0 |
| ldsMSL_rangeIQ3 | 0.583908 |   0.001 |        0 |
| ldsMSL_simpson  | 0.799475 |   0.001 |        0 |
| ldsMSL_theilID3 | 0.615352 |   0.001 |        0 |
| ldsRea_meanIQ3  | 0.95118  |   0.001 |        0 |
| ldsRea_rangeIQ3 | 0.600647 |   0.001 |        0 |
| ldsRea_simpson  | 0.80886  |   0.001 |        0 |
| ldsRea_theilID3 | 0.618526 |   0.001 |        0 |
| libNCo_meanIQ3  | 0.949998 |   0.001 |        0 |
| libNCo_rangeIQ3 | 0.841513 |   0.001 |        0 |
| libNCo_simpson  | 0.909637 |   0.001 |        0 |
| libNCo_theilID3 | 0.561885 |   0.001 |        0 |
| licGDe_meanIQ3  | 0.976722 |   0.001 |        0 |
| licGDe_rangeIQ3 | 0.758523 |   0.001 |        0 |
| licGDe_simpson  | 0.845604 |   0.001 |        0 |
| licGDe_theilID3 | 0.60388  |   0.001 |        0 |
| likWBB_meanIQ3  | 0.904411 |   0.001 |        0 |
| likWBB_rangeIQ3 | 0.59347  |   0.001 |        0 |
| likWBB_simpson  | 0.803015 |   0.001 |        0 |
| likWBB_theilID3 | 0.599414 |   0.001 |        0 |
| linP3W_meanIQ3  | 0.962415 |   0.001 |        0 |
| linP3W_rangeIQ3 | 0.513581 |   0.001 |        0 |
| linP3W_simpson  | 0.690559 |   0.001 |        0 |
| linP3W_theilID3 | 0.56403  |   0.001 |        0 |
| linP4W_meanIQ3  | 0.976016 |   0.001 |        0 |
| linP4W_rangeIQ3 | 0.508686 |   0.001 |        0 |
| linP4W_simpson  | 0.71637  |   0.001 |        0 |
| linP4W_theilID3 | 0.646389 |   0.001 |        0 |
| linPDE_meanIQ3  | 0.95383  |   0.001 |        0 |
| linPDE_rangeIQ3 | 0.551748 |   0.001 |        0 |
| linPDE_simpson  | 0.827951 |   0.001 |        0 |
| linPDE_theilID3 | 0.627833 |   0.001 |        0 |
| linWID_meanIQ3  | 0.922797 |   0.001 |        0 |
| linWID_rangeIQ3 | 0.602441 |   0.001 |        0 |
| linWID_simpson  | 0.815416 |   0.001 |        0 |
| linWID_theilID3 | 0.595879 |   0.001 |        0 |
| lskCCo_meanIQ3  | 0.882728 |   0.001 |        0 |
| lskCCo_rangeIQ3 | 0.518586 |   0.001 |        0 |
| lskCCo_simpson  | 0.682315 |   0.001 |        0 |
| lskCCo_theilID3 | 0.714485 |   0.001 |        0 |
| lskCWA_meanIQ3  | 0.913762 |   0.001 |        0 |
| lskCWA_rangeIQ3 | 0.593642 |   0.001 |        0 |
| lskCWA_simpson  | 0.790063 |   0.001 |        0 |
| lskCWA_theilID3 | 0.568035 |   0.001 |        0 |
| lskERI_meanIQ3  | 0.897361 |   0.001 |        0 |
| lskERI_rangeIQ3 | 0.566972 |   0.001 |        0 |
| lskERI_simpson  | 0.671685 |   0.001 |        0 |
| lskERI_theilID3 | 0.785261 |   0.001 |        0 |
| ltbIBD_meanIQ3  | 0.916813 |   0.001 |        0 |
| ltbIBD_rangeIQ3 | 0.641772 |   0.001 |        0 |
| ltbIBD_simpson  | 0.760663 |   0.001 |        0 |
| ltbIBD_theilID3 | 0.619924 |   0.001 |        0 |
| ltcBuA_meanIQ3  | 0.961734 |   0.001 |        0 |
| ltcBuA_rangeIQ3 | 0.631009 |   0.001 |        0 |
| ltcBuA_simpson  | 0.79074  |   0.001 |        0 |
| ltcBuA_theilID3 | 0.725754 |   0.001 |        0 |
| ltcWRB_meanIQ3  | 0.915843 |   0.001 |        0 |
| ltcWRB_rangeIQ3 | 0.737241 |   0.001 |        0 |
| ltcWRB_simpson  | 0.850155 |   0.001 |        0 |
| ltcWRB_theilID3 | 0.609031 |   0.001 |        0 |
| ltkOri_meanIQ3  | 0.904165 |   0.001 |        0 |
| ltkOri_rangeIQ3 | 0.536899 |   0.001 |        0 |
| ltkOri_simpson  | 0.697909 |   0.001 |        0 |
| ltkOri_theilID3 | 0.68647  |   0.001 |        0 |
| ltkWNB_meanIQ3  | 0.928892 |   0.001 |        0 |
| ltkWNB_rangeIQ3 | 0.54861  |   0.001 |        0 |
| ltkWNB_simpson  | 0.74367  |   0.001 |        0 |
| ltkWNB_theilID3 | 0.60766  |   0.001 |        0 |
| mdcAre_meanIQ3  | 0.861546 |   0.001 |        0 |
| mdcAre_rangeIQ3 | 0.751638 |   0.001 |        0 |
| mdcAre_simpson  | 0.8328   |   0.001 |        0 |
| mdcAre_theilID3 | 0.574389 |   0.001 |        0 |
| mdsAre_meanIQ3  | 0.944663 |   0.001 |        0 |
| mdsAre_rangeIQ3 | 0.617205 |   0.001 |        0 |
| mdsAre_simpson  | 0.807483 |   0.001 |        0 |
| mdsAre_theilID3 | 0.57988  |   0.001 |        0 |
| midAre_meanIQ3  | 0.947303 |   0.001 |        0 |
| midAre_rangeIQ3 | 0.620141 |   0.001 |        0 |
| midAre_simpson  | 0.810922 |   0.001 |        0 |
| midAre_theilID3 | 0.586441 |   0.001 |        0 |
| midRea_meanIQ3  | 0.904878 |   0.001 |        0 |
| midRea_rangeIQ3 | 0.507217 |   0.001 |        0 |
| midRea_simpson  | 0.766685 |   0.001 |        0 |
| midRea_theilID3 | 0.610119 |   0.001 |        0 |
| misRea_meanIQ3  | 0.903812 |   0.001 |        0 |
| misRea_rangeIQ3 | 0.534213 |   0.001 |        0 |
| misRea_simpson  | 0.77369  |   0.001 |        0 |
| misRea_theilID3 | 0.604976 |   0.001 |        0 |
| mtbAli_meanIQ3  | 0.845607 |   0.001 |        0 |
| mtbAli_rangeIQ3 | 0.741485 |   0.001 |        0 |
| mtbAli_simpson  | 0.83494  |   0.001 |        0 |
| mtbAli_theilID3 | 0.676688 |   0.001 |        0 |
| mtbNDi_meanIQ3  | 0.855789 |   0.001 |        0 |
| mtbNDi_rangeIQ3 | 0.755206 |   0.001 |        0 |
| mtbNDi_simpson  | 0.846039 |   0.001 |        0 |
| mtbNDi_theilID3 | 0.729665 |   0.001 |        0 |
| mtbSWR_meanIQ3  | 0.920196 |   0.001 |        0 |
| mtbSWR_rangeIQ3 | 0.744766 |   0.001 |        0 |
| mtbSWR_simpson  | 0.839345 |   0.001 |        0 |
| mtbSWR_theilID3 | 0.642402 |   0.001 |        0 |
| mtcWNe_meanIQ3  | 0.869615 |   0.001 |        0 |
| mtcWNe_rangeIQ3 | 0.654455 |   0.001 |        0 |
| mtcWNe_simpson  | 0.75302  |   0.001 |        0 |
| mtcWNe_theilID3 | 0.682041 |   0.001 |        0 |
| mtdDeg_meanIQ3  | 0.835449 |   0.001 |        0 |
| mtdDeg_rangeIQ3 | 0.519432 |   0.001 |        0 |
| mtdDeg_simpson  | 0.705833 |   0.001 |        0 |
| mtdDeg_theilID3 | 0.723812 |   0.001 |        0 |
| mtdMDi_meanIQ3  | 0.925984 |   0.001 |        0 |
| mtdMDi_rangeIQ3 | 0.593588 |   0.001 |        0 |
| mtdMDi_simpson  | 0.806522 |   0.001 |        0 |
| mtdMDi_theilID3 | 0.588363 |   0.001 |        0 |
| sdbAre_meanIQ3  | 0.820124 |   0.001 |        0 |
| sdbAre_rangeIQ3 | 0.756028 |   0.001 |        0 |
| sdbAre_simpson  | 0.900207 |   0.001 |        0 |
| sdbAre_theilID3 | 0.743363 |   0.001 |        0 |
| sdbCoA_meanIQ3  | 0.676399 |   0.001 |        0 |
| sdbCoA_rangeIQ3 | 0.472574 |   0.001 |        0 |
| sdbCoA_simpson  | 0.902308 |   0.001 |        0 |
| sdbCoA_theilID3 | 0.74238  |   0.001 |        0 |
| sdbHei_meanIQ3  | 0.941584 |   0.001 |        0 |
| sdbHei_rangeIQ3 | 0.78105  |   0.001 |        0 |
| sdbHei_simpson  | 0.92606  |   0.001 |        0 |
| sdbHei_theilID3 | 0.756276 |   0.001 |        0 |
| sdbPer_meanIQ3  | 0.880991 |   0.001 |        0 |
| sdbPer_rangeIQ3 | 0.809868 |   0.001 |        0 |
| sdbPer_simpson  | 0.881562 |   0.001 |        0 |
| sdbPer_theilID3 | 0.770573 |   0.001 |        0 |
| sdbVol_meanIQ3  | 0.840984 |   0.001 |        0 |
| sdbVol_rangeIQ3 | 0.764246 |   0.001 |        0 |
| sdbVol_simpson  | 0.904012 |   0.001 |        0 |
| sdbVol_theilID3 | 0.708305 |   0.001 |        0 |
| sdcAre_meanIQ3  | 0.846201 |   0.001 |        0 |
| sdcAre_rangeIQ3 | 0.788472 |   0.001 |        0 |
| sdcAre_simpson  | 0.833662 |   0.001 |        0 |
| sdcAre_theilID3 | 0.64362  |   0.001 |        0 |
| sdcLAL_meanIQ3  | 0.858866 |   0.001 |        0 |
| sdcLAL_rangeIQ3 | 0.721431 |   0.001 |        0 |
| sdcLAL_simpson  | 0.823481 |   0.001 |        0 |
| sdcLAL_theilID3 | 0.657668 |   0.001 |        0 |
| sddAre_meanIQ3  | 0.937527 |   0.001 |        0 |
| sddAre_rangeIQ3 | 0.611057 |   0.001 |        0 |
| sddAre_simpson  | 0.806723 |   0.001 |        0 |
| sddAre_theilID3 | 0.548801 |   0.001 |        0 |
| sdsAre_meanIQ3  | 0.925027 |   0.001 |        0 |
| sdsAre_rangeIQ3 | 0.606761 |   0.001 |        0 |
| sdsAre_simpson  | 0.805935 |   0.001 |        0 |
| sdsAre_theilID3 | 0.524675 |   0.001 |        0 |
| sdsLen_meanIQ3  | 0.91244  |   0.001 |        0 |
| sdsLen_rangeIQ3 | 0.598489 |   0.001 |        0 |
| sdsLen_simpson  | 0.796079 |   0.001 |        0 |
| sdsLen_theilID3 | 0.576659 |   0.001 |        0 |
| sdsSHD_meanIQ3  | 0.891916 |   0.001 |        0 |
| sdsSHD_rangeIQ3 | 0.718592 |   0.001 |        0 |
| sdsSHD_simpson  | 0.876636 |   0.001 |        0 |
| sdsSHD_theilID3 | 0.68296  |   0.001 |        0 |
| sdsSPH_meanIQ3  | 0.954994 |   0.001 |        0 |
| sdsSPH_rangeIQ3 | 0.685786 |   0.001 |        0 |
| sdsSPH_simpson  | 0.885641 |   0.001 |        0 |
| sdsSPH_theilID3 | 0.659245 |   0.001 |        0 |
| sdsSPO_meanIQ3  | 0.910225 |   0.001 |        0 |
| sdsSPO_rangeIQ3 | 0.525057 |   0.001 |        0 |
| sdsSPO_simpson  | 0.715839 |   0.001 |        0 |
| sdsSPO_theilID3 | 0.773536 |   0.001 |        0 |
| sdsSPR_meanIQ3  | 0.964001 |   0.001 |        0 |
| sdsSPR_rangeIQ3 | 0.725299 |   0.001 |        0 |
| sdsSPR_simpson  | 0.889633 |   0.001 |        0 |
| sdsSPR_theilID3 | 0.64308  |   0.001 |        0 |
| sdsSPW_meanIQ3  | 0.879784 |   0.001 |        0 |
| sdsSPW_rangeIQ3 | 0.540892 |   0.001 |        0 |
| sdsSPW_simpson  | 0.695483 |   0.001 |        0 |
| sdsSPW_theilID3 | 0.683547 |   0.001 |        0 |
| sdsSWD_meanIQ3  | 0.859928 |   0.001 |        0 |
| sdsSWD_rangeIQ3 | 0.544153 |   0.001 |        0 |
| sdsSWD_simpson  | 0.706063 |   0.001 |        0 |
| sdsSWD_theilID3 | 0.683033 |   0.001 |        0 |
| sicCAR_meanIQ3  | 0.942188 |   0.001 |        0 |
| sicCAR_rangeIQ3 | 0.775051 |   0.001 |        0 |
| sicCAR_simpson  | 0.877473 |   0.001 |        0 |
| sicCAR_theilID3 | 0.771826 |   0.001 |        0 |
| sicFAR_meanIQ3  | 0.964149 |   0.001 |        0 |
| sicFAR_rangeIQ3 | 0.889602 |   0.001 |        0 |
| sicFAR_simpson  | 0.934126 |   0.001 |        0 |
| sicFAR_theilID3 | 0.74142  |   0.001 |        0 |
| sisBpM_meanIQ3  | 0.834023 |   0.001 |        0 |
| sisBpM_rangeIQ3 | 0.520404 |   0.001 |        0 |
| sisBpM_simpson  | 0.774814 |   0.001 |        0 |
| sisBpM_theilID3 | 0.593089 |   0.001 |        0 |
| ssbCCD_meanIQ3  | 0.849419 |   0.001 |        0 |
| ssbCCD_rangeIQ3 | 0.780761 |   0.001 |        0 |
| ssbCCD_simpson  | 0.84992  |   0.001 |        0 |
| ssbCCD_theilID3 | 0.813876 |   0.001 |        0 |
| ssbCCM_meanIQ3  | 0.889831 |   0.001 |        0 |
| ssbCCM_rangeIQ3 | 0.819487 |   0.001 |        0 |
| ssbCCM_simpson  | 0.881239 |   0.001 |        0 |
| ssbCCM_theilID3 | 0.78196  |   0.001 |        0 |
| ssbCCo_meanIQ3  | 0.864255 |   0.001 |        0 |
| ssbCCo_rangeIQ3 | 0.749751 |   0.001 |        0 |
| ssbCCo_simpson  | 0.788952 |   0.001 |        0 |
| ssbCCo_theilID3 | 0.790146 |   0.001 |        0 |
| ssbCor_meanIQ3  | 0.841669 |   0.001 |        0 |
| ssbCor_rangeIQ3 | 0.697948 |   0.001 |        0 |
| ssbCor_simpson  | 0.826181 |   0.001 |        0 |
| ssbCor_theilID3 | 0.688075 |   0.001 |        0 |
| ssbERI_meanIQ3  | 0.856649 |   0.001 |        0 |
| ssbERI_rangeIQ3 | 0.808194 |   0.001 |        0 |
| ssbERI_simpson  | 0.812285 |   0.001 |        0 |
| ssbERI_theilID3 | 0.848991 |   0.001 |        0 |
| ssbElo_meanIQ3  | 0.864312 |   0.001 |        0 |
| ssbElo_rangeIQ3 | 0.698684 |   0.001 |        0 |
| ssbElo_simpson  | 0.765896 |   0.001 |        0 |
| ssbElo_theilID3 | 0.791906 |   0.001 |        0 |
| ssbFoF_meanIQ3  | 0.893053 |   0.001 |        0 |
| ssbFoF_rangeIQ3 | 0.777009 |   0.001 |        0 |
| ssbFoF_simpson  | 0.857507 |   0.001 |        0 |
| ssbFoF_theilID3 | 0.805237 |   0.001 |        0 |
| ssbSqu_meanIQ3  | 0.89365  |   0.001 |        0 |
| ssbSqu_rangeIQ3 | 0.827903 |   0.001 |        0 |
| ssbSqu_simpson  | 0.873586 |   0.001 |        0 |
| ssbSqu_theilID3 | 0.659983 |   0.001 |        0 |
| ssbVFR_meanIQ3  | 0.892769 |   0.001 |        0 |
| ssbVFR_rangeIQ3 | 0.777149 |   0.001 |        0 |
| ssbVFR_simpson  | 0.876502 |   0.001 |        0 |
| ssbVFR_theilID3 | 0.772907 |   0.001 |        0 |
| sscCCo_meanIQ3  | 0.837064 |   0.001 |        0 |
| sscCCo_rangeIQ3 | 0.633735 |   0.001 |        0 |
| sscCCo_simpson  | 0.730701 |   0.001 |        0 |
| sscCCo_theilID3 | 0.781972 |   0.001 |        0 |
| sscERI_meanIQ3  | 0.814612 |   0.001 |        0 |
| sscERI_rangeIQ3 | 0.691816 |   0.001 |        0 |
| sscERI_simpson  | 0.720924 |   0.001 |        0 |
| sscERI_theilID3 | 0.75613  |   0.001 |        0 |
| sssLin_meanIQ3  | 0.834239 |   0.001 |        0 |
| sssLin_rangeIQ3 | 0.626923 |   0.001 |        0 |
| sssLin_simpson  | 0.815024 |   0.001 |        0 |
| sssLin_theilID3 | 0.731798 |   0.001 |        0 |
| stbCeA_meanIQ3  | 0.833449 |   0.001 |        0 |
| stbCeA_rangeIQ3 | 0.75756  |   0.001 |        0 |
| stbCeA_simpson  | 0.838166 |   0.001 |        0 |
| stbCeA_theilID3 | 0.784623 |   0.001 |        0 |
| stbOri_meanIQ3  | 0.909016 |   0.001 |        0 |
| stbOri_rangeIQ3 | 0.639928 |   0.001 |        0 |
| stbOri_simpson  | 0.797732 |   0.001 |        0 |
| stbOri_theilID3 | 0.752463 |   0.001 |        0 |
| stbSAl_meanIQ3  | 0.844173 |   0.001 |        0 |
| stbSAl_rangeIQ3 | 0.694922 |   0.001 |        0 |
| stbSAl_simpson  | 0.827305 |   0.001 |        0 |
| stbSAl_theilID3 | 0.61161  |   0.001 |        0 |
| stcOri_meanIQ3  | 0.890039 |   0.001 |        0 |
| stcOri_rangeIQ3 | 0.696291 |   0.001 |        0 |
| stcOri_simpson  | 0.795035 |   0.001 |        0 |
| stcOri_theilID3 | 0.805094 |   0.001 |        0 |
| stcSAl_meanIQ3  | 0.832939 |   0.001 |        0 |
| stcSAl_rangeIQ3 | 0.719319 |   0.001 |        0 |
| stcSAl_simpson  | 0.821816 |   0.001 |        0 |
| stcSAl_theilID3 | 0.739995 |   0.001 |        0 |
| xcnSCl_meanIQ3  | 0.838289 |   0.001 |        0 |
| xcnSCl_rangeIQ3 | 0.592369 |   0.001 |        0 |
| xcnSCl_simpson  | 0.780986 |   0.001 |        0 |
| xcnSCl_theilID3 | 0.422105 |   0.001 |        0 |

Table: Global Moran's I spatial autocorrelation of contextual characters. Key to character IDs is available in table A7.3. \label{moran_conx}

## 7.7 Statistical overview of contextual characters results {.unnumbered}

### Interquartile mean {.unnumbered}

|                |         mean |          std |         min |          25% |          50% |          75% |          max |
|:---------------|-------------:|-------------:|------------:|-------------:|-------------:|-------------:|-------------:|
| stcOri |     18       |      6.8     |     0.12    |     13       |     18       |     23       |     42       |
| sdcLAL |     69       |     25       |    25       |     51       |     64       |     82       |    310       |
| sdcAre |   2400       |   2100       |   180       |   1100       |   1700       |   2900       |  50000       |
| sscCCo |      0.45    |      0.055   |     0.14    |      0.42    |      0.46    |      0.49    |      0.74    |
| sscERI |      0.97    |      0.018   |     0.86    |      0.96    |      0.97    |      0.98    |      1.1     |
| stcSAl |      9.3     |      3.7     |     0.12    |      6.7     |      9       |     12       |     36       |
| sicCAR |      0.19    |      0.1     |     0.0022  |      0.13    |      0.16    |      0.21    |      0.73    |
| sicFAR |      0.66    |      0.7     |     0.0022  |      0.25    |      0.39    |      0.73    |      4.4     |
| mtcWNe |      0.045   |      0.013   |     0.0016  |      0.036   |      0.045   |      0.054   |      0.15    |
| mdcAre |  18000       |  14000       |  1600       |   8700       |  14000       |  22000       | 370000       |
| licGDe |      0.57    |      0.64    |     0.0022  |      0.2     |      0.36    |      0.65    |      4.1     |
| ltcWRB |      8.8e-05 |      5.6e-05 |     2.7e-06 |      4.6e-05 |      7.8e-05 |      0.00012 |      0.00048 |
| sdbHei |      9.9     |      4.7     |     3       |      6.3     |      8.1     |     12       |     37       |
| sdbAre |    310       |    330       |    33       |    130       |    200       |    360       |  10000       |
| sdbVol |   3800       |   4600       |   130       |    910       |   2000       |   5100       | 150000       |
| sdbPer |     68       |     26       |    24       |     49       |     60       |     79       |    460       |
| sdbCoA |      3.3     |     15       |     0       |      0       |      0       |      0       |    340       |
| ssbFoF |      1.4     |      0.3     |     0.73    |      1.2     |      1.4     |      1.6     |      4.8     |
| ssbVFR |      3.1     |      0.9     |     1.4     |      2.5     |      2.9     |      3.7     |     19       |
| ssbCCo |      0.53    |      0.044   |     0.27    |      0.5     |      0.53    |      0.56    |      0.72    |
| ssbCor |      9.2     |      2.7     |     4       |      7.5     |      8.6     |     10       |     54       |
| ssbSqu |      5.4     |      3.5     |     0.016   |      2.9     |      4.5     |      7.1     |     39       |
| ssbERI |      0.93    |      0.03    |     0.7     |      0.92    |      0.94    |      0.95    |      1.1     |
| ssbElo |      0.7     |      0.085   |     0.23    |      0.65    |      0.72    |      0.76    |      0.96    |
| ssbCCM |      9.8     |      3.5     |     3.8     |      7.3     |      8.9     |     11       |     59       |
| ssbCCD |      1.7     |      0.81    |     0.00036 |      1.1     |      1.5     |      2       |     16       |
| stbOri |     16       |      8.8     |     0.026   |      9.8     |     15       |     22       |     44       |
| stbSAl |      6.8     |      4.5     |     0.038   |      3.3     |      6.1     |      9.3     |     39       |
| stbCeA |      7       |      3       |     0.058   |      4.8     |      6.8     |      9       |     27       |
| mtbSWR |      0.17    |      0.12    |     0       |      0.077   |      0.14    |      0.25    |      0.75    |
| mtbAli |      4.9     |      2.7     |     0.005   |      2.8     |      4.7     |      6.7     |     38       |
| mtbNDi |     26       |     10       |     0       |     19       |     25       |     32       |    120       |
| libNCo |      0.59    |      2.7     |     0       |      0       |      0       |      0.049   |     51       |
| ldbPWL |    180       |    190       |    24       |     69       |    110       |    210       |   2100       |
| ltbIBD |     27       |      9.7     |     0       |     21       |     26       |     33       |    120       |
| ltcBuA |      0.65    |      0.22    |     0.083   |      0.5     |      0.69    |      0.82    |      1       |
| mtdDeg |      3.1     |      0.44    |     1       |      2.9     |      3.1     |      3.4     |      4.8     |
| lcdMes |      0.15    |      0.054   |    -0.23    |      0.11    |      0.15    |      0.19    |      0.32    |
| linP3W |      0.64    |      0.1     |     0       |      0.57    |      0.64    |      0.71    |      0.93    |
| linP4W |      0.23    |      0.11    |     0       |      0.15    |      0.22    |      0.3     |      0.72    |
| linPDE |      0.13    |      0.077   |     0       |      0.072   |      0.11    |      0.17    |      1       |
| lcnClo |      5.3e-06 |      2.3e-06 |     6.8e-08 |      3.6e-06 |      5.1e-06 |      6.7e-06 |      1.7e-05 |
| ldsCDL |    280       |    310       |     0       |     78       |    190       |    370       |   3600       |
| xcnSCl |      0.056   |      0.055   |     0       |      0.012   |      0.046   |      0.083   |      0.75    |
| mtdMDi |    170       |    120       |    36       |    110       |    140       |    190       |   3300       |
| lddNDe |      0.013   |      0.004   |     0.0028  |      0.01    |      0.012   |      0.014   |      0.063   |
| linWID |      0.025   |      0.0079  |     0       |      0.02    |      0.024   |      0.029   |      0.11    |
| lddRea |    190       |     71       |     2       |    140       |    190       |    230       |    630       |
| lddARe | 370000       | 270000       | 39000       | 230000       | 300000       | 410000       |      3.8e+06 |
| sddAre |  30000       |  39000       |  3000       |  12000       |  19000       |  32000       | 660000       |
| midRea |     52       |     22       |     2       |     38       |     49       |     62       |    270       |
| midAre |  97000       |  96000       | 12000       |  51000       |  70000       | 110000       |      1.2e+06 |
| sdsLen |    230       |    200       |    36       |    140       |    180       |    260       |   3300       |
| sdsSPW |     29       |      5       |    11       |     26       |     29       |     32       |     50       |
| sdsSPH |     10       |      5.1     |     0       |      6.6     |      8.5     |     13       |     38       |
| sdsSPR |      0.41    |      0.27    |     0       |      0.24    |      0.31    |      0.47    |      2       |
| sdsSPO |      0.58    |      0.14    |     0.027   |      0.5     |      0.58    |      0.66    |      1       |
| sdsSWD |      3.6     |      1.2     |     0       |      2.8     |      3.6     |      4.4     |      9.8     |
| sdsSHD |      2.3     |      1.5     |     0       |      1.2     |      1.8     |      2.9     |     14       |
| sssLin |      0.95    |      0.077   |     0       |      0.93    |      0.97    |      0.99    |      1       |
| sdsAre |  31000       |  46000       |  2100       |  10000       |  17000       |  32000       | 740000       |
| sisBpM |      0.074   |      0.031   |     0.0013  |      0.056   |      0.07    |      0.086   |      0.79    |
| misRea |     44       |     19       |     2       |     32       |     40       |     52       |    230       |
| mdsAre |  86000       |  92000       |  8600       |  41000       |  59000       |  95000       |      1.1e+06 |
| ldsMSL |    150       |     67       |    57       |    110       |    140       |    170       |   1200       |
| ldsRea | 350000       | 270000       | 39000       | 220000       | 280000       | 390000       |      3.8e+06 |
| ldkAre | 120000       | 200000       |  3200       |  26000       |  56000       | 130000       |      2e+06   |
| ldkPer |   1500       |   1400       |   250       |    720       |   1100       |   1800       |  13000       |
| lskCCo |      0.43    |      0.09    |     0.13    |      0.37    |      0.43    |      0.5     |      0.98    |
| lskERI |      0.86    |      0.096   |     0.36    |      0.81    |      0.88    |      0.93    |      1.1     |
| lskCWA |    370       |    370       |     0.43    |    140       |    240       |    450       |   3100       |
| ltkOri |     18       |      9.4     |     0.034   |     10       |     17       |     25       |     45       |
| ltkWNB |      0.0074  |      0.0035  |     0       |      0.0047  |      0.0071  |      0.0097  |      0.025   |
| likWBB |      0.00088 |      0.00051 |     3e-05   |      0.00051 |      0.0008  |      0.0012  |      0.004   |

Table: Overview of the contextual morphometric values of interquartile mean for the whole case study. Key to character IDs is available in table A7.3. \label{meanIQ3_chars}

![Histograms of interquartile mean for characters 1-15 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_15__meanIQ3.pdf "Histograms of contextual characters 1-15"){#fig:conxdistplot1 width=100%}

![Histograms of interquartile mean for characters 16-30 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_30__meanIQ3.pdf "Histograms of contextual characters 16-30"){#fig:conxdistplot2 width=100%}

![Histograms of interquartile mean for characters 31-45 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_45__meanIQ3.pdf "Histograms of contextual characters 31-45"){#fig:conxdistplot3 width=100%}

![Histograms of interquartile mean for characters 46-60 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_60__meanIQ3.pdf "Histograms of contextual characters 46-60"){#fig:conxdistplot4 width=100%}

![Histograms of interquartile mean for characters 61-74 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_74__meanIQ3.pdf "Histograms of contextual characters 61-74"){#fig:conxdistplot5 width=100%}

### Interquartile range {.unnumbered}
|                 |         mean |          std |     min |         25% |         50% |          75% |          max |
|:----------------|-------------:|-------------:|--------:|------------:|------------:|-------------:|-------------:|
| stcOri |     14       |      7.4     | 0.013   |     8.8     |    14       |     19       |     45       |
| sdcLAL |     36       |     23       | 0.045   |    17       |    30       |     51       |    160       |
| sdcAre |   1800       |   2000       | 3.7     |   590       |  1100       |   2200       |  47000       |
| sscCCo |      0.19    |      0.052   | 0.00011 |     0.15    |     0.18    |      0.22    |      0.5     |
| sscERI |      0.069   |      0.022   | 0.00024 |     0.054   |     0.067   |      0.081   |      0.27    |
| stcSAl |     11       |      5.4     | 0.013   |     7.2     |    10       |     14       |     41       |
| sicCAR |      0.13    |      0.062   | 2e-05   |     0.083   |     0.11    |      0.15    |      0.62    |
| sicFAR |      0.56    |      0.56    | 2e-05   |     0.19    |     0.32    |      0.73    |      3.8     |
| mtcWNe |      0.021   |      0.0089  | 7.8e-07 |     0.015   |     0.02    |      0.025   |      0.15    |
| mdcAre |  13000       |  13000       | 0       |  4500       |  9300       |  18000       | 290000       |
| licGDe |      0.19    |      0.22    | 0       |     0.062   |     0.12    |      0.24    |      2.4     |
| ltcWRB |      4e-05   |      3.1e-05 | 0       |     1.8e-05 |     3.3e-05 |      5.4e-05 |      0.00038 |
| sdbHei |      5       |      4.9     | 0       |     2       |     3.1     |      6.1     |     42       |
| sdbAre |    170       |    250       | 0.097   |    57       |    96       |    180       |  17000       |
| sdbVol |   2400       |   3300       | 2.1     |   480       |  1100       |   3500       | 170000       |
| sdbPer |     28       |     26       | 0.018   |    13       |    20       |     32       |    420       |
| sdbCoA |      0.096   |      2       | 0       |     0       |     0       |      0       |    160       |
| ssbFoF |      0.47    |      0.29    | 0.00044 |     0.28    |     0.39    |      0.58    |      4.2     |
| ssbVFR |      1.1     |      0.84    | 0.0029  |     0.58    |     0.86    |      1.4     |     21       |
| ssbCCo |      0.13    |      0.054   | 0.00027 |     0.086   |     0.12    |      0.16    |      0.37    |
| ssbCor |      5.6     |      2.9     | 0       |     4       |     5.2     |      6.8     |     76       |
| ssbSqu |      5.7     |      6       | 0.001   |     1.1     |     2.4     |      9.9     |     45       |
| ssbERI |      0.087   |      0.046   | 1.6e-05 |     0.059   |     0.079   |      0.1     |      0.44    |
| ssbElo |      0.26    |      0.09    | 0.00025 |     0.2     |     0.26    |      0.32    |      0.69    |
| ssbCCM |      3.7     |      3.7     | 0.0029  |     1.6     |     2.5     |      4.2     |     57       |
| ssbCCD |      1.7     |      1.1     | 0.00014 |     1       |     1.5     |      2.1     |     22       |
| stbOri |      9.8     |      8.8     | 7.3e-09 |     2.3     |     7.6     |     15       |     45       |
| stbSAl |      7.9     |      6.7     | 2.5e-08 |     2.5     |     6.4     |     11       |     42       |
| stbCeA |      8.8     |      4.7     | 0.015   |     5.3     |     8.5     |     12       |     43       |
| mtbSWR |      0.2     |      0.13    | 0       |     0.12    |     0.21    |      0.28    |      0.9     |
| mtbAli |      4.7     |      2.8     | 0       |     2.6     |     4.6     |      6.5     |     24       |
| mtbNDi |     15       |      9.4     | 0       |     8.6     |    13       |     20       |     82       |
| libNCo |      0.62    |      3.2     | 0       |     0       |     0       |      0       |     52       |
| ldbPWL |    130       |    220       | 0       |    28       |    62       |    140       |   3200       |
| ltbIBD |      6.6     |      4.2     | 0       |     3.5     |     5.7     |      8.7     |     49       |
| ltcBuA |      0.1     |      0.061   | 0       |     0.057   |     0.085   |      0.13    |      0.62    |
| mtdDeg |      0.6     |      0.73    | 0       |     0       |     0       |      1       |      4       |
| lcdMes |      0.029   |      0.024   | 0       |     0.013   |     0.024   |      0.038   |      0.47    |
| linP3W |      0.051   |      0.046   | 0       |     0.024   |     0.043   |      0.067   |      0.8     |
| linP4W |      0.044   |      0.037   | 0       |     0.02    |     0.036   |      0.059   |      0.46    |
| linPDE |      0.039   |      0.045   | 0       |     0.016   |     0.03    |      0.05    |      0.97    |
| lcnClo |      1.2e-06 |      9.1e-07 | 0       |     5.5e-07 |     1e-06   |      1.7e-06 |      7e-06   |
| ldsCDL |    200       |    290       | 0       |    11       |   110       |    260       |   4100       |
| xcnSCl |      0.056   |      0.074   | 0       |     0       |     0.04    |      0.08    |      1       |
| mtdMDi |     74       |     98       | 0       |    21       |    43       |     87       |   1500       |
| lddNDe |      0.0028  |      0.0038  | 0       |     0.00098 |     0.0019  |      0.0035  |      0.096   |
| linWID |      0.0055  |      0.0065  | 0       |     0.002   |     0.0039  |      0.0069  |      0.15    |
| lddRea |     56       |     44       | 0       |    25       |    46       |     76       |    480       |
| lddARe | 140000       | 180000       | 0       | 42000       | 89000       | 170000       |      3.7e+06 |
| sddAre |  20000       |  31000       | 0       |  4400       |  9700       |  22000       | 590000       |
| midRea |     22       |     17       | 0       |    10       |    18       |     29       |    220       |
| midAre |  49000       |  66000       | 0       | 14000       | 28000       |  56000       | 900000       |
| sdsLen |    140       |    190       | 0       |    44       |    85       |    160       |   2900       |
| sdsSPW |      8.9     |      5.3     | 0       |     4.8     |     8.8     |     13       |     36       |
| sdsSPH |      2.9     |      3.5     | 0       |     0.77    |     1.6     |      3.7     |     38       |
| sdsSPR |      0.18    |      0.17    | 0       |     0.063   |     0.12    |      0.23    |      2.2     |
| sdsSPO |      0.19    |      0.11    | 0       |     0.11    |     0.18    |      0.26    |      0.91    |
| sdsSWD |      2.3     |      1.3     | 0       |     1.3     |     2.2     |      3.1     |      8.7     |
| sdsSHD |      1.7     |      2       | 0       |     0.53    |     1       |      2.1     |     20       |
| sssLin |      0.073   |      0.13    | 0       |     0       |     0.011   |      0.09    |      1       |
| sdsAre |  23000       |  40000       | 0       |  4900       | 11000       |  25000       | 710000       |
| sisBpM |      0.039   |      0.029   | 0       |     0.021   |     0.034   |      0.051   |      0.92    |
| misRea |     19       |     16       | 0       |     9       |    16       |     25       |    180       |
| mdsAre |  46000       |  67000       | 0       | 12000       | 25000       |  53000       | 970000       |
| ldsMSL |     31       |     43       | 0       |     8       |    17       |     36       |   1100       |
| ldsRea | 130000       | 170000       | 0       | 40000       | 80000       | 160000       |      2.9e+06 |
| ldkAre |  98000       | 200000       | 0       |  5300       | 21000       |  96000       |      2e+06   |
| ldkPer |    940       |   1500       | 0       |    98       |   340       |   1100       |  13000       |
| lskCCo |      0.12    |      0.095   | 0       |     0.042   |     0.1     |      0.18    |      0.56    |
| lskERI |      0.11    |      0.11    | 0       |     0.031   |     0.08    |      0.16    |      0.65    |
| lskCWA |    270       |    410       | 0       |    30       |   100       |    340       |   3000       |
| ltkOri |      9.9     |      9.5     | 0       |     2.3     |     6.9     |     15       |     45       |
| ltkWNB |      0.0028  |      0.0024  | 0       |     0.00085 |     0.0023  |      0.0041  |      0.019   |
| likWBB |      0.00049 |      0.00048 | 0       |     0.00014 |     0.00037 |      0.0007  |      0.0053  |

Table: Overview of the contextual morphometric values of interquartile range for the whole case study. Key to character IDs is available in table A7.3. \label{rangeIQ3_chars}

![Histograms of interquartile range for characters 1-15 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_15__rangeIQ3.pdf "Histograms of contextual characters 1-15 (range)"){#fig:conxdistplot1range width=100%}

![Histograms of interquartile range for characters 16-30 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_30__rangeIQ3.pdf "Histograms of contextual characters 16-30 (range)"){#fig:conxdistplot2range width=100%}

![Histograms of interquartile range for characters 31-45 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_45__rangeIQ3.pdf "Histograms of contextual characters 31-45 (range)"){#fig:conxdistplot3range width=100%}

![Histograms of interquartile range for characters 46-60 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_60__rangeIQ3.pdf "Histograms of contextual characters 46-60 (range)"){#fig:conxdistplot4range width=100%}

![Histograms of interquartile range for characters 61-74 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_74__rangeIQ3.pdf "Histograms of contextual characters 61-74 (range)"){#fig:conxdistplot5range width=100%}

### Interdecile Theil index {.unnumbered}
|                 |    mean |    std |      min |     25% |     50% |     75% |   max |
|:----------------|--------:|-------:|---------:|--------:|--------:|--------:|------:|
| stcOri | 0.14    | 0.13   |  8.3e-08 | 0.059   | 0.11    | 0.19    | 2.2   |
| sdcLAL | 0.046   | 0.033  |  2e-08   | 0.02    | 0.039   | 0.066   | 0.27  |
| sdcAre | 0.18    | 0.12   |  1.7e-07 | 0.085   | 0.15    | 0.24    | 1.6   |
| sscCCo | 0.027   | 0.022  |  1.3e-08 | 0.014   | 0.021   | 0.032   | 0.41  |
| sscERI | 0.00078 | 0.0005 |  2.5e-08 | 0.00047 | 0.00067 | 0.00096 | 0.023 |
| stcSAl | 0.32    | 0.16   |  1e-06   | 0.21    | 0.29    | 0.4     | 2.4   |
| sicCAR | 0.093   | 0.072  |  1e-06   | 0.043   | 0.073   | 0.12    | 0.78  |
| sicFAR | 0.16    | 0.11   |  1e-06   | 0.084   | 0.14    | 0.22    | 1.2   |
| mtcWNe | 0.037   | 0.029  |  1.2e-07 | 0.017   | 0.029   | 0.049   | 0.39  |
| mdcAre | 0.11    | 0.082  |  0       | 0.048   | 0.084   | 0.14    | 1     |
| licGDe | 0.026   | 0.032  | -1.1e-16 | 0.0073  | 0.017   | 0.034   | 0.75  |
| ltcWRB | 0.038   | 0.036  | -2.2e-16 | 0.014   | 0.026   | 0.049   | 0.47  |
| sdbHei | 0.044   | 0.046  |  0       | 0.015   | 0.027   | 0.056   | 0.51  |
| sdbAre | 0.12    | 0.12   |  2.5e-07 | 0.04    | 0.073   | 0.15    | 1.5   |
| sdbVol | 0.18    | 0.17   |  2.5e-07 | 0.064   | 0.13    | 0.25    | 2.1   |
| sdbPer | 0.04    | 0.042  |  1.6e-08 | 0.014   | 0.024   | 0.05    | 0.47  |
| sdbCoA | 0.041   | 0.34   | -1.1e-16 | 0       | 0       | 0       | 4.7   |
| ssbFoF | 0.023   | 0.025  |  2.8e-08 | 0.0075  | 0.013   | 0.029   | 0.34  |
| ssbVFR | 0.024   | 0.025  |  2.2e-07 | 0.0093  | 0.016   | 0.03    | 0.39  |
| ssbCCo | 0.01    | 0.0082 |  1.3e-07 | 0.004   | 0.0077  | 0.014   | 0.097 |
| ssbCor | 0.087   | 0.045  | -1.1e-16 | 0.06    | 0.079   | 0.1     | 0.8   |
| ssbSqu | 0.54    | 0.27   |  0.00012 | 0.33    | 0.53    | 0.71    | 2.2   |
| ssbERI | 0.0017  | 0.0021 |  4.2e-11 | 0.00063 | 0.0011  | 0.0019  | 0.032 |
| ssbElo | 0.022   | 0.016  |  5.9e-07 | 0.01    | 0.018   | 0.03    | 0.19  |
| ssbCCM | 0.031   | 0.036  |  9.4e-09 | 0.0087  | 0.017   | 0.038   | 0.41  |
| ssbCCD | 0.38    | 0.28   |  3.4e-07 | 0.19    | 0.3     | 0.48    | 2.7   |
| stbOri | 0.13    | 0.18   |  4.4e-09 | 0.017   | 0.075   | 0.17    | 3.6   |
| stbSAl | 0.4     | 0.24   |  6.1e-07 | 0.23    | 0.35    | 0.52    | 3     |
| stbCeA | 0.48    | 0.22   |  6.3e-07 | 0.33    | 0.45    | 0.6     | 2.4   |
| mtbSWR | 0.88    | 0.78   | -1.1e-16 | 0.3     | 0.69    | 1.3     | 4.3   |
| mtbAli | 0.22    | 0.17   |  0       | 0.11    | 0.18    | 0.29    | 2.3   |
| mtbNDi | 0.065   | 0.051  |  0       | 0.031   | 0.052   | 0.085   | 0.67  |
| libNCo | 0.14    | 0.43   | -1.1e-16 | 0       | 0       | 0       | 4.6   |
| ldbPWL | 0.11    | 0.11   | -2.2e-16 | 0.03    | 0.07    | 0.15    | 1.2   |
| ltbIBD | 0.01    | 0.012  | -2.2e-16 | 0.0031  | 0.0066  | 0.013   | 0.28  |
| ltcBuA | 0.0073  | 0.011  |  0       | 0.001   | 0.0029  | 0.0085  | 0.15  |
| mtdDeg | 0.029   | 0.04   | -1.1e-16 | 0.005   | 0.0095  | 0.049   | 0.27  |
| lcdMes | 0.024   | 0.096  | -5.6e-16 | 0.0021  | 0.0056  | 0.015   | 3.3   |
| linP3W | 0.0038  | 0.044  | -6.7e-16 | 0.00042 | 0.00095 | 0.002   | 3.9   |
| linP4W | 0.038   | 0.16   | -6.7e-16 | 0.0022  | 0.0058  | 0.016   | 3.9   |
| linPDE | 0.073   | 0.22   | -4.4e-16 | 0.0065  | 0.017   | 0.046   | 3.9   |
| lcnClo | 0.02    | 0.041  | -6.7e-16 | 0.0031  | 0.0088  | 0.023   | 1.6   |
| ldsCDL | 0.38    | 0.51   | -6.7e-16 | 0.038   | 0.17    | 0.51    | 4.3   |
| xcnSCl | 0.54    | 0.65   | -4.4e-16 | 0.008   | 0.31    | 0.84    | 4.7   |
| mtdMDi | 0.045   | 0.06   | -5.6e-16 | 0.0099  | 0.025   | 0.057   | 0.96  |
| lddNDe | 0.017   | 0.044  | -6.7e-16 | 0.0022  | 0.0058  | 0.015   | 1.5   |
| linWID | 0.017   | 0.056  | -5.6e-16 | 0.0024  | 0.0061  | 0.015   | 3.9   |
| lddRea | 0.029   | 0.039  | -1.1e-16 | 0.0052  | 0.014   | 0.037   | 0.94  |
| lddARe | 0.043   | 0.06   | -5.6e-16 | 0.0079  | 0.022   | 0.053   | 0.97  |
| sddAre | 0.11    | 0.11   | -6.7e-16 | 0.036   | 0.078   | 0.15    | 1.2   |
| midRea | 0.046   | 0.047  | -1.1e-16 | 0.015   | 0.032   | 0.063   | 0.71  |
| midAre | 0.067   | 0.077  | -6.7e-16 | 0.018   | 0.042   | 0.088   | 1.1   |
| sdsLen | 0.083   | 0.09   | -6.7e-16 | 0.027   | 0.056   | 0.11    | 1.1   |
| sdsSPW | 0.022   | 0.019  | -5.6e-16 | 0.0087  | 0.018   | 0.03    | 0.25  |
| sdsSPH | 0.03    | 0.082  | -5.6e-16 | 0.0026  | 0.0076  | 0.025   | 3     |
| sdsSPR | 0.049   | 0.084  | -6.7e-16 | 0.013   | 0.028   | 0.054   | 3.7   |
| sdsSPO | 0.033   | 0.049  | -6.7e-16 | 0.0092  | 0.02    | 0.039   | 1.5   |
| sdsSWD | 0.13    | 0.15   | -6.7e-16 | 0.034   | 0.084   | 0.18    | 3.7   |
| sdsSHD | 0.16    | 0.19   | -5.6e-16 | 0.038   | 0.091   | 0.21    | 3.7   |
| sssLin | 0.009   | 0.044  | -5.6e-16 | 0       | 0.00033 | 0.0043  | 2     |
| sdsAre | 0.15    | 0.14   | -6.7e-16 | 0.059   | 0.11    | 0.2     | 1.5   |
| sisBpM | 0.061   | 0.056  | -6.7e-16 | 0.025   | 0.047   | 0.08    | 1.1   |
| misRea | 0.049   | 0.049  | -1.1e-16 | 0.016   | 0.034   | 0.067   | 0.6   |
| mdsAre | 0.079   | 0.089  | -5.6e-16 | 0.021   | 0.049   | 0.1     | 1     |
| ldsMSL | 0.012   | 0.025  | -5.6e-16 | 0.0012  | 0.0039  | 0.011   | 0.35  |
| ldsRea | 0.042   | 0.061  | -5.6e-16 | 0.0072  | 0.021   | 0.051   | 0.96  |
| ldkAre | 0.22    | 0.25   | -6.7e-16 | 0.04    | 0.13    | 0.32    | 1.9   |
| ldkPer | 0.1     | 0.13   | -6.7e-16 | 0.013   | 0.053   | 0.15    | 1     |
| lskCCo | 0.023   | 0.028  | -6.7e-16 | 0.0048  | 0.014   | 0.032   | 0.31  |
| lskERI | 0.0063  | 0.011  | -6.7e-16 | 0.00058 | 0.0022  | 0.0072  | 0.12  |
| lskCWA | 0.16    | 0.18   | -6.7e-16 | 0.034   | 0.1     | 0.23    | 1.4   |
| ltkOri | 0.14    | 0.18   | -6.7e-16 | 0.018   | 0.078   | 0.2     | 2.6   |
| ltkWNB | 0.041   | 0.047  | -6.7e-16 | 0.0092  | 0.026   | 0.058   | 0.54  |
| likWBB | 0.081   | 0.082  | -6.7e-16 | 0.019   | 0.057   | 0.12    | 0.84  |

Table: Overview of the contextual morphometric values of interdecile Theil index for the whole case study. Key to character IDs is available in table A7.3. \label{theilID3_chars}

![Histograms of interdecile Theil index for characters 1-15 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_15__theilID3.pdf "Histograms of contextual characters 1-15 (Theil)"){#fig:conxdistplot1Theil width=100%}

![Histograms of interdecile Theil index for characters 16-30 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_30__theilID3.pdf "Histograms of contextual characters 16-30 (Theil)"){#fig:conxdistplot2Theil width=100%}

![Histograms of interdecile Theil index for characters 31-45 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_45__theilID3.pdf "Histograms of contextual characters 31-45 (Theil)"){#fig:conxdistplot3Theil width=100%}

![Histograms of interdecile Theil index for characters 46-60 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_60__theilID3.pdf "Histograms of contextual characters 46-60 (Theil)"){#fig:conxdistplot4Theil width=100%}

![Histograms of interdecile Theil index for characters 61-74 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_74__theilID3.pdf "Histograms of contextual characters 61-74 (Theil)"){#fig:conxdistplot5Theil width=100%}

### Simpson index {.unnumbered}
|                |   mean |   std |   min |   25% |   50% |   75% |   max |
|:---------------|-------:|------:|------:|------:|------:|------:|------:|
| sdcLAL |   0.57 | 0.22  |  0.15 |  0.39 |  0.54 |  0.74 |     1 |
| sdcAre |   0.67 | 0.22  |  0.15 |  0.49 |  0.67 |  0.85 |     1 |
| stcSAl |   0.5  | 0.16  |  0.14 |  0.38 |  0.47 |  0.6  |     1 |
| sicCAR |   0.58 | 0.21  |  0.13 |  0.42 |  0.56 |  0.73 |     1 |
| sicFAR |   0.7  | 0.26  |  0.13 |  0.5  |  0.75 |  0.95 |     1 |
| mdcAre |   0.62 | 0.24  |  0.12 |  0.42 |  0.6  |  0.85 |     1 |
| licGDe |   0.83 | 0.22  |  0.12 |  0.62 |  1    |  1    |     1 |
| ltcWRB |   0.67 | 0.26  |  0.1  |  0.44 |  0.61 |  1    |     1 |
| sdbHei |   0.68 | 0.25  |  0.13 |  0.46 |  0.67 |  0.94 |     1 |
| sdbAre |   0.71 | 0.22  |  0.16 |  0.51 |  0.73 |  0.91 |     1 |
| sdbVol |   0.73 | 0.23  |  0.17 |  0.51 |  0.78 |  0.96 |     1 |
| sdbPer |   0.61 | 0.21  |  0.17 |  0.44 |  0.6  |  0.79 |     1 |
| sdbCoA |   0.99 | 0.048 |  0.43 |  1    |  1    |  1    |     1 |
| ssbFoF |   0.52 | 0.18  |  0.11 |  0.4  |  0.49 |  0.64 |     1 |
| ssbVFR |   0.59 | 0.21  |  0.14 |  0.41 |  0.56 |  0.78 |     1 |
| ssbCor |   0.53 | 0.14  |  0.16 |  0.43 |  0.52 |  0.62 |     1 |
| ssbSqu |   0.63 | 0.18  |  0.16 |  0.5  |  0.64 |  0.77 |     1 |
| ssbCCM |   0.62 | 0.23  |  0.14 |  0.44 |  0.6  |  0.83 |     1 |
| ssbCCD |   0.53 | 0.15  |  0.18 |  0.42 |  0.51 |  0.62 |     1 |
| stbSAl |   0.59 | 0.21  |  0.13 |  0.42 |  0.55 |  0.76 |     1 |
| stbCeA |   0.53 | 0.16  |  0.15 |  0.4  |  0.5  |  0.63 |     1 |
| mtbAli |   0.54 | 0.23  |  0.12 |  0.35 |  0.48 |  0.7  |     1 |
| mtbNDi |   0.53 | 0.21  |  0.13 |  0.37 |  0.49 |  0.66 |     1 |
| libNCo |   0.92 | 0.16  |  0.2  |  0.94 |  1    |  1    |     1 |
| ldbPWL |   0.74 | 0.23  |  0.15 |  0.53 |  0.78 |  1    |     1 |
| linPDE |   0.75 | 0.23  |  0.18 |  0.53 |  0.77 |  1    |     1 |
| ldsCDL |   0.75 | 0.23  |  0.18 |  0.53 |  0.77 |  1    |     1 |
| xcnSCl |   0.66 | 0.23  |  0.2  |  0.47 |  0.6  |  0.9  |     1 |
| mtdMDi |   0.74 | 0.22  |  0.22 |  0.53 |  0.76 |  1    |     1 |
| lddNDe |   0.7  | 0.23  |  0.19 |  0.51 |  0.68 |  0.97 |     1 |
| linWID |   0.7  | 0.23  |  0.17 |  0.5  |  0.66 |  0.96 |     1 |
| lddARe |   0.76 | 0.22  |  0.21 |  0.54 |  0.8  |  1    |     1 |
| sddAre |   0.78 | 0.22  |  0.21 |  0.56 |  0.83 |  1    |     1 |
| midRea |   0.65 | 0.22  |  0.17 |  0.49 |  0.59 |  0.85 |     1 |
| midAre |   0.77 | 0.22  |  0.17 |  0.56 |  0.82 |  1    |     1 |
| sdsLen |   0.73 | 0.22  |  0.2  |  0.53 |  0.72 |  1    |     1 |
| sdsSPH |   0.75 | 0.25  |  0.15 |  0.52 |  0.82 |  1    |     1 |
| sdsSPR |   0.74 | 0.25  |  0.15 |  0.51 |  0.78 |  1    |     1 |
| sdsSHD |   0.69 | 0.25  |  0.15 |  0.48 |  0.66 |  1    |     1 |
| sdsAre |   0.78 | 0.22  |  0.2  |  0.57 |  0.83 |  1    |     1 |
| sisBpM |   0.6  | 0.21  |  0.2  |  0.45 |  0.54 |  0.74 |     1 |
| misRea |   0.65 | 0.22  |  0.16 |  0.49 |  0.59 |  0.85 |     1 |
| mdsAre |   0.78 | 0.22  |  0.17 |  0.56 |  0.83 |  1    |     1 |
| ldsMSL |   0.79 | 0.22  |  0.2  |  0.58 |  0.87 |  1    |     1 |
| ldsRea |   0.77 | 0.22  |  0.17 |  0.56 |  0.82 |  1    |     1 |
| ldkAre |   0.82 | 0.21  |  0    |  0.61 |  0.94 |  1    |     1 |
| ldkPer |   0.78 | 0.21  |  0    |  0.57 |  0.82 |  1    |     1 |
| lskCWA |   0.77 | 0.21  |  0.25 |  0.56 |  0.8  |  1    |     1 |
| likWBB |   0.67 | 0.24  |  0.16 |  0.5  |  0.61 |  0.95 |     1 |
| stcOri |   0.3  | 0.13  |  0.17 |  0.21 |  0.25 |  0.34 |     1 |
| sscCCo |   0.2  | 0.05  |  0.14 |  0.18 |  0.19 |  0.22 |     1 |
| sscERI |   0.2  | 0.041 |  0.13 |  0.18 |  0.2  |  0.22 |     1 |
| mtcWNe |   0.27 | 0.093 |  0.13 |  0.21 |  0.25 |  0.3  |     1 |
| ssbCCo |   0.24 | 0.081 |  0.14 |  0.19 |  0.22 |  0.28 |     1 |
| ssbERI |   0.32 | 0.11  |  0.14 |  0.25 |  0.29 |  0.36 |     1 |
| ssbElo |   0.24 | 0.075 |  0.17 |  0.2  |  0.23 |  0.27 |     1 |
| stbOri |   0.47 | 0.22  |  0.17 |  0.3  |  0.41 |  0.59 |     1 |
| mtbSWR |   0.49 | 0.17  |  0.25 |  0.36 |  0.44 |  0.58 |     1 |
| ltbIBD |   0.45 | 0.19  |  0.15 |  0.31 |  0.4  |  0.52 |     1 |
| ltcBuA |   0.56 | 0.21  |  0.17 |  0.41 |  0.51 |  0.67 |     1 |
| mtdDeg |   0.63 | 0.18  |  0.33 |  0.5  |  0.59 |  0.76 |     1 |
| lcdMes |   0.55 | 0.19  |  0.16 |  0.41 |  0.51 |  0.66 |     1 |
| linP3W |   0.54 | 0.19  |  0.13 |  0.4  |  0.5  |  0.63 |     1 |
| linP4W |   0.59 | 0.2   |  0.16 |  0.45 |  0.54 |  0.72 |     1 |
| lcnClo |   0.52 | 0.2   |  0.16 |  0.37 |  0.48 |  0.62 |     1 |
| lddRea |   0.47 | 0.18  |  0.15 |  0.34 |  0.43 |  0.55 |     1 |
| sdsSPW |   0.38 | 0.15  |  0.15 |  0.27 |  0.33 |  0.43 |     1 |
| sdsSPO |   0.38 | 0.16  |  0.15 |  0.27 |  0.34 |  0.43 |     1 |
| sdsSWD |   0.37 | 0.15  |  0.17 |  0.27 |  0.33 |  0.42 |     1 |
| sssLin |   0.74 | 0.22  |  0.2  |  0.54 |  0.75 |  1    |     1 |
| lskCCo |   0.47 | 0.19  |  0.15 |  0.33 |  0.42 |  0.54 |     1 |
| lskERI |   0.49 | 0.19  |  0.16 |  0.36 |  0.45 |  0.57 |     1 |
| ltkOri |   0.53 | 0.21  |  0.17 |  0.37 |  0.48 |  0.63 |     1 |
| ltkWNB |   0.53 | 0.22  |  0.15 |  0.36 |  0.47 |  0.64 |     1 |

Table: Overview of the contextual morphometric values of Simpson index for the whole case study. Key to character IDs is available in table A7.3. \label{simpson_chars}

![Histograms of Simpson index for characters 1-15 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_15__simpson.pdf "Histograms of contextual characters 1-15 (Simpson)"){#fig:conxdistplot1Simpson width=100%}

![Histograms of Simpson index for characters 16-30 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_30__simpson.pdf "Histograms of contextual characters 16-30 (Simpson)"){#fig:conxdistplot2Simpson width=100%}

![Histograms of Simpson index for characters 31-45 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_45__simpson.pdf "Histograms of contextual characters 31-45 (Simpson)"){#fig:conxdistplot3Simpson width=100%}

![Histograms of Simpson index for characters 46-60 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_60__simpson.pdf "Histograms of contextual characters 46-60 (Simpson)"){#fig:conxdistplot4Simpson width=100%}

![Histograms of Simpson index for characters 61-74 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_74__simpson.pdf "Histograms of contextual characters 61-74 (Simpson)"){#fig:conxdistplot5Simpson width=100%}


## 7.8 Correlation matrix of contextual characters {.unnumbered}

	![Correlation matrix of contextual characters](source/figures/appendix_conx/spearman_conx.pdf "Correlation matrix of contextual characters"){#fig:spearman_conx_hq width=100%}

==Commented out, uncomment for final export.==

## 7.9 Structure of clusters of sampled and complete clustering {.unnumbered}

Supplementary material for section 7.2.3.2.2.1.

![Composition of clusters in relation to sampled clustering. Shows number of features labeled as studied cluster and their labels in the other clustering variant.](source/figures/a7/relation_complete-sampled.pdf "Composition of clusters in relation to sampled clustering."){#fig:compsamp width=100%}


![Composition of sampled clusters in relation to original clustering. Shows number of features labeled as studied cluster and their labels in the other clustering variant.](source/figures/a7/relation_sampled-complete.pdf "Composition of sampled clusters in relation to original clustering"){#fig:sapmcomp width=100%}

