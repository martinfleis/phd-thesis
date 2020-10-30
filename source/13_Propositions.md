# Propositions

## Synthesis of background chapters
*Draw on the conclusions of the background chapters to identify your research hypotheses or research questions.*

*Understand where your work lies on the dimensions that are appropriate to your discipline: theoretical or applied, study or case study, and so on. Use this understanding to inform your explanation of your intended contribution.*

*Positioning requires justification. For example, if you decide on a case-study approach, explain why, and justify your choice of specific case to study; if a long description of the case is needed, note that you will do this in a separate following chapter.*

The goal of chapters 2, 3 and 4 was to provide a necessary theoretical, conceptual and methodological background for the work proposed within this study. It is clear that the field of urban morphometrics is advancing in recent years in a fast pace. However, as shown in each of the chapters, there are still clear and wide gaps to fill.

Existing literature, as shown in the chapter 2, offers a various methods for classification of urban form. While approaches vary from simple duality *organised-unorganised* form based on remotely sensed data () to comprehensive small scale studies based on detailed manual digitisation of  urban form elements [@dibble2017], none of them is ideal. The optimal classification model, which consists of 7 principles (see section XXX) is not fully reflected in any of the existing proposals.

One of the potential pathway which could lead to better classification models is morphometrics and related numerical taxonomy stemming from the phenetic studies in biology. Conceptually, morphometrics itself is already well established in urban morphology (as shown in detail in chapter 4) and previous work of @dibble2017 showed the potential of application of numerical taxonomy as well. However, as shown in the chapter 3, the existing proposals bridging the two are not fully operational on a large scale and on unrestricted spatial units. The critical elements, an operational taxonomic unit, needs to be fully revisited to better reflect the nature of urban form and allow exhaustive analysis of metropolitan areas, rather than a specific carefully selected set of case studies.

The related biological concept with may help with the issue of undefined OTU is a *mixture problem*. That arises when a taxonomist needs to identify populations within samples to then perform classification on a population level. The parallel in urban morphology is apparent. From a pool of fundamental units, i.e buildings, plots and streets [@moudon1997], morphologist needs to identify distinct patterns of form and classify those into a taxonomy.

Chapter 4 then provided a deep dive into urban morphometrics and existing methods of measuring of urban form. For the rest of the thesis, it is possible to draw three conclusions out of the chapter. First, although there is a rich pool of relevant studies, we often lack those which are at the same time granular and extensive, while providing comprehensive description of form. Second, the field has a nomenclature issue to tackle. The so called *nicknaming issue* prevents comparability and brings a layer of inconsistency hard to declutter without a detailed decomposition of each individual method to the level of characters' formulas. Last,  urban morphometrics can already measure an abundant number of characters covering all aspects of urban form. However, the focus is not very balanced and some categories of characters require a development of new approaches.
 
## Hypothesis & research questions
The aim of this work is to fill some of the gaps identified in previous chapters and develop a method of classification of urban form which reflects *optimal classification model* and follows principles of morphometrics and numerical taxonomy. The scope of the work is primarily technical, focused on reproducibility and replicability of quantitative science of urban morphology, eventually leading to the establishment of the atlas of urban form. However, in its nature the work is still exploratory. If the principles will hold, the work should pave the way for more robust implementations.

The theoretical contribution lies in the revaluation of the bridge between numerical taxonomy and urban morphology previously proposed by @dibble2017. 

### Hypothesis
Drawing on the background knowledge presented in previous chapters, the main hypothesis behind the proposals laid in the rest of the thesis is then as follows:

> Methods of morphometrics and numerical taxonomy established in the classification of biological species can be applied in the context of urban morphology to lay foundations of numerical taxonomy of urban form.

The rest of the thesis builds on the hypothesis and proposes an actual implementation of numerical taxonomy, which is later validated in chapter 8. The validation of the method then indicates whether the hypothesis should be proved or disproved, which in turn tells whether the application of numerical taxonomy in urban morphology is a viable direction of research.
 
### Research questions
The process of verification of hypothesis needs to provide an answer to the main research question and a series of subsequent supplementary research questions. 

#### Main research question
The main research question (RQ) focus on the operationalisation of numerical taxonomy in the context of urban morphology:

> How to adapt methods of numerical taxonomy to study of urban form?

Answering the question gives us enough ground to understand whether such adaptation provides meaningful information for further analysis of built environment. The task itself could then be subdivided into four supplementary research questions, which together outline the research proposal eventually answering the RQ.

#### Supplementary research questions
All four supplementary research questions (SRQ) focus on operationalisation of numerical taxonomy as a method based on urban morphometrics.

The first question focus on the identification of features which at the same time form urban fabric and could be studied using morphometric methods and the connections between them:

> What are the fundamental morphometric elements and how to model their relationship?

Chapter 6 is dedicated to answering the question.

The second question builds on the previous and fills the gap identified in chapter 3. The question of OTU is critical as it directly affects very nature of the taxonomy. The question itself seeks an answer to both theoretical definition of the fundamental unit of urban form and the technical aspects of its delineation:

> What is the optimal Operational Taxonomic Unit of urban form and how to identify it in continuous urban fabric?

Since an OTU is the result of a population delineation (see *mixture problem*), it is necessarily an aggregation of fundamental morphometric elements. The overview of aggregation models is available in the chapter 6, together with a theoretical discussion and definition of OTU for this study. The delineation part is the content of the chapter 7.

Morphometric assessment of any kind is based on morphometric characters, i.e. measurable aspects of elements used within the study. Their selection and implementation are the key drivers influencing the results of the analysis, hence it is necessary to give them enough attention and dedicate one SRQ to the topic:

> What are the taxonomic characters describing urban form?

The first part of the chapter 7 aims to provide answers, building on the database collected in the chapter 4.

The final SRQ focus on the final aspect of creation of a numerical taxonomy, the quantification of similarity of OTUs:

> How to determine the taxonomic relationship between OTUs to derive taxa of urban form?

The method of numerical taxonomy in the context of urban form and related answers to the last question are part of the chapter 8.

## Methodological propositions
- *describe method and say why this particular method*
- *Discuss the range of research methods that could be used to test your hypotheses or answer your questions, and choose the most appropriate. Don’t forget to justify your choice, even if it is standard for your discipline.*
- *Experimental validation requires an experimental design. Expect to have to explain it in detail, and also to justify it. Make appropriate choices of measurement or assessment mechanisms.*
- *link to the scope*

*If you have not already described your detailed research procedure in the ‘Research Design’ chapter you should describe it first before you go on to report any research results.*

*building a case that your new approach solves problems that previous approaches neglected.*

*top level to reflect the questions above and chapter-level*

### Assessment of morphometric elements

*fundamental elements, aggregations, models*
- understand fundamental elements for morphometric assessment ==link to scope==
	- exploration of morphological tessellation
- understand methods of their aggregation to larger spatial units
- understand models of capturing relations between elements and their aggregations
*leading to the relational model and tissue as OTU*
- define the model of capturing the relationship between elements and their aggregations 
- define the role of urban tissue in relation to the model

### OTU
- Urban tissue is an optimal OTU
- ==Hypothesis *Urban tissues can be recognised by empirical measuring of the physical structure of urban fabric in a form of homogenous clusters.*==
- Urban tissue is a contiguous area of a single tissue type, i.e. a single cluster

_Refer back to chapter 2 and discuss the reason why tissue is optimal_
- _it reflects unconstrained morphological unit_
- _tissue as OTU (link to Ch4 and Ch5)_ ==after ch4 is done==
- _morphological regionalizaition (Oliveira)_
- _heavily refer to literature which sees tissue as unit as well. Why SA is not a unit is in chapter 4_

### Identification of OTU in urban fabric

*selection and definition of morphometric characters*
- definition of selection criteria
- primary and contextual characters
- selection of primary characters
- selection of contextual characters
*identification of OTU using cluster analysis*
- clustering method (==justify selection==)
	- ==move from ch7?==

### Estimating taxonomic relationships

*Ward's hierarchical clustering*
- clustering method

### Validation
*Validation theory*
- if it relates to data and works elsewhere and can be expanded
*validation method*
- relation to data
- transferability
- expandability
- *if A & B & C, then valid*

### momepy: Urban Morphology Measuring Toolkit
reproducibility, scalability, openness
Need for tools
==link functions and classes to each relevant stage==
==link Jupyter notebooks to each relevant stage==

### Case studies
*for a case study, you need to persuade the reader that the subject is representative of a broader population.*

Prague
- brief description

Amsterdam
- brief description

Zurich
- used for a specific task (mostly due to publishing as an independent paper)
- brief description (take from ch6)

## Outline of the second part
- ch6
- ch7
- ch8
- ch9

———


*These components together form a hypothesis*

*Design a narrative flow that takes the reader painlessly through the central part of your thesis—the part that consists of the new ideas that you are arguing for (and is thus the most unfamiliar).*

*Ensure that at all stages you have a clear understanding of the argument you*
*intend to use for linking of question, data, analysis, and outcome.*

