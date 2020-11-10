# Appendix A7: Supplementary material for chapter 7 {.unnumbered}

\renewcommand\thefigure{A7.\arabic{figure}}
\setcounter{figure}{0}
\renewcommand\thetable{A7.\arabic{table}}
\setcounter{table}{0}
\pagestyle{plain}

## 7.1 Selection of primary characters {.unnumbered}
==refer back to the section==
To be done.

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

==todo: description==

Note: Please refer to the electronical version of the thesis for a better clarity. Sectional diagrams are not optimised for print.

![Sectional](source/figures/a7/sect_full.pdf "Sectional"){#fig:sect_full width=100%}

![Sectional](source/figures/a7/sect_det.pdf "Sectional"){#fig:sect_det width=100%}

\newpage

## 7.4 Analysis of local central tendency characters {.unnumbered}
To be done.

## 7.5 Contextual characters comparison {.unnumbered}
To be done.

## 7.6 Spatial autocorrelation of contextual characters {.unnumbered}
To be done.

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

Table: Overview of the contextual morphometric values of interquartile mean for the whole case study. Key to character IDs is available in table XXX. \label{meanIQ3_chars}

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

Table: Overview of the contextual morphometric values of interquartile range for the whole case study. Key to character IDs is available in table XXX. \label{rangeIQ3_chars}

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

Table: Overview of the contextual morphometric values of interdecile Theil index for the whole case study. Key to character IDs is available in table XXX. \label{theilID3_chars}

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

Table: Overview of the contextual morphometric values of Simpson index for the whole case study. Key to character IDs is available in table XXX. \label{simpson_chars}

![Histograms of Simpson index for characters 1-15 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_15__simpson.pdf "Histograms of contextual characters 1-15 (Simpson)"){#fig:conxdistplot1Simpson width=100%}

![Histograms of Simpson index for characters 16-30 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_30__simpson.pdf "Histograms of contextual characters 16-30 (Simpson)"){#fig:conxdistplot2Simpson width=100%}

![Histograms of Simpson index for characters 31-45 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_45__simpson.pdf "Histograms of contextual characters 31-45 (Simpson)"){#fig:conxdistplot3Simpson width=100%}

![Histograms of Simpson index for characters 46-60 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_60__simpson.pdf "Histograms of contextual characters 46-60 (Simpson)"){#fig:conxdistplot4Simpson width=100%}

![Histograms of Simpson index for characters 61-74 are showing the variety of distributions within the measured contextual data.](source/figures/appendix_conx/conx_distplot_74__simpson.pdf "Histograms of contextual characters 61-74 (Simpson)"){#fig:conxdistplot5Simpson width=100%}


## 7.8 Correlation matrix of contextual characters {.unnumbered}

	![TITLE. ](source/figures/appendix_conx/spearman_conx.pdf "Short caption"){#fig:spearman_conx_hq width=100%}

==Commented out, uncomment for final export.==

## 7.9 Structure of clusters of sampled and complete clustering {.unnumbered}

To be done.
(Maybe not)