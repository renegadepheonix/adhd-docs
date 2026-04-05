<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" style="height:64px;margin-right:32px"/>

# Requirements elicitation methods in software and knowledge engineering.

Structured techniques for decomposing ambiguous user goals into specific,
testable objectives. Empirical comparisons of elicitation techniques by
quality and completeness of outputs. Practitioner-grounded evidence.
NOT vendor methodology documentation.

Requirements elicitation methods that best decompose ambiguous goals into concrete, testable requirements tend to combine goal‑oriented modeling with interactive, artefact‑rich sessions (e.g., prototyping, structured workshops) and are empirically associated with higher completeness and better stakeholder acceptance than interviews alone.[^1_1][^1_2][^1_3][^1_4][^1_5][^1_6]

## Core elicitation methods (software and knowledge engineering)

- **Semi‑structured interviews and variants**: Unstructured interviews, Joint Application Design (JAD), and paper prototyping in interview settings are widely studied; a family of experiments with 167 participants found paper prototyping yielded the highest number of elicited requirements, while JAD improved diversity and completeness compared to unstructured interviews.[^1_1]
- **Workshops and group techniques**: Practitioners in multiple companies report meetings and workshops as their primary elicitation mode, especially in agile and continuous delivery contexts, often combining brainstorming, story mapping, and collaborative modeling.[^1_7][^1_3]
- **Scenario‑ and use‑case–based elicitation**: Systematic mappings and comparative reviews show scenarios, use cases, and user stories are among the most frequently used methods and are seen as effective at surfacing both functional and non‑functional requirements when combined with interviews.[^1_8][^1_9][^1_5]
- **Prototyping (paper, low‑fi, executable)**: Experimental work shows paper prototyping in elicitation interviews increases the number of requirements discovered and supports clarification and negotiation in situ.[^1_5][^1_1]
- **Creativity‑support techniques**: Lightweight “creativity trigger” card sets used in elicitation workshops increase the novelty and breadth of requirements while remaining acceptable to practitioners in different organizational contexts.[^1_2]
- **Design thinking–inspired methods**: Techniques such as IoThinking and Mind IoT for IoT requirements show similar effectiveness in the number of requirements elicited but differ in practitioner‑perceived fit: one better for early elicitation, the other for refining and mapping requirements after an initial pass.[^1_10][^1_11]
- **AI/ML‑based elicitation aids**: Reviews of AI and machine‑learning–based elicitation identify tasks such as extracting candidate requirements from text, clustering feedback, or generating initial requirements; these approaches augment rather than replace human elicitation and still require refinement steps.[^1_12][^1_13]


## Goal decomposition into testable objectives

In both software and ontology/knowledge engineering, structured goal modeling and competency questions are central devices for turning vague stakeholder intentions into specific, testable statements.[^1_14][^1_4][^1_6]

- **Goal models (e.g., KAOS, i\*)**: Goal decomposition frameworks advocate recursively refining high‑level stakeholder goals into subgoals and finally into operational tasks, using AND/OR patterns grounded in temporal semantics to ensure that lower‑level goals are sufficient and non‑redundant.[^1_4][^1_6]
- **From goals to operational requirements**: These approaches explicitly connect problem‑space expressions (goals) to solution‑space actions, making it easier to derive measurable conditions and test cases (e.g., success scenarios, obstacle analysis) from each leaf‑level goal.[^1_6]
- **Competency question (CQ) elicitation for ontologies**: Comparative work contrasts manual CQ formulation, pattern‑based CQs, and LLM‑generated CQs; manually and pattern‑generated questions tend to score higher on acceptability and reduced ambiguity, while LLM‑generated CQs are useful as an initial elicitation source but require subsequent human refinement.[^1_14]
- **Patterns and templates**: CQ patterns and goal decomposition templates provide reusable structures for turning user intents into specific, answerable or verifiable questions (e.g., “Which X have property Y at time T?”), improving clarity and testability compared to ad‑hoc formulations.[^1_6][^1_14]

A concrete illustration: starting from “improve user engagement,” a goal‑oriented process would refine this into subgoals such as “increase daily active users by 20% within six months” and “reduce average onboarding time to under five minutes,” each of which then maps to specific functional/non‑functional requirements and acceptance tests.[^1_15][^1_6]

## Empirical comparisons of elicitation techniques

Several studies and reviews address comparative performance of elicitation techniques on quality, completeness, and other attributes, often with practitioner‑grounded or realistic settings.

- **Interview‑based methods: family of experiments**
    - Methods compared: unstructured interviews, JAD, paper prototyping.[^1_1]
    - Measures: number of requirements, time, diversity, completeness, quality, performance; teams produced specification documents after up to four interview rounds.[^1_1]
    - Findings: paper prototyping yielded more requirements; JAD showed advantages on diversity/completeness; unstructured interviews generally underperformed on these quantitative measures.[^1_1]
- **Combined techniques and FR/NFR quality**
    - A study of combined techniques (interview, prototyping, brainstorming) found that using multiple techniques improved completeness and consistency for both functional and non‑functional requirements compared to single techniques in a course‑based setting.[^1_5]
- **Traditional vs modern techniques**
    - Comparative research across multiple projects observed that modern techniques (collaborative workshops, prototyping, AI‑supported methods) tended to gather more comprehensive and clearer requirements and increase stakeholder satisfaction, though they often required more facilitation skill and setup compared with basic interviews and questionnaires.[^1_16]
- **Creativity triggers (CTs)**
    - Large‑scale, multi‑context evaluation of CT cards in requirements elicitation showed that they helped stakeholders uncover novel system features and were judged useful and usable by participants from differing viewpoints.[^1_2]
- **Systematic mappings and “right technique” constructs**
    - A systematic mapping of comparisons among elicitation techniques identified 43 studies and 58 distinct metrics used to judge “appropriateness,” including quantity of requirements, coverage of functional/non‑functional areas, ambiguity, understandability, stakeholder satisfaction, and cost/time.[^1_17][^1_18][^1_19]
    - These reviews emphasize that no single technique dominates across all constructs, and advocate multi‑criteria decision‑making approaches (e.g., analytic network process, best–worst method) for selecting techniques tailored to project, people, and process characteristics.[^1_20][^1_21][^1_18]
- **State of practice and continuous engineering**
    - Interview‑based surveys of practitioners in Swedish IT companies report that group interaction techniques are the most popular, with individual techniques (e.g., one‑to‑one interviews) more common in small projects.[^1_3]
    - In continuous software engineering, companies combine qualitative feedback (interviews, support channels, workshops) with quantitative data (telemetry, A/B tests) but struggle with selecting metrics and analyzing data fast enough to inform frequent releases.[^1_7]


## Practitioner‑grounded evidence and selection guidance

Several bodies of work explicitly ground their findings in practitioner experience or realistic settings and avoid vendor‑specific prescriptions.

- **Practitioner interviews and case studies**: Studies on state‑of‑practice elicitation and continuous feedback loop practices are based on interviews and cross‑case analyses in multiple product development companies, surfacing real constraints such as stakeholder availability, conflicting perspectives, and data overload.[^1_3][^1_7]
- **Frameworks for technique selection**:
    - Attribute‑based frameworks and decision models consider project characteristics, stakeholder types, domain, and development process to recommend appropriate combinations of elicitation techniques, arguing that over‑reliance on a single method (especially open interviews) is problematic.[^1_21][^1_18][^1_19]
    - Neural‑network and best–worst method–based approaches operationalize this selection, though evidence of industrial uptake remains limited.[^1_22][^1_18][^1_20]
- **Knowledge‑engineering specific evidence**:
    - Comparative CQ‑generation studies in ontology engineering use multi‑annotator evaluation of ambiguity, relevance, readability, and complexity, and show that mixed workflows (automatic generation plus human refinement) offer a practical balance between productivity and quality.[^1_14]


### Emerging patterns for practice

Across these studies and mappings, several consistent findings emerge:

- No single elicitation technique is sufficient; combining techniques (e.g., workshops + interviews + prototyping) improves completeness and consistency of requirements.[^1_23][^1_24][^1_5][^1_1]
- Artefact‑mediated and visual techniques (prototypes, storyboards, goal models, CT cards) help stakeholders articulate and refine requirements more effectively than verbal discussion alone, especially for ambiguous or innovative goals.[^1_2][^1_6][^1_1]
- Goal‑oriented and CQ‑based methods provide a structured backbone for decomposing high‑level, ambiguous goals into lower‑level, verifiable requirements in both software and ontology settings.[^1_4][^1_6][^1_14]
- Practitioner‑grounded studies stress that technique selection must account for organizational context, delivery cadence, and available feedback channels; continuous product teams, for example, lean more on telemetry and iterative experiments than one‑off elicitation phases.[^1_7][^1_3]

Would it be most useful for you if I synthesize this into a compact, method‑by‑method table with columns for “supports goal decomposition?”, “evidence on completeness/quality?”, and “strength of practitioner grounding?”
<span style="display:none">[^1_25][^1_26][^1_27][^1_28][^1_29][^1_30][^1_31][^1_32]</span>

<div align="center">⁂</div>

[^1_1]: https://linkinghub.elsevier.com/retrieve/pii/S0950584920301282

[^1_2]: https://linkinghub.elsevier.com/retrieve/pii/S0164121222000930

[^1_3]: https://arxiv.org/abs/2102.11556

[^1_4]: http://www.yorku.ca/liaskos/Docs/Eye11.pdf

[^1_5]: https://www.scitepress.org/Papers/2021/104327/104327.pdf

[^1_6]: https://ceur-ws.org/Vol-766/paper09.pdf

[^1_7]: https://link.springer.com/10.1007/s10664-024-10557-2

[^1_8]: https://ieeexplore.ieee.org/document/10496655/

[^1_9]: https://eecs481.org/readings/requirements.pdf

[^1_10]: https://dl.acm.org/doi/10.1145/3701625.3701693

[^1_11]: https://sol.sbc.org.br/index.php/sbes/article/view/30358

[^1_12]: http://www.jsoftware.us/show-244-3113-1.html

[^1_13]: https://www.cambridge.org/core/services/aop-cambridge-core/content/view/9B3886539161631E08661FDBCA4192BB/S0890060422000166a.pdf/div-class-title-machine-learning-in-requirements-elicitation-a-literature-review-div.pdf

[^1_14]: https://arxiv.org/abs/2507.02989

[^1_15]: https://bscdesigner.com/strategy-decomposition.htm

[^1_16]: https://www.fmdbpub.com/user/journals/article_details/FTSTPL/247

[^1_17]: https://scielo.conicyt.cl/pdf/ingeniare/v24n2/art09.pdf

[^1_18]: https://downloads.hindawi.com/journals/mpe/2020/2156023.pdf

[^1_19]: https://oa.upm.es/37447/1/INVE_MEM_2014_195480-3.pdf

[^1_20]: http://thesai.org/Downloads/Volume12No11/Paper_83-Multi_Criteria_Decision_Making_Approach_for_Selection_of_Requirements.pdf

[^1_21]: https://arxiv.org/pdf/1709.08481.pdf

[^1_22]: http://thesai.org/Downloads/Volume13No1/Paper_44-Selection_of_Requirement_Elicitation_Techniques.pdf

[^1_23]: https://www.ijrdet.com/files/Volume1Issue3/IJRDET_1213_01.pdf

[^1_24]: https://research.ijcaonline.org/volume116/number4/pxc3902408.pdf

[^1_25]: https://www.icck.org/article/abs/jse.2025.862549

[^1_26]: http://thesai.org/Downloads/Volume9No1/Paper_45-Requirement_Elicitation_Techniques_for_Open_Source_Systems.pdf

[^1_27]: http://thesai.org/Downloads/Volume12No8/Paper_16-Enhanced_Framework_for_Big_Data_Requirement.pdf

[^1_28]: http://www.arpnjournals.org/jeas/research_papers/rp_2019/jeas_0119_7590.pdf

[^1_29]: https://plprojects.co.uk/eliciting-requirements-from-stakeholders/

[^1_30]: https://lifetips.alibaba.com/tech-efficiency/how-can-i-turn-vague-goals-into-actionable-to-dos

[^1_31]: https://citeseerx.ist.psu.edu/document?repid=rep1\&type=pdf\&doi=2ca8e9d5c226863202402acb75585b543751d6fc

[^1_32]: https://www.ijera.com/papers/Vol6_issue4/Part%20-%205/A0604050107.pdf


---

# Problem structuring methods for ill-defined objectives in decision analysis

and operations research. How these methods surface implicit constraints,
missing information, and unstated assumptions. Trade-offs between approaches
by cognitive demand on participants and practitioner uptake. Exclude
management consulting generics and MBA-level summaries.

Problem structuring methods (PSMs) in OR/decision analysis provide facilitated, model‑based ways to turn messy, ill‑defined situations into tractable decision problems, and they do so by making objectives, constraints, assumptions, and knowledge gaps explicit in shared representations.[^2_1][^2_2][^2_3]

## Main PSM families and how they surface “hidden” structure

- **Soft Systems Methodology (SSM)**: Uses rich pictures, root definitions and CATWOE analysis to externalize differing stakeholder worldviews, highlighting implicit constraints (e.g., institutional roles, norms), conflicting purposes, and areas where the “system” boundary is contested.[^2_2][^2_3]
- **Strategic Options Development and Analysis (SODA)**: Builds individual and group cognitive maps from interviews; causal links in the maps surface assumptions about how variables influence each other, reveal missing factors, and expose conflicting beliefs about what drives key objectives.[^2_4][^2_5][^2_6]
- **Strategic Choice Approach (SCA)**: Structures problems around decision areas, options, and “comparison areas,” then explicitly logs uncertainties and “commitment packages,” forcing discussion of dependencies, information gaps, and implementation constraints before optimization.[^2_7][^2_8]
- **Value‑Focused Thinking (VFT) as a structuring step**: Uses iterative questioning (“why is that important?”) and value hierarchies to elicit fundamental objectives, which then become criteria for MCDA, revealing hidden value trade‑offs and missing performance attributes.[^2_9][^2_10]
- **Group model building and system dynamics‑based PSMs**: Facilitation leads participants to identify feedback loops, accumulations, and delays, often surfacing dynamic constraints (capacity, time lags) and tacit strategic assumptions that are invisible in static lists.[^2_8][^2_2]

Across these families, shared diagrams (rich pictures, cognitive maps, influence diagrams) function as **boundary objects**, giving participants something concrete to critique, extend, or reframe, which is where implicit constraints, missing information, and tacit assumptions tend to be articulated.[^2_6][^2_2][^2_4]

## Mechanisms for surfacing constraints, gaps, and assumptions

- **Iterative, facilitated mapping**: PSMs typically start from loosely structured narratives and iteratively refine visual models through questioning and re‑mapping; interventions like “what must be true for this arrow to hold?” or “what is missing between these nodes?” deliberately target hidden assumptions and information gaps.[^2_5][^2_4][^2_6]
- **Multiple stakeholder worldviews**: Methods such as SSM and SODA explicitly encourage separate maps or worldviews before convergence, so differences in perceived objectives, constraints, and problem boundaries are visible rather than averaged away.[^2_3][^2_2][^2_4]
- **Explicit uncertainty and “problematic” elements**: SCA, in particular, distinguishes between “shaping,” “designing,” and “choosing” phases and keeps a record of key uncertainties and interdependencies, which highlights where more information, negotiation, or contingency planning is required.[^2_7][^2_8]
- **Transition to formal DA/MCDA models**: Reviews of MCDA practice show that problem structuring steps (often via VFT, SSM, or ad‑hoc rich pictures) are where objectives and constraints are made explicit before moving to value functions or outranking models, thereby surfacing unstated modelling assumptions early.[^2_11][^2_10][^2_9]

A typical sequence in SODA, for example, starts from free‑form expressions of “issues,” builds them into linked cognitive maps, then clusters and re‑labels them as goals, constraints, and options; the need to assign these roles and directions (cause→effect) is what draws out tacit constraints and contested causal stories.[^2_4][^2_5][^2_6]

## Cognitive demand vs practitioner uptake

Evidence on cognitive demand and uptake is patchy but there are some comparative and review‑level findings.

- **Overall practitioner uptake**
    - A recent review of PSM applications across 15 years of practice finds SSM, SODA, and SCA remain the most frequently used methods in OR interventions, usually embedded in facilitated workshops and often combined with “hard” OR tools; uptake is stronger in Europe than in the USA.[^2_12][^2_13][^2_2]
    - A separate review emphasizes that PSMs have expanded OR’s reach to complex, strategic problems but still face recognition challenges and uneven adoption, partly due to required facilitation skill and lack of standardization.[^2_2][^2_3]
- **Comparative workshop study (PSM‑supported vs self‑organized)**
    - A quasi‑experimental study comparing workshops supported by SSM and SCA with non‑PSM “self‑organised” workshops found that PSM‑supported groups produced outputs judged more useful for decision making, but required more facilitation effort and imposed more structure on participant thinking.[^2_7]
    - Participants reported that PSM workshops improved clarity and shared understanding but could feel demanding due to unfamiliar notation and the need to articulate reasoning explicitly.[^2_7]
- **Cognitive load characteristics by method (from reviews and practice reports)**
    - SSM: Conceptually demanding (systems thinking, CATWOE) and facilitation‑intensive, but representationally simple (rich pictures, plain language); often seen as accessible after brief explanation, though full methodology can be heavy for novices.[^2_3][^2_2]
    - SODA: Cognitive maps can become large and intricate; participants must articulate causal links, which is mentally demanding but also stimulating; software support can help, but cognitive mapping remains a learned skill.[^2_5][^2_6][^2_4]
    - SCA: Requires participants to think in terms of options, commitments, and interdependent decision areas; reviews describe it as powerful but complex, with a steeper learning curve and lower diffusion than SSM/SODA.[^2_8][^2_3]
    - VFT (as a structuring step): Conceptually straightforward (iterative “why?” and “how?” questions) and relatively low notation burden; widely adapted and taught in decision analysis, but rigorous application still requires skilled facilitation.[^2_14][^2_10][^2_11]

Soft‑OR overviews consistently note that while these methods reduce **computational** burden for participants (no math required in the structuring phase), they intentionally **raise conceptual** and reflective demands, which can cause resistance in time‑constrained settings or cultures used to jumping directly to solutions.[^2_6][^2_2][^2_4]

## Trade‑offs and combinations

Reviews of PSM characteristics and method combinations in MCDA/OR suggest several trade‑offs that align with your focus.[^2_15][^2_9][^2_3]

- **Depth of structuring vs time and cognitive effort**
    - Rich pictures and informal mapping give quick, low‑threshold structure but may leave assumptions and constraints under‑articulated.[^2_16][^2_2]
    - Full SSM/SODA/SCA cycles elicit richer, more transparent structures and assumptions, at the cost of more sessions, higher facilitation complexity, and greater participant cognitive effort.[^2_2][^2_4][^2_7]
- **Formalism vs practitioner uptake**
    - Highly formal PSM variants or tightly specified protocols can intimidate new users and reduce uptake outside specialist OR communities.[^2_8][^2_3]
    - “Lightweight” or hybrid practices (e.g., using cognitive mapping or VFT‑style objectives trees to feed into AHP or other MCDA methods) see higher use in applied domains such as defence and environmental management, because they align more closely with existing planning practices.[^2_10][^2_9][^2_11]
- **Facilitator dependence vs scalability**
    - PSMs are generally facilitation‑intensive; reports from OR practitioner networks identify facilitator skill as both a strength (quality of engagement) and a bottleneck for wider uptake.[^2_4][^2_8][^2_2]
    - Some recent work embeds PSM concepts in group decision support software or integrates them with MCDA templates, aiming to reduce dependence on elite facilitation while retaining structuring benefits.[^2_17][^2_13][^2_9]


### A concise comparison across key methods

| Method | How it surfaces constraints/assumptions | Cognitive demand on participants | Practitioner uptake (OR/DA) |
| :-- | :-- | :-- | :-- |
| SSM | Multiple rich pictures, CATWOE and root definitions expose differing system boundaries, roles, and environmental constraints.[^2_2][^2_3] | Moderate conceptual load (systems notions) but relatively simple visuals; discussion‑heavy.[^2_2] | High within European soft‑OR practice; often combined with hard OR/MCDA.[^2_13][^2_12] |
| SODA | Cognitive maps make causal assumptions and goal–constraint linkages explicit; clustering reveals missing or conflicting elements.[^2_4][^2_6][^2_5] | High cognitive demand: participants articulate causal structure; can be intense in large maps.[^2_4] | Widely used in strategy/organizational decisions where specialised facilitation is available.[^2_6][^2_8] |
| SCA | Structures decisions into areas/options, tracks dependencies and uncertainties; “commitment packages” highlight feasibility constraints and information gaps.[^2_8][^2_7] | Moderate–high: requires thinking in decision structures and embracing explicit uncertainty.[^2_7] | Moderate; valued in complex infrastructure and public‑policy contexts but less diffused than SSM/SODA.[^2_8][^2_2] |
| VFT (as structuring) | Recursive “why?”/“how?” questions and value trees reveal fundamental objectives, hidden trade‑offs, and missing criteria.[^2_10][^2_11] | Low–moderate: conceptually simple but can be demanding if many stakeholders and objectives.[^2_11] | High in DA/MCDA communities; often first step before quantitative modelling.[^2_11][^2_14] |
| Group model building (SD‑based) | Feedback loop diagrams expose dynamic constraints (capacity, delays) and implicit beliefs about system behaviour.[^2_8][^2_2] | High: requires grasping stocks/flows and feedback; rich but cognitively heavy for novices.[^2_2] | Moderate; institutionalised in some policy and environmental domains.[^2_8][^2_2] |

Given your interest, the more demanding PSMs (SSM, SODA, SCA, SD‑based GMB) yield deeper structuring and more explicit assumptions/constraints, but they trade off against scalability and ease of adoption, whereas lighter approaches (rich pictures, VFT objectives hierarchies feeding MCDA) offer a gentler on‑ramp with somewhat shallower, but still useful, structuring.

Is there a particular application domain (e.g., health, infrastructure, defence, environmental planning, digital products) where you’d like this comparison sharpened into more concrete design guidance?
<span style="display:none">[^2_18][^2_19][^2_20][^2_21][^2_22][^2_23][^2_24][^2_25][^2_26][^2_27][^2_28][^2_29][^2_30][^2_31][^2_32]</span>

<div align="center">⁂</div>

[^2_1]: https://www.iaorifors.com/paper/20200

[^2_2]: https://www.emerald.com/insight/content/doi/10.1108/IJOA-01-2023-3562/full/html?skipTracking=true

[^2_3]: https://www.sciencedirect.com/science/article/abs/pii/S0377221718303783

[^2_4]: https://eijh.modares.ac.ir/article-27-4631-en.pdf

[^2_5]: https://ojs.jdss.org.pk/journal/article/download/932/874/1313

[^2_6]: https://pubsonline.informs.org/do/10.1287/orms.2009.02.16/full/

[^2_7]: https://linkinghub.elsevier.com/retrieve/pii/S0377221718310683

[^2_8]: https://www.theorsociety.com/media/6856/reinvigorating-soft-or-for-practitioners-report-to-horaf-v12.pdf

[^2_9]: https://linkinghub.elsevier.com/retrieve/pii/S0377221717303880

[^2_10]: https://www.scielo.br/j/prod/a/9VNRWL95sCxRH85bVh8qcYs/?format=pdf\&lang=en

[^2_11]: https://linkinghub.elsevier.com/retrieve/pii/S0377221724005988

[^2_12]: https://www.emerald.com/ijoa/article/33/10/3587/1258996/Dealing-with-complexity-the-use-of-problem

[^2_13]: https://www.emerald.com/insight/content/doi/10.1108/ijoa-08-2024-4746/full/html

[^2_14]: https://arxiv.org/pdf/1302.3565.pdf

[^2_15]: https://research.manchester.ac.uk/en/publications/the-characteristics-of-problem-structuring-methods-a-literature-r/

[^2_16]: https://ianjseath.wordpress.com/2015/02/11/problem-structuring-an-essential-first-step/

[^2_17]: https://ouci.dntb.gov.ua/en/works/9je6Jjpl/

[^2_18]: https://link.springer.com/10.1007/s11356-022-22507-w

[^2_19]: https://doiserbia.nb.rs/Article.aspx?ID=0354-02432500037M

[^2_20]: http://www.emerald.com/ijoa/article/32/2/272-285/1226869

[^2_21]: http://link.springer.com/10.1007/s12351-017-0310-0

[^2_22]: https://link.springer.com/10.1007/s10479-024-05896-8

[^2_23]: http://arxiv.org/pdf/2311.17326.pdf

[^2_24]: https://www.shs-conferences.org/articles/shsconf/pdf/2021/27/shsconf_icsr2021_00070.pdf

[^2_25]: https://pmc.ncbi.nlm.nih.gov/articles/PMC9338582/

[^2_26]: http://downloads.hindawi.com/journals/sp/2017/7219656.pdf

[^2_27]: https://dx.plos.org/10.1371/journal.pone.0323735

[^2_28]: https://www.matec-conferences.org/articles/matecconf/pdf/2018/55/matecconf_rsp2018_04024.pdf

[^2_29]: https://www.youtube.com/watch?v=22LBNRMHGI0

[^2_30]: https://www.youtube.com/watch?v=vbSUsrgkZrE

[^2_31]: https://en.wikipedia.org/wiki/Problem_structuring_methods

[^2_32]: https://www.youtube.com/watch?v=i9J8cXkYuyM


---

# Structured questioning sequences for goal and value clarification in

clinical practice. How question ordering, type, and pacing surfaces
implicit objectives. Evidence from therapeutic and coaching contexts.
Distinguish from unstructured open questioning. Practitioner evidence
and clinical protocols preferred over theoretical treatment.

Several structured questioning sequences in clinical and coaching practice explicitly scaffold goal and value clarification, with evidence that ordering, type, and pacing of questions shape how implicit objectives emerge, in contrast to unstructured open questioning.[^3_1][^3_2][^3_3][^3_4][^3_5]

## Key structured sequences used clinically

- **Motivational Interviewing (MI) four‑process sequence**: Engagement → Focusing → Evoking → Planning, each with characteristic question types (relationship‑building questions, focus‑negotiating questions, discrepancy‑evoking questions, and action questions).[^3_6][^3_7][^3_8][^3_9]
- **CBT Socratic questioning protocols**: Stepwise sequences move from informational questions, through guided discovery, to synthesis around personally meaningful alternatives, rather than ad‑hoc challenges.[^3_4][^3_10]
- **Values clarification exercises in ACT and related therapies**: Manuals and practice papers describe structured moves from broad life domains, to candidate values, to “chosen directions” and concrete value‑consistent goals.[^3_3][^3_11]
- **Coaching frameworks such as GROW/GROWS**: Sessions follow Goal → Reality → Options → Will (and sometimes Self‑efficacy), with question sets pre‑specified for each phase.[^3_12][^3_5][^3_13]

These sequences are typically embedded in protocols or worksheets that spell out canonical questions for each step, distinguishing them from free‑form “any open question” interviewing.[^3_14][^3_11][^3_3]

## How ordering, type, and pacing surface implicit objectives

### Motivational Interviewing

- **Ordering**
    - MI intentionally delays goal negotiation until after engagement, so early questions emphasise understanding the client’s story and building alliance, not imposing goals.[^3_7][^3_6]
    - Focusing questions (“What would you like to focus on today?” “What change feels most important right now?”) then narrow to a shared goal topic, followed by evoking questions that elicit personal reasons and values behind change (e.g., “How would life be different if this changed?”).[^3_15][^3_8][^3_1]
- **Question types**
    - MI uses open questions plus reflections and scaling questions (e.g., readiness rulers) specifically to draw out desire, ability, reasons, and need (“change talk”) rather than factual detail.[^3_16][^3_6]
    - Value‑oriented questions (“What matters most to you about your health?”) are commonly recommended in MI‑consistent “What Matters to You?” conversations to link behavioural goals to higher‑order values.[^3_17][^3_8]
- **Pacing**
    - Guidelines emphasise slow pacing with frequent summaries; summaries consolidate emergent goals and values in the client’s own words, which often brings implicit objectives into focus (“So keeping up with your grandchildren and staying independent are really important to you…”).[^3_1][^3_6][^3_14]

Randomised and controlled studies plus systematic reviews show MI‑style structured conversations improve health behaviour change and goal adherence across multiple conditions compared with usual care or advice‑giving, with process research linking specific question sequences and evoked “change talk” to better outcomes.[^3_2][^3_18][^3_6]

### Socratic questioning in CBT

- **Staged sequence**
    - Clinical formulations of Socratic questioning describe four stages: (1) informational questions, (2) listening, (3) summarising, and (4) synthesising through guided discovery questions.[^3_4]
    - Within cognitive restructuring, scripts move from identifying the automatic thought, through evidence‑gathering (“What is the evidence for and against this?”), to perspective‑shifting (“If your friend were in this situation, what would you advise?”) and finally to constructing alternative meanings and action plans.[^3_10]
- **How it elicits goals/values**
    - Explicit protocols recommend questions that ask about consequences and desired outcomes (“If this belief were less strong, what would you be doing differently?”), which tends to surface implicit functional objectives, such as social connection or competence.[^3_10][^3_4]

Empirical work indicates that the quality and sequence of Socratic questions predict CBT symptom improvement above and beyond simple therapist support, suggesting that structured guided discovery is not equivalent to unstructured open questioning.[^3_4][^3_10]

### Values clarification in ACT and related therapies

- **Structured exercises and sequences**
    - ACT practice overviews describe using structured tools like values card sorts, life‑domain checklists, and written values worksheets that ask clients to identify what matters in specific domains (relationships, work, health, growth), then derive concrete goals and actions.[^3_11][^3_3]
    - Question sequences often start broad (“What gives you a sense of meaning?”) and progressively narrow to domain‑specific and situational values (“In your relationships, how do you want to act when things are difficult?”) and then to time‑bound committed actions.[^3_3][^3_11]
- **Ordering and pacing**
    - Protocols note that some clients struggle with highly open values questions; more structured sequences and prompts are recommended for those with limited “values language,” whereas unstructured discussion suits clients with an existing values repertoire.[^3_3]

Evidence syntheses and trials show that values clarification components, when implemented with structured exercises, are associated with greater alignment between goals and personal values and mediate improvements in functioning and quality of life in several conditions.[^3_3]

### Coaching protocols (GROW/GROWS)

- **Canonical sequence**
    - The GROW model uses a fixed order: clarify the Goal of the conversation, explore current Reality, brainstorm Options, and define Will/Way forward; question lists for each stage are widely used in coaching training and organisational development.[^3_5][^3_12]
    - The extended GROWS model inserts explicit Self‑efficacy questions after Will (e.g., “How confident are you on a scale from 1 to 10 that you can do this?”), which then triggers further questions to strengthen confidence.[^3_13]
- **Eliciting implicit objectives**
    - By first insisting on a clear session goal and desired longer‑term outcome, then contrasting this with current reality, these sequences systematically draw out discrepancies that reveal tacit priorities (for example, discovering that “being respected at work” matters more than specific task metrics).[^3_12][^3_5]

A qualitative evaluation of GROWS reported that adding structured self‑efficacy questions deepened clients’ sense of agency and clarified their motivation and commitment to change, compared with standard GROW conversations.[^3_13]

## Distinguishing structured sequences from unstructured open questioning

- **Explicit protocols vs ad‑hoc questioning**: MI, CBT Socratic questioning, ACT values exercises, and GROW‑type models all come with explicit manuals, question lists, and ordered phases; unstructured open questioning lacks this pre‑defined architecture.[^3_14][^3_5][^3_1][^3_3]
- **Functional targets**: Structured sequences are designed to evoke particular classes of client language (change talk, alternative cognitions, values statements, goals and plans) at specific points, whereas unstructured open questions may elicit a mix of narrative, complaint, and detail without systematically moving from values to goals to action.[^3_18][^3_6][^3_4]
- **Evidence base**: MI and CBT have extensive RCTs and process research; values‑focused ACT work and coaching models like GROW/GROWS have smaller but growing empirical literatures, with studies showing that structured questioning improves clarity of goals and values, commitment, and behaviour change compared to more diffuse discussion.[^3_2][^3_6][^3_13][^3_3]

If you plan to adapt one of these sequences for a non‑clinical, work‑focused setting, which context is primary for you right now (e.g., health behaviour change, mental health, or performance coaching in organisations)?
<span style="display:none">[^3_19][^3_20][^3_21][^3_22][^3_23]</span>

<div align="center">⁂</div>

[^3_1]: https://pmc.ncbi.nlm.nih.gov/articles/PMC2719555/

[^3_2]: https://pmc.ncbi.nlm.nih.gov/articles/PMC8200683/

[^3_3]: https://pmc.ncbi.nlm.nih.gov/articles/PMC8854463/

[^3_4]: https://www.cambridge.org/core/journals/bjpsych-advances/article/socratic-questioning-put-into-clinical-practice/8C44C0BF33871FB55349695407700738

[^3_5]: https://www.susannemadsen.co.uk/uploads/6/3/2/3/6323088/grow_coaching_questions.pdf

[^3_6]: https://pmc.ncbi.nlm.nih.gov/articles/PMC3330017/

[^3_7]: https://psychcentral.com/pro/the-four-processes-of-motivational-interviewing

[^3_8]: https://www.sciencedirect.com/science/article/pii/S0033062023000099

[^3_9]: https://cdpsdocs.state.co.us/epic/epicwebsite/resources/mi_communities_of_practice/4_processes/4_processes.pdf

[^3_10]: https://dialecticalbehaviortherapy.com/cbt/cognitive-restructuring/socratic-questions-script/

[^3_11]: https://www.simplepractice.com/resource/values-clarification-worksheet/

[^3_12]: https://www.ucl.ac.uk/human-resources/sites/human-resources/files/using_grow_questions_1.pdf

[^3_13]: https://centaur.reading.ac.uk/104381/1/Final Revision - Panchal and Riddell Research Paper_27th%20Feb%202020%5B1%5D.pdf

[^3_14]: https://pmc.ncbi.nlm.nih.gov/articles/PMC6342439/

[^3_15]: https://www.motivationalinterviewing.org/sites/default/files/Teaching the Four Processes.pdf

[^3_16]: https://thewellnesssociety.org/6-types-of-motivational-interviewing-questions-for-therapists/

[^3_17]: https://pmc.ncbi.nlm.nih.gov/articles/PMC11822820/

[^3_18]: https://www.aclweb.org/anthology/W15-1209.pdf

[^3_19]: https://ojs.mruni.eu/ojs/social-work/article/view/6502

[^3_20]: https://pmc.ncbi.nlm.nih.gov/articles/PMC6529989/

[^3_21]: https://pmc.ncbi.nlm.nih.gov/articles/PMC6488959/

[^3_22]: https://positivepsychology.com/motivational-interviewing/

[^3_23]: https://www.anxiousminds.co.uk/cbt-tools-socratic-questioning/


---

# Socratic questioning as a structured elicitation method in education

and clinical ethics. Evidence for how question sequencing changes the
quality and specificity of articulated goals or positions. Practitioner
evidence and empirical studies. NOT philosophical commentary on Socratic
method in the abstract.

Socratic questioning is used as a structured elicitation method in both education and clinical ethics, with empirical work showing that planned sequences of question types can make learners’ or clinicians’ positions more explicit, specific, and reason‑giving than unstructured dialogue or lectures.[^4_1][^4_2][^4_3][^4_4][^4_5]

## Structured Socratic sequences in education

- Studies in secondary and higher education typically operationalise Socratic questioning using taxonomies of question types (clarification, probing assumptions, probing reasons/evidence, alternative viewpoints, implications, and meta‑questions) and require teachers to sequence these deliberately in classroom discussions.[^4_2][^4_6][^4_7]
- Action‑research and quasi‑experimental designs in language and subject teaching show that repeated cycles of such structured questioning improve students’ critical thinking, reading, and writing, compared with traditional teaching or unplanned questioning.[^4_8][^4_9][^4_1][^4_2]

Mechanistically, the **ordering** usually moves from clarification (“What do you mean by…?”) to justification (“What’s your reason for that?”), then to challenges to assumptions and alternative perspectives, and finally to consequences and synthesis, which pushes students from vague opinions toward more precise, justified positions or goals.[^4_7][^4_10][^4_2][^4_8]

- In a quasi‑experimental study of Turkish 6th‑grade language classes, instruction based on Socratic questioning led to significantly higher post‑test scores in critical thinking, critical reading, and creative thinking than conventional teaching, with the authors attributing gains to structured, tiered discussions rather than isolated open questions.[^4_1]
- An action‑research study in EFL writing found that cycles of Socratic questioning improved the specificity and argumentative quality of students’ written responses; field notes and interview data indicated that moving systematically through clarification → probe reasons → explore alternatives helped students articulate clearer thesis statements and support.[^4_2]
- In online language classes using Nominal Group Technique plus Socratic questioning, pre‑experimental data suggested increased critical thinking and engagement; the protocol explicitly required teachers to scaffold from comprehension questions to analytic and evaluative questions in a fixed order.[^4_8]

Recent work on “Socratic questioning 2.0” and digital Socratic dialogue (e.g., AI‑mediated questioning in physics) also emphasises structured prompt sequences rather than ad‑hoc questioning, and reports high perceived learning and engagement when students are led through staged conceptual clarification and reasoning prompts.[^4_11][^4_12][^4_13]

## Structured Socratic questioning in clinical and nursing ethics

- In nursing and healthcare ethics education, Socratic questioning has been embedded in ethics courses and case‑based seminars to move students from intuitive reactions toward explicit moral reasoning and articulated value positions.[^4_14][^4_3][^4_4][^4_5]
- A quasi‑experimental study comparing Socratic questioning with lectures in nursing ethics found that both improved moral reasoning scores, but the Socratic group gained more, leading the authors to conclude that structured questioning is a more effective method for developing moral reasoning competence.[^4_4]

Ethics‑focused implementations generally use **ill‑defined clinical scenarios** followed by sequenced questions that ask students to:

1) clarify the problem and stakeholders,
2) identify relevant values and principles,
3) examine assumptions and conflicting considerations, and
4) reason toward and defend a course of action.[^4_5][^4_4]

- A study implementing Socratic inquiry, reflection, and argumentation in nursing education used ill‑defined case scenarios with structured questioning and guided argument; qualitative analysis showed students refining care plans by clarifying misconceptions, weighing opposing stances, and adjusting previously skewed views.[^4_5]
- Earlier work combining Socratic discussion with “learning through discussion” in nursing courses reported, via questionnaires and qualitative feedback, that students became more able to articulate and justify decisions in clinical situations, although adaptation issues (e.g., discomfort with being questioned) needed management.[^4_14]

While not labelled “clinical ethics” per se, CBT‑oriented clinical protocols on Socratic questioning in psychiatric practice also describe a four‑stage structure (information → listening → summarising → synthesising) that moves patients from diffuse concerns to specific, testable alternative appraisals and goals, and this model has influenced some health‑professional education in ethical and clinical reasoning.[^4_3][^4_15]

## How sequencing affects quality and specificity of positions/goals

Across these domains, several consistent features distinguish structured Socratic sequences from unstructured open questioning:

- **Planned progression of cognitive operations**: Question sets are designed to move from description to analysis to evaluation and synthesis, rather than mixing question types randomly; this progression is reported to increase the **specificity** and **justification density** in student and trainee responses.[^4_3][^4_1][^4_2][^4_5]
- **Use of question categories**: Protocols often follow or adapt Paul’s taxonomy (questions of clarification, assumptions, reasons/evidence, viewpoints, implications, and meta‑questions), and teachers are trained to step through these categories deliberately.[^4_16][^4_17][^4_7][^4_3]
- **Repetition and pacing**: Studies emphasise repeated practice over weeks or months, with time allowed for reflection; slower pacing and recurring summarisation points appear important for enabling learners to revise and sharpen their articulated stances.[^4_2][^4_14][^4_3][^4_5]

For example, in medical biochemistry teaching, a structured Socratic “learning sheet” guided students through questions on purpose, assumptions, evidence, and implications; evaluation showed improvements in multiple dimensions of critical thinking and metacognitive monitoring, suggesting the sequence helped students articulate and refine their reasoning rather than just recall content.[^4_3]

## Practitioner protocols, tools, and contrasts with unstructured questioning

- **Nursing/clinical practice tools**: Clinical teaching resources such as “Socratic Questions for Clinical Practice” provide structured lists of clarification, priority‑setting, reasoning, and perspective‑taking questions for supervisors to use at the bedside (e.g., “What are the most important client problems? Why?”, “What other possibilities could explain this?”).[^4_18]
- **Educational practice reports**: Classroom‑based studies (e.g., in Islamic religious education, language arts, and healthcare education) document teachers using six‑type Socratic question sequences in tiered dialogues; observation and interview data suggest that these structured tiers encourage students to explain concepts, link arguments, evaluate implications, and consider alternative views more consistently than in classes dominated by closed or unplanned questions.[^4_19][^4_16][^4_3]

Systematic and narrative reviews on questioning as a high‑level cognitive strategy consistently distinguish between **planned, hierarchical questioning patterns** and general open questioning, noting that the former are associated with stronger gains in critical thinking, reasoning, and engagement across multiple studies and disciplines.[^4_6][^4_7][^4_3]

In both education and clinical ethics‑related teaching, then, Socratic questioning functions as a **structured elicitation** method: by sequencing question types and pacing them over time, practitioners can help learners and clinicians move from implicit or intuitive stances to explicit, specific, and reasoned goals or ethical positions, in ways that are measurably different from unstructured open‑ended questioning or lecture‑based teaching.[^4_4][^4_1][^4_5][^4_2][^4_3]

To tailor this further, would it be more useful for you if I concentrate next on concrete question‑by‑question templates for ethics case discussions, or on empirical measures used to assess changes in quality/specificity of positions under Socratic protocols?
<span style="display:none">[^4_20][^4_21][^4_22][^4_23][^4_24][^4_25][^4_26][^4_27][^4_28][^4_29][^4_30][^4_31][^4_32][^4_33]</span>

<div align="center">⁂</div>

[^4_1]: https://ijonmes.net/index.php/ijonmes/article/view/424

[^4_2]: http://www.journals.aiac.org.au/index.php/IJELS/article/download/2683/2294

[^4_3]: https://pmc.ncbi.nlm.nih.gov/articles/PMC10026783/

[^4_4]: https://pubmed.ncbi.nlm.nih.gov/27694549/

[^4_5]: https://pmc.ncbi.nlm.nih.gov/articles/PMC12505419/

[^4_6]: https://ccsenet.org/journal/index.php/elt/article/download/53031/28389

[^4_7]: https://www.criticalthinking.org/pages/the-role-of-socratic-questioning-in-thinking-teaching-amp-learning/522

[^4_8]: http://jurnal.unsyiah.ac.id/SiELE/article/download/22352/15848

[^4_9]: https://www.semanticscholar.org/paper/The-Socratic-Method:-Empirical-Assessment-of-a-Burns-Stephenson/bda374467176af3ca0ef1a5151c8cb6fc0719d97

[^4_10]: https://positivepsychology.com/socratic-questioning/

[^4_11]: https://journal.um-surabaya.ac.id/Tell/article/view/26322

[^4_12]: https://www.mdpi.com/2227-7102/16/2/184

[^4_13]: https://aclanthology.org/2022.emnlp-main.277.pdf

[^4_14]: https://curationis.org.za/index.php/curationis/article/download/894/831

[^4_15]: https://www.cambridge.org/core/journals/bjpsych-advances/article/socratic-questioning-put-into-clinical-practice/8C44C0BF33871FB55349695407700738

[^4_16]: https://jurnal.itscience.org/index.php/educendikia/article/view/7329

[^4_17]: https://www.authorea.com/users/537437/articles/606327/master/file/data/essoar/essoar.10510608.1.pdf

[^4_18]: https://www.keithrn.com/site/wp-content/uploads/2017/02/Socratic-Questions-for-Clinical-Practice-handout.pdf

[^4_19]: https://journal2.upgris.ac.id/index.php/paudia/article/view/2377

[^4_20]: https://ir.uitm.edu.my/id/eprint/131062/1/131062.pdf

[^4_21]: https://ejournal.amirulbangunbangsapublishing.com/index.php/jpnmb/article/view/656

[^4_22]: http://eudl.eu/doi/10.4108/eai.14-10-2024.2356590

[^4_23]: https://link.springer.com/10.1007/s40889-023-00161-1

[^4_24]: http://gcbss.org/CIMSSR2025INDONESIA/CIMSSR-00252.html

[^4_25]: http://online-journals.org/index.php/i-jac/article/download/4442/3523

[^4_26]: https://onlinelibrary.wiley.com/doi/10.1002/tesj.601

[^4_27]: https://www.youtube.com/watch?v=L8YJdM--vr8

[^4_28]: https://www.youtube.com/watch?v=_tnQcSR1zJI

[^4_29]: https://www.youtube.com/watch?v=ImxtXXJjjIw

[^4_30]: https://www.youtube.com/watch?v=fIU5uT1stEk

[^4_31]: https://scholar.google.com/citations?view_op=view_citation\&hl=en\&user=fHgmV5kAAAAJ\&citation_for_view=fHgmV5kAAAAJ%3AqjMakFHDy7sC

[^4_32]: https://www.youtube.com/watch?v=p5LyS9spQ_o

[^4_33]: https://discovery.researcher.life/article/qualitative-observations-of-student-reasoning/ab42ceb2fc473c2582d3cc2c6cffcad4


---

# Intent disambiguation in dialogue systems and conversational AI. Methods

for iterative clarification beyond single-turn interpretation. Slot-filling
vs open-ended clarification strategies. Empirical evaluation of clarification
effectiveness. Research from NLP, dialogue systems, and human-AI interaction.

Iterative intent disambiguation in conversational systems is handled through combinations of confidence‑aware routing, explicit clarification subdialogues, and mixed slot‑filling / open‑ended strategies, with growing empirical work on when and how clarification improves task success and user experience.[^5_1][^5_2][^5_3][^5_4]

## Core methods for iterative clarification

- **Confidence‑based clarification triggers**: Many task‑oriented systems use NLU confidence thresholds to decide whether to answer, ask a targeted clarification, or fall back, sometimes using distinct thresholds for “confirm top intent” vs “disambiguate between multiple intents.”[^5_5][^5_1]
- **Intent‑ranking and disambiguation dialogues**: Work on intent disambiguation in task‑oriented dialogue exposes the top‑N likely intents, then generates a clarifying question listing or contrasting these options (e.g., “Are you asking to X, Y, or Z?”), with user responses fed back into the classifier in multi‑turn fashion.[^5_4][^5_1]
- **Multi‑stage clarification for QA and search**: In conversational QA, multi‑stage frameworks reason about ambiguity, ask follow‑up questions, then refine logical forms or queries in subsequent turns rather than relying on a single clarification opportunity.[^5_6][^5_2][^5_3]
- **Plan/goal recognition with queries**: Sequential plan recognition work chooses questions that maximally reduce uncertainty among competing plans/hypotheses, asking “Is your goal G?” or “Will you do action A next?” and updating its belief state iteratively.[^5_7]

These methods treat clarification as a subdialogue with its own state and policy, rather than a one‑off reaction to a single ambiguous turn.[^5_2][^5_5]

## Slot‑filling vs open‑ended clarification

### Slot‑filling strategies

- **Form‑style elicitation**: Classic task bots use slot‑filling: once an intent is chosen, the system asks a series of targeted questions to fill missing slots (e.g., origin, destination, date), often in a fixed or learned order.[^5_8][^5_5]
- **Slot updates and repairs**: Real conversational data show users revise or correct slot values mid‑utterance (“Thursday… actually Friday afternoon”), requiring models to treat clarification as slot repair and overwriting rather than simple filling.[^5_9]

Slot‑filling clarifications are narrow, closed or highly constrained (e.g., “Which city are you flying from?”), which simplifies NLU and supports downstream APIs, but can feel rigid and fail when the intent itself is unclear or multi‑goal.[^5_9][^5_8]

### Open‑ended clarification strategies

- **Free‑form follow‑ups**: Open‑ended clarifications ask the user to elaborate or restate, sometimes with hints (“Could you tell me more about what you’re trying to do?”), or pose contrastive questions that invite explanation rather than simple selection.[^5_10][^5_2][^5_5]
- **Hierarchical facet clarifications**: Systems like AmbigChat detect ambiguous facets (e.g., entity, attribute, time frame) and ask higher‑level questions such as “Which product are you referring to?” before moving to more specific slot questions.[^5_3]

Open‑ended clarifications can better handle under‑specified or mixed intents, and can surface user constraints not represented as slots, but they increase NLU complexity and can be harder to evaluate automatically.[^5_2][^5_3][^5_9]

### Hybrid approaches

Modern systems often combine these approaches: first disambiguate at the intent/facet level (often with semi‑open or list‑based questions), then use more traditional slot‑filling within the chosen task.[^5_1][^5_3][^5_2]

## Example iterative clarification patterns

- **Intent disambiguation for contact‑centre virtual assistants**: One deployed system detects ambiguous queries before intent classification, then presents a clarification question constructed from the top‑N intents; experiments on real contact‑centre data show statistically significant improvements in intent disambiguation accuracy and mean reciprocal rank over popularity‑based and pure ranking baselines.[^5_1]
- **Discriminative clarifying questions**: Another approach retrieves or generates clarifying questions that are maximally discriminative for a pair of candidate intents (e.g., contrasting attributes or actions). It uses a trained intent classifier plus a question generator, selecting the question whose expected answers best separate the intents, and falls back to template questions when needed.[^5_4]
- **Multi‑stage clarification in conversational QA**: A proposed QA framework runs ambiguity detection, then a clarification stage that asks targeted questions, then answer generation; in experiments, clarification leads to higher answer accuracy on ambiguous questions than either answering directly or providing generic error messages.[^5_2]
- **Clarification‑enhanced KGQA**: CLEAR‑KGQA quantifies entity and intent ambiguity in questions over knowledge graphs, uses a Bayesian mechanism to decide whether to clarify, and then iteratively refines candidate logical forms with user input, improving performance on WebQSP and CWQ compared with non‑interactive baselines.[^5_6]
- **Enterprise AI assistants (ECLAIR)**: ECLAIR uses multiple agents to reason about ambiguity and generate clarification questions, integrating signals across tools; experiments on enterprise data show better clarification question quality and ambiguity resolution than few‑shot prompting baselines.[^5_11][^5_10]


## Empirical evaluation of clarification effectiveness

Clarification mechanisms are typically evaluated along several axes:

- **Task performance**
    - Intent disambiguation accuracy, intent MRR, and overall task success (e.g., correct routing, successful completion of a transaction) improve when clarification subdialogues are used compared to non‑interactive baselines.[^5_6][^5_4][^5_1][^5_2]
    - In KGQA and QA, clarification increases exact‑match or F1 scores on ambiguous queries versus directly answering or asking users to rephrase.[^5_6][^5_2]
- **Clarification question quality**
    - Some work uses automatic metrics (e.g., BERTScore, discriminative power between intent candidates) and human ratings to assess whether clarifying questions are understandable, minimally intrusive, and actually disambiguate the intended dimension.[^5_11][^5_3][^5_4]
- **Interaction flow and user experience**
    - Studies in conversational search and QA report that well‑timed clarifications reduce user frustration compared to generic fallbacks, but poorly targeted or overly frequent clarifications harm perceived intelligence and efficiency, emphasizing the need for calibrated triggering policies.[^5_12][^5_3][^5_2]

Human–AI interaction work on large‑model assistants generally highlights that leveraging conversation history for context, and asking selective, context‑aware follow‑ups, improves perceived naturalness and responsiveness, though systematic metrics for clarification effectiveness in open‑domain settings remain sparse.[^5_13][^5_14][^5_12]

## Iterative disambiguation beyond single‑turn interpretation

Beyond local single‑turn fixes, several strands treat disambiguation as a **multi‑turn decision problem**:

- **Sequential plan/intent recognition**: Systems model a sequence of possible user plans and choose queries that maximally reduce hypothesis space over time, updating beliefs after each answer.[^5_7]
- **Iterative clarify–retrieve–filter loops**: Multi‑turn academic recommendation and similar agents learn policies that interleave clarification with retrieval and filtering, using reinforcement learning over long dialogues to decide when to clarify and what to ask.[^5_15]
- **Verifier‑assisted iterative prompting**: Frameworks like CLAIRIFY explicitly separate generation and verification, using a verifier to inspect outputs, identify ambiguities or mismatches with user intent, and drive further clarifying turns until a stopping criterion is reached.[^5_16]

These approaches move intent understanding from static classification to a **sequential decision‑making** problem, with clarification treated as an action whose long‑term value is learned or optimized.[^5_15][^5_16][^5_7]

Would it be most useful for your purposes if I next map these methods into a compact table (dimensions: ambiguity detection, clarification style, evaluation metrics), or would you prefer design guidance for implementing hybrid slot‑filling/open‑ended clarification in a specific domain (e.g., support, search, recommendation)?
<span style="display:none">[^5_17][^5_18][^5_19][^5_20][^5_21][^5_22][^5_23][^5_24][^5_25][^5_26][^5_27][^5_28][^5_29][^5_30][^5_31][^5_32][^5_33]</span>

<div align="center">⁂</div>

[^5_1]: https://dl.acm.org/doi/10.1145/3511808.3557516

[^5_2]: http://arxiv.org/pdf/2110.15235.pdf

[^5_3]: https://dl.acm.org/doi/full/10.1145/3746059.3747686

[^5_4]: https://arxiv.org/html/2008.07559v2

[^5_5]: https://web.stanford.edu/~jurafsky/slp3/old_dec20/24.pdf

[^5_6]: https://ieeexplore.ieee.org/document/11229206/

[^5_7]: https://www.sciencedirect.com/science/article/pii/S0004370218301103

[^5_8]: https://boost.ai/blog/making-strides-towards-natural-dialogue-in-broad-scope-virtual-agents/

[^5_9]: https://www.annotera.ai/blog/nuances-of-slot-filling-conversational-speech/

[^5_10]: http://arxiv.org/pdf/2503.20791.pdf

[^5_11]: https://arxiv.org/html/2503.15739v1

[^5_12]: https://www.frontiersin.org/journals/artificial-intelligence/articles/10.3389/frai.2024.1418869/full

[^5_13]: http://arxiv.org/pdf/2403.00662.pdf

[^5_14]: https://pmc.ncbi.nlm.nih.gov/articles/PMC11564924/

[^5_15]: https://ieeexplore.ieee.org/document/11397045/

[^5_16]: https://www.emergentmind.com/topics/verifier-assisted-iterative-prompting-clairify

[^5_17]: http://link.springer.com/10.1007/b105612

[^5_18]: https://link.springer.com/10.1007/978-3-642-10291-2

[^5_19]: http://link.springer.com/10.1007/978-3-540-74782-6

[^5_20]: https://onlinelibrary.wiley.com/doi/10.1002/jso.20825

[^5_21]: https://ajph.aphapublications.org/doi/full/10.2105/AJPH.92.7.1054

[^5_22]: https://www.semanticscholar.org/paper/28833eef79330b20184e569d2e3675c965bdb510

[^5_23]: https://www.semanticscholar.org/paper/b4c3ebd1de99af783a7bfd0cd3c92e4d2cf1dd03

[^5_24]: https://arxiv.org/pdf/2008.07559.pdf

[^5_25]: https://aclanthology.org/2023.findings-emnlp.359.pdf

[^5_26]: https://arxiv.org/pdf/2310.05592.pdf

[^5_27]: https://arxiv.org/pdf/2104.08964.pdf

[^5_28]: https://arxiv.org/html/2411.06022v1

[^5_29]: https://aclanthology.org/2025.emnlp-main.482.pdf

[^5_30]: https://papers.ssrn.com/sol3/Delivery.cfm/04e0a839-35eb-4f92-ab6e-4d8c33f50576-MECA.pdf?abstractid=5165685\&mirid=1

[^5_31]: https://onlinelibrary.wiley.com/doi/10.1002/tesq.3409

[^5_32]: https://www.jeffjianzhao.com/papers/uxva.pdf

[^5_33]: https://arxiv.org/html/2509.04472v2


---

# Depth interview techniques for surfacing implicit motivations and values

behind stated preferences. Structured elicitation methods from psychology,
consumer research, and design research. Evidence for validity and
practitioner use. NOT marketing summaries — primary methodology and
empirical studies.

Depth interview methods like laddering and metaphor‑elicitation provide structured ways to move from stated preferences to implicit motivations and values, with empirical use in psychology, consumer, and design research beyond marketing gloss.[^6_1][^6_2][^6_3][^6_4][^6_5]

## Means–End laddering interviews

- **Method structure**
    - Laddering operationalises means–end chain theory by repeatedly probing from concrete attributes → perceived consequences → personal values using “why is that important to you?” questions in one‑to‑one depth interviews.[^6_6][^6_3][^6_7]
    - Interviewers start from elicited attributes (e.g., features, choices), then iteratively ask tailored “why” questions until respondents articulate higher‑order benefits (functional/psychosocial) and eventually terminal values (e.g., security, autonomy, social approval).[^6_3][^6_7]
- **Evidence and applications**
    - Systematic and case studies apply laddering to farmers’ adoption of climate‑smart practices, organic food consumption, agricultural certification, insect‑based foods, residential preferences, and patient experiences, showing it can map from behavioural choices to core values.[^6_8][^6_9][^6_10][^6_11][^6_2][^6_1]
    - A systematic review on patient laddering in hospitals found hierarchical value mapping (aggregating individual ladders) useful for identifying core patient value themes beyond standard satisfaction scores, supporting design decisions about care processes and environments.[^6_2]
    - Recent work in healthcare built environments integrates laddering with design documents and observations (i3 method) to link spatial attributes to service outcomes and user values, demonstrating feasibility and perceived usefulness for multi‑stakeholder value clarification.[^6_12]
- **Validity and limitations**
    - Methodological critiques note risks of “artificial abstraction” and rationalisation when respondents feel forced up the ladder, and challenges when people lack prior reflection on deep motives; these are addressed with careful probing, stopping rules, and triangulation.[^6_7][^6_2][^6_3]


## Zaltman Metaphor Elicitation Technique (ZMET)

- **Method structure**
    - ZMET asks participants to collect images representing their thoughts/feelings about a topic, then uses a lengthy semi‑structured interview to probe each image, elicit metaphors, construct mental maps, and identify deeper constructs (values, identity, emotions) underpinning expressed preferences.[^6_4][^6_13][^6_14]
    - Interviews use a sequence of prompts (storytelling about images, missing images, sensory probes, opposite images) before co‑constructing a consensus map across participants.[^6_13][^6_14]
- **Evidence and use**
    - A recent systematic review of 47 ZMET studies (2019–2023) finds frequent use for exploring experience, emotion, identity, values, and decision‑making, and concludes ZMET effectively uncovers “hidden layers of meaning,” especially where experiences are complex or affect‑laden.[^6_4][^6_13]
    - Case studies report that combining ZMET with grounded theory and in‑depth interviews yields rich conceptual structures that align with psychological theories (e.g., schemas, implicit beliefs), supporting its use as a bridge between theory and qualitative data.[^6_14][^6_13]
- **Validity considerations**
    - The review highlights strengths in accessing non‑verbalised meanings and weaknesses around analytic complexity and subjectivity, recommending rigorous planning, interviewer training, and triangulation for credible inferences about values.[^6_4]


## Generative and contextual depth interviews in design research

- **Generative toolkits + semi‑structured interviews**
    - Generative design research methods (e.g., generative focus groups, Experience Reflection Modelling) combine artefact creation (collages, maps, probes) with one‑to‑one or small‑group semi‑structured interviews to elicit tacit knowledge and latent needs users cannot easily verbalise.[^6_5][^6_15]
    - The interview sequences typically move from concrete recounting of activities, to discussion of created artefacts, to reflective prompts about why certain elements matter and what ideal futures would look like, surfacing underlying motives and values.[^6_15][^6_5]
- **Evidence and practitioner reports**
    - Design research case work argues that pairing interviews with contextual observation and re‑enactments better reveals latent needs than interviews alone, because participants can demonstrate and then explain situated practices and frustrations.[^6_5][^6_15]

These methods contrast with unstructured conversational interviews by prescribing **staged moves** (e.g., concrete → consequence → value, or artefact → story → reflection) and often using explicit coding frameworks (hierarchical value maps, consensus maps, theme structures) to link expressed preferences to deeper motivations.[^6_2][^6_3][^6_13][^6_15]

## Validity, implicit constructs, and practitioner use

- **Construct validity for motivations/values**
    - Means–end chain applications consistently treat values as the highest level in interview data structures and use hierarchical value maps to check that elicited value themes cohere across respondents; healthcare and built‑environment studies use this to design or redesign services around empirically grounded value hierarchies.[^6_1][^6_12][^6_2]
    - ZMET’s systematic review notes that its findings line up with cognitive‑psychological notions of schemas and unconscious meaning structures, supporting its use to probe beliefs, values, and emotions that are hard to reach with direct questioning alone.[^6_13]
- **Reliability and interviewer effects**
    - Laddering methodology papers discuss interviewer skill and persistence as key sources of variation; recommendations include training, piloting, careful question tracking, and stopping rules to mitigate bias and fatigue effects.[^6_3][^6_7]
- **Extent of practitioner adoption**
    - Laddering and means–end analysis are now used beyond commercial branding, in agriculture, food ethics, housing, healthcare, and environmental practice, indicating cross‑domain uptake for value‑level elicitation in real‑world projects.[^6_9][^6_10][^6_12][^6_8][^6_1][^6_2]
    - ZMET is widely used in qualitative psychological and experience research, especially where emotional and identity‑laden topics require richer, metaphor‑based elicitation.[^6_14][^6_13][^6_4]
    - Generative design interviews and contextual inquiries are standard techniques in human‑centred design practice for surfacing tacit needs and motivations that users cannot easily state as “requirements.”[^6_15][^6_5]

Would it help you most if I next lay out a compact table comparing laddering, ZMET, and generative design interviews on structure, kind of implicit construct surfaced, and evidence base, or are you more interested in detailed interview scripts/protocol moves for one of these methods?
<span style="display:none">[^6_16][^6_17][^6_18][^6_19][^6_20][^6_21][^6_22][^6_23][^6_24][^6_25][^6_26][^6_27][^6_28][^6_29][^6_30][^6_31]</span>

<div align="center">⁂</div>

[^6_1]: https://www.tandfonline.com/doi/full/10.1080/17565529.2018.1442786

[^6_2]: https://pmc.ncbi.nlm.nih.gov/articles/PMC7786779/

[^6_3]: https://nsuworks.nova.edu/tqr/vol11/iss4/1/

[^6_4]: https://ejurnal.mercubuana-yogya.ac.id/index.php/psikologi/article/view/4505

[^6_5]: https://www.hfes-europe.org/wp-content/uploads/2016/11/Jentsch2017.pdf

[^6_6]: https://en.wikipedia.org/wiki/Ladder_interview

[^6_7]: https://nsuworks.nova.edu/cgi/viewcontent.cgi?article=1651\&context=tqr

[^6_8]: https://link.springer.com/10.1007/s10901-023-10017-1

[^6_9]: http://www.ingentaconnect.com/content/10.14485/HBPR.5.2.4

[^6_10]: http://link.springer.com/10.1007/s10806-015-9572-9

[^6_11]: http://link.springer.com/10.1007/978-3-319-74011-9_25

[^6_12]: https://journals.sagepub.com/doi/10.1177/19375867251353734

[^6_13]: https://ejurnal.mercubuana-yogya.ac.id/index.php/psikologi/article/download/4505/1827/15253

[^6_14]: https://eprints.bournemouth.ac.uk/39186/1/Binder1.pdf

[^6_15]: https://openjournals.ljmu.ac.uk/DesignTechnologyEducation/article/download/1782/920/5561

[^6_16]: https://periodicos.ufpe.br/revistas/cbr/article/view/265486

[^6_17]: https://linkinghub.elsevier.com/retrieve/pii/S0736585321001039

[^6_18]: https://journals.sagepub.com/doi/10.1177/10963480221103224

[^6_19]: https://pmc.ncbi.nlm.nih.gov/articles/PMC6687518/

[^6_20]: https://pmc.ncbi.nlm.nih.gov/articles/PMC9983757/

[^6_21]: https://pmc.ncbi.nlm.nih.gov/articles/PMC7849589/

[^6_22]: https://www.scielo.br/j/bar/a/tMVwXYBdYkcBktKyw78Wvnq/?format=pdf\&lang=en

[^6_23]: https://journals.sagepub.com/doi/pdf/10.1177/14707853231184742

[^6_24]: https://lirias.kuleuven.be/bitstream/20.500.12942/702335/2/smac025.pdf

[^6_25]: https://pmc.ncbi.nlm.nih.gov/articles/PMC8041053/

[^6_26]: https://www.newtonx.com/article/unlocking-value-with-the-laddering-method/

[^6_27]: https://www.entropik.io/resources/blog-articles/in-depth-interviews-and-their-use-in-consumer-research

[^6_28]: https://www.uxmatters.com/mt/archives/2009/07/laddering-a-research-interview-technique-for-uncovering-core-values.php

[^6_29]: https://borderlessaccess.com/blog/the-value-of-in-depth-interviews-to-assess-consumer-behavior/

[^6_30]: https://www.rajivgopinath.com/blogs/marketing-hub/fundamentals-of-marketing/research-methodologies/intermediate/the-art-of-laddering-interviews-in-brand-equity-studies

[^6_31]: https://nexusexpertresearch.co/blog/when-to-use-in-depth-interviews/


---

# Implicit preference modeling and intent inference from partial or indirect

user signals. Methods for inferring goals, priorities, or objectives when
users cannot fully articulate them. Research from recommender systems,
adaptive interfaces, assistive technology, and behavioral signal processing.
Applications in populations with communication or executive function barriers.
NOT sentiment analysis or emotion detection.

Implicit preference and intent inference from partial signals is usually framed as learning latent user goals from interaction traces, contextual cues, and behavioral patterns, with some work explicitly targeting users who cannot fully articulate objectives.[^7_1][^7_2][^7_3][^7_4]

## Recommender systems: inferring goals from implicit feedback

- **Implicit feedback modeling**
    - Implicit feedback recommenders treat behaviors such as clicks, dwell time, purchases, skips, and replays as noisy indicators of underlying preference, rather than explicit ratings.[^7_5][^7_1]
    - Matrix factorization, NMF, and modern deep models learn latent user and item factors from these signals, sometimes integrating exposure models to distinguish lack of interest from lack of opportunity.[^7_6][^7_7][^7_8][^7_1]
    - Sequential and multi‑feedback models explicitly separate short‑term session goals from long‑term tastes by modelling sequences of actions and multiple behavior types (view, add‑to‑cart, purchase) with recurrent or attention‑based architectures.[^7_9][^7_10][^7_11]
- **Handling noise and bias**
    - Work on unbiased implicit feedback and exposure‑aware models uses causal or bi‑level optimization to correct for position bias and missing‑not‑at‑random data, improving the fidelity of inferred preferences.[^7_12][^7_7][^7_13]
    - Other approaches identify unexpected or noisy behaviors and discount them to avoid misinterpreting accidental clicks as genuine interest.[^7_14][^7_15]
- **Beyond “like”: richer goals and strategic behavior**
    - Some models acknowledge that users choose content strategically to influence future recommendations, framing interaction as a signalling game rather than a direct expression of preference, and adapting policies accordingly.[^7_16]
    - Goal‑focused recommenders like GoalPods let users specify high‑level learning or mood goals and then infer suitable content within those constraints, revealing that implicit traces alone often miss users’ broader objectives.[^7_17]


## Adaptive interfaces and user‑state inference

- **Multimodal and psycho‑ecological modeling**
    - A generic framework for inferring user states in HCI uses multimodal observations (interaction patterns, context sensors, sometimes physiology) within probabilistic models (e.g., dynamic Bayesian networks) to infer latent states such as goals or workloads and adapt the interface.[^7_3]
    - A recent psycho‑ecological model of user behavior on digital platforms builds dual‑channel representations of psychological and ecological signals, using attention mechanisms to infer motivational embeddings (e.g., information‑seeking, social connection) that drive future behavior.[^7_18]
- **From implicit interaction to adaptive support**
    - Surveys of implicit‑feedback recommendation emphasise that many applications must infer preferences without explicit ratings, relying on clickstreams, navigation paths, dwell times, and revisits to personalize content and layout.[^7_1][^7_5]
    - Structured memory approaches for LLM‑based agents treat each observed behavior as evidence for specific interest “atoms,” organizing and evolving these in memory to infer multi‑faceted and changing user goals from sparse signals.[^7_19]

These approaches operationalise “intent inference” as learning latent variables that best explain observed sequences and context, then using them to drive ranking, adaptation, or prompting.

## Assistive technology and executive‑function support

- **Goal‑directed behavior with limited articulation**
    - Assistive technologies for cognition (ATC) aim to compensate for executive dysfunction (e.g., after acquired brain injury), supporting goal formulation, planning, initiation, and monitoring of activities of daily living.[^7_20][^7_21][^7_4]
    - A scoping review of ATC for executive function notes that most tools support prospective memory (reminders) and step sequencing, but highlights goal formulation as under‑addressed and calls for richer user‑centred methods and sensing to infer user goals.[^7_4]
- **Behavior‑driven adaptation**
    - A single‑case experimental protocol for smart home, mobile, and wearable technologies in ABI uses detailed baseline and intervention logs of target behaviors to infer how technology support changes goal‑directed activity, effectively treating behavioral change patterns as evidence of successful goal support.[^7_21][^7_20]
    - More broadly, assistive systems often monitor task completion, errors, and adherence to suggested routines to adapt prompts and interfaces without requiring users to explicitly state changing goals or capacities.[^7_3][^7_4]

These designs are particularly relevant for populations with communication or executive barriers, where implicit signals (task initiation, completion, reliance on prompts) serve as proxies for goals and priorities.

## Behavioral signal processing for intent and preference

- **From raw behavior to latent intent**
    - Work in behavioral signal processing for digital media use models sequences of interactions and contexts to infer latent behavioral intents (e.g., immersive use, information seeking) using architectures like dual‑channel cross‑attention networks.[^7_18]
    - This framework builds motivational embeddings from textual messages and contextual signals, then predicts high‑risk or goal‑related behaviors, showing that combining psychological and ecological features improves behavior prediction over baselines.[^7_18]
- **Multimodal user‑state inference**
    - Multimodal HCI frameworks combine interaction logs with other channels (e.g., gaze, posture, environment) to infer user states that are not explicitly reported, supporting adaptive tutoring, workload management, or assistance.[^7_3]

While some BSP work focuses on affect, these examples show how similar techniques can infer information‑seeking goals, risk‑taking, or engagement patterns, all without explicit user articulation.

## Populations with communication or executive barriers

- **Executive dysfunction and assistive systems**
    - Evidence from ATC studies indicates that technologies like smart homes and mobile reminders can reduce prospective memory failures and support functional therapy by aligning prompts with inferred daily routines and goals, with single‑case designs used to demonstrate causal effects.[^7_20][^7_21][^7_4]
- **Design recommendations from reviews**
    - The scoping review on ATC for executive function recommends greater use of observational and ideation methods to understand user goals, more explicit support for goal formulation operations, and broader coverage of daily activities, highlighting gaps where further implicit goal inference work is needed.[^7_4]

Across these domains, the dominant pattern is to model user goals and preferences as **latent variables** inferred from sequences of interactions, context, and sometimes personality or psychological signals, then to update and exploit these latent representations for recommendation, adaptation, or assistance—especially valuable when explicit articulation of goals is difficult or impossible.[^7_2][^7_19][^7_1][^7_4][^7_3]

What would be most useful for you next: a method‑by‑method table (e.g., collaborative filtering, exposure‑aware models, multimodal AT, psycho‑ecological BSP) with signals, inference technique, and typical applications, or a deeper dive into how these approaches are being adapted specifically for users with communication and executive function impairments?
<span style="display:none">[^7_22][^7_23][^7_24][^7_25][^7_26][^7_27][^7_28][^7_29][^7_30][^7_31][^7_32][^7_33]</span>

<div align="center">⁂</div>

[^7_1]: https://eldorado.tu-dortmund.de/server/api/core/bitstreams/7f57b3cb-a7c0-4956-a63d-beb447862eaf/content

[^7_2]: https://discovery.ucl.ac.uk/id/eprint/10088708/1/Jawaheer Modelling RS ACM Transactions TiiS 2014(4)bh.pdf

[^7_3]: https://ict.usc.edu/pubs/A generic framework for the inference of user states in human computer interaction.pdf

[^7_4]: https://journals.sagepub.com/doi/10.1177/20556683241268658

[^7_5]: https://web-ainf.aau.at/pub/jannach/files/BookChapter_Social_Information_Access_2018.pdf

[^7_6]: https://ieeexplore.ieee.org/document/10959059/

[^7_7]: https://arxiv.org/pdf/1510.07025.pdf

[^7_8]: https://www.sciencedirect.com/science/article/pii/S095741742100213X

[^7_9]: https://dl.acm.org/doi/10.1145/3711896.3736927

[^7_10]: https://arxiv.org/pdf/2107.12325.pdf

[^7_11]: https://arxiv.org/pdf/2107.01529.pdf

[^7_12]: https://arxiv.org/pdf/2206.00147.pdf

[^7_13]: https://dl.acm.org/doi/10.1145/3564284

[^7_14]: https://arxiv.org/abs/2112.11023v1

[^7_15]: https://fajieyuan.github.io/papers/mingyue_sigir2021.pdf

[^7_16]: https://arxiv.org/pdf/2302.06559.pdf

[^7_17]: https://dl.acm.org/doi/10.1145/3581641.3584032

[^7_18]: https://journals.plos.org/plosone/article?id=10.1371%2Fjournal.pone.0338507

[^7_19]: https://arxiv.org/abs/2601.16872

[^7_20]: https://www.researchprotocols.org/2023/1/e48503/

[^7_21]: https://pmc.ncbi.nlm.nih.gov/articles/PMC10498320/

[^7_22]: https://arxiv.org/abs/2302.04473

[^7_23]: https://ieeexplore.ieee.org/document/11126013/

[^7_24]: https://arxiv.org/abs/2409.05033

[^7_25]: https://arxiv.org/abs/2502.15711

[^7_26]: https://arxiv.org/abs/2511.07295

[^7_27]: https://journals.sagepub.com/doi/full/10.3233/IDA-226576

[^7_28]: https://dl.acm.org/doi/pdf/10.1145/3580305.3599473

[^7_29]: http://arxiv.org/pdf/2409.05461.pdf

[^7_30]: https://arxiv.org/html/2510.27157v1

[^7_31]: https://www.cs.ubc.ca/~conati/my-papers/iui03-camera.pdf

[^7_32]: https://ceur-ws.org/Vol-2697/paper4_impactrs.pdf

[^7_33]: https://pubmed.ncbi.nlm.nih.gov/37642985/

