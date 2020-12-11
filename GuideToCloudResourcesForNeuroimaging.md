# Hitchhiker\'s Guide to Using Cloud-Based Resources for Neuroimaging Research

**Authors:** Deanna Barch, Maryann Martone, Jonathan Cohen, Nita
Farahany, Gregory Farber, Magali Haas, Sean Horgan, David Kennedy, Tara
Madhyastha, and Russell Poldrack

©2019. This work is licensed under a [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license. 


## Background

**[Mission]{.ul}**: On September 24, 2019, the National Academies of
Sciences, Engineering, and Medicine's Forum on Neuroscience and Nervous
System Disorders hosted a workshop titled "[[Neuroscience Data in the
Cloud]{.ul}](https://www.nationalacademies.org/event/09-24-2019/neuroscience-data-in-the-cloud-a-workshop),"
that explored the burgeoning use of cloud technology to advance
neuroscience research and approaches to addressing current barriers.
Following the one-day meeting, it was decided that there would be value
in generating an informational guide for investigators and
administrators in the field at different levels of experience for
understanding, accessing and successfully using cloud based tools in
support of neuroscience research, using neuroimaging as an example.
Neuroimaging was chosen as this example field as it already has numerous
Cloud-based infrastructure and tools, but the guidance is meant to be
useful for neuroscientific data of all kinds. The [[action
collaborative]{.ul}](https://www.nationalacademies.org/our-work/action-collaborative-on-neuroscience-data-in-the-cloud)[^1]
was charged with producing such guidance to help users and
administrators at different levels of expertise access and navigate
cloud-based resources for neuroscience research.

**[Process]{.ul}**: We convened a collaborative working group of
individuals from the workshop who indicated their interest in
participating in such an ongoing effort, attempting to ensure a wide
range of representation. The group met monthly starting in February
2020. We began by generating a use case scenario of an early-stage
investigator with limited expertise. We then generated an evaluation
matrix, comprising different types of concerns and issues that such an
investigator would address if they wanted to conduct research that used
cloud-based resources. For each of these considerations, we provide a
description, a range of values or levels for that consideration (e.g.,
the researchers skill level in cloud based computing, level of privacy
or security needed) and definitions of those levels. We then proceeded
to generate best-case practices for each of those considerations, as
well as resources for gathering more information or training, things to
avoid, articles, and tools. Finally, we consider the use case against
this evaluation matrix to provide an illustration of how these different
considerations affect decisions about using the Cloud.

The guide should help researchers and administrators understand:

1.  When to use Cloud resources

2.  How to use the Cloud effectively

## User Scenario

**[Persona]{.ul}**: Jordan is a first-year assistant professor at a
midsize R1 (research intensive) university. She received her Ph.D. in
cognitive neuroscience in a lab that did primarily small-N task-based
fMRI studies, and used relatively traditional approaches to data
analysis (lab-based server or laptop) and did not regularly engage in
data sharing. However, Jordan did a postdoctoral fellowship in the lab
of a mentor who was regularly engaged in larger scale studies that
sometimes utilized cloud-based computing and engaged in broad data
sharing. Jordan learned to do some analyses in the cloud while a
postdoctoral fellow, but was not responsible for setting up any of the
infrastructure and was not responsible for setting up data sharing on
any projects.

**[Environment]{.ul}**: Jordan's institute has a high performance
computing center for use by investigators with expertise in using
containerized (i.e., pre-packaged) computing tools, and a data science
center with cloud office hours. Further, there is at least one
investigator in another department that regularly uses cloud-based
computing resources. However, no one in Jordan's department does so.
Jordan's institution has been involved in a number of large-scale
clinical studies that involved data sharing of clinical data, but has
not done so with neuroimaging data in previous studies.

**[Use case]{.ul}**: Jordan would like to conduct a neuroimaging study
in which she would recruit approximately 200 individuals from the
community to examine the relationship between individual differences in
facets of emotion regulation, and associated individual differences in
structural and functional connectivity. She is also considering whether
she will need a larger N and whether she needs to join or launch a
multi-institution study or perhaps whether there are existing data that
she can use. Jordan will assess a range of behavioral measures
(individual differences in psychopathology, personality and behavior)
outside of the scanner, as well as T1- and T2-weighted MRI, resting
state fMRI and diffusion MRI. Her team is also considering obtaining DNA
samples for whole-genome analysis and the possibility of doing mobile
sensing with participants, collecting information about activity, sleep,
geolocation, and potentially even scraping information about app usage,
frequency of texts and calls, etc.

Jordan would like to establish robust and replicable analysis approaches
for all of her data types, and she would like to compare and contrast
several different analysis streams. Jordan may also need to develop
novel analysis tools to accomplish some of her aims. She wonders whether
she should be using the cloud and if so, how should she go about it? She
is planning to share the data through the NIMH Data Archive (NDA) or
another repository, but she wants the data to be reusable by other
platforms. It is also possible that she will want to follow these
individuals longitudinally and conduct follow-up imaging or behavioral
studies and make these data available as well.

*Why would Jordan use the Cloud?*

In general, researchers benefit from using the Cloud when data sets and
compute needs become large and are shared. "Large" in this case is a
moving target but generally refers to data size and complexity when
moving, downloading, storing and working with the data becomes
prohibitive over the course of the project. Cloud resources allow
storage and compute to scale with size and complexity. Sharing data and
compute resources also becomes easier as all parties are working off a
common platform. Although Cloud resources can be expensive, with the
commercial platforms, costs can be easily shared among parties depending
on how they are set up. Nevertheless, the Cloud isn't necessarily right
for all applications and researchers and can lead to high monetary and
technological costs if an investigator is not careful.

We developed an evaluation matrix that summarizes major dimensions that
can impact whether using the Cloud is right for Jordan. When considering
whether to utilize cloud-based resources for her project, Jordan should
consider where her project falls on each of the dimensions described
below to determine whether the size and goals of the project warrants
the use of cloud-based resources and whether her lab or institution has
the resources necessary to help her navigate the complexities of cloud
based resources.

Note that in our evaluation matrix, we are generally considering the use
of Cloud resources that provide both storage and compute resources. We
are not considering popular cloud-based storage options such as Dropbox,
Box, Google Drive or iCloud, unless explicitly noted.

## Evaluation Matrix

+----------------------+----------------------+----------------------+
| **Dimension**        | **Description**      | **Value set**        |
+----------------------+----------------------+----------------------+
| Researcher skills    | What computational   | Low, Medium, High    |
|                      | skills and data      |                      |
|                      | handling skills does |                      |
|                      | the researcher have? |                      |
+----------------------+----------------------+----------------------+
| Number of            | The more             | Same institution,    |
| institutions         | institutions         |                      |
|                      | involved, the        | Multi-institution    |
|                      | greater the          |                      |
|                      | challenge for        |                      |
|                      | coordination and     |                      |
|                      | consistency of       |                      |
|                      | control over the     |                      |
|                      | data and tools.      |                      |
|                      | Additional           |                      |
|                      | institutions means   |                      |
|                      | additional           |                      |
|                      | complexities with    |                      |
|                      | data use agreements, |                      |
|                      | HIPAA compliance,    |                      |
|                      | IRB approvals and    |                      |
|                      | intellectual         |                      |
|                      | property, as well as |                      |
|                      | more technical       |                      |
|                      | factors, such as     |                      |
|                      | standards for data   |                      |
|                      | storage and          |                      |
|                      | calibration of       |                      |
|                      | tools.               |                      |
+----------------------+----------------------+----------------------+
| Access to            | Access to expertise  | Low, Mixed, High     |
| computational        | within a computer    |                      |
| resources and        | science department   |                      |
| expertise            | or data center and   |                      |
|                      | degree of services   |                      |
|                      | provided by a IT     |                      |
|                      | services and/or data |                      |
|                      | science center.      |                      |
+----------------------+----------------------+----------------------+
| Data size            | \# of subjects, \#   | Yes, No              |
|                      | of files per         |                      |
|                      | subject, and size of |                      |
|                      | files; \# of copies  |                      |
|                      | of files; to be      |                      |
|                      | downloaded or not    |                      |
+----------------------+----------------------+----------------------+
| Data                 | Number of modalities | Low, Medium, High    |
| complexity/scope     | and data types;      |                      |
|                      | dimensions of these  |                      |
|                      | data, e.g.,          |                      |
|                      | different licenses,  |                      |
|                      | identifiability, and |                      |
|                      | different sharing,   |                      |
|                      | IRB and HIPAA        |                      |
|                      | regulations          |                      |
+----------------------+----------------------+----------------------+
| Number of copies     | Will all data be     | 1, \>1               |
|                      | accessed through a   |                      |
|                      | single centralized   |                      |
|                      | storage (e.g.,       |                      |
|                      | Cloud) or are local  |                      |
|                      | copies required?     |                      |
|                      | Multiple copies can  |                      |
|                      | lead to issues with  |                      |
|                      | data integrity,      |                      |
|                      | versioning, and      |                      |
|                      | archival storage.    |                      |
+----------------------+----------------------+----------------------+
| Privacy              | Protections for      | Low, Medium, High    |
|                      | human subjects or    |                      |
|                      | other types of       |                      |
|                      | access control. Note |                      |
|                      | that this will       |                      |
|                      | interact with the    |                      |
|                      | data complexity      |                      |
|                      | issue because        |                      |
|                      | privacy concerns may |                      |
|                      | change as more and   |                      |
|                      | more data types      |                      |
|                      | accrue.              |                      |
+----------------------+----------------------+----------------------+
| Security             | Issues include       | Low, Medium, High    |
|                      | different regulatory |                      |
|                      | policies that would  |                      |
|                      | govern compliance    |                      |
|                      | and what the archive |                      |
|                      | already has in       |                      |
|                      | place; e.g., NIH     |                      |
|                      | Authority to Operate |                      |
+----------------------+----------------------+----------------------+
| Data generation      | Will all data be     | Yes, No              |
| sources              | generated by the     |                      |
|                      | institutions         |                      |
|                      | involved in the      |                      |
|                      | study or will some   |                      |
|                      | come from outside    |                      |
|                      | parties, e.g.,       |                      |
|                      | wearable devices?    |                      |
+----------------------+----------------------+----------------------+
| Length of study      | Longer studies may   | Short, Medium, Long  |
|                      | necessitate the use  |                      |
|                      | of multiple scanner  |                      |
|                      | protocols over time  |                      |
|                      | or analysis          |                      |
|                      | strategies may       |                      |
|                      | change. Issues       |                      |
|                      | include complexities |                      |
|                      | of managing a length |                      |
|                      | of study and length  |                      |
|                      | of time data         |                      |
|                      | required to be       |                      |
|                      | stored as well as    |                      |
|                      | data and software    |                      |
|                      | versioning.          |                      |
+----------------------+----------------------+----------------------+
| Costs                | How many direct      | Low, Medium, High    |
|                      | costs for compute,   |                      |
|                      | storage, network     |                      |
|                      | costs are borne by   |                      |
|                      | the researcher?      |                      |
|                      | Issues include both  |                      |
|                      | short-term (while    |                      |
|                      | doing the study and  |                      |
|                      | analysis) and        |                      |
|                      | long-term costs for  |                      |
|                      | storage; cost of     |                      |
|                      | curation and         |                      |
|                      | organizing data,     |                      |
|                      | both the data you    |                      |
|                      | are generating and   |                      |
|                      | the output; cost of  |                      |
|                      | complying and using  |                      |
|                      | standards; and cost  |                      |
|                      | of compute.          |                      |
+----------------------+----------------------+----------------------+
| Existing data        | If the researcher    | Yes, No              |
|                      | use other datasets   |                      |
|                      | in the study, then   |                      |
|                      | they must understand |                      |
|                      | the conditions for   |                      |
|                      | data reuse and       |                      |
|                      | sharing of           |                      |
|                      | derivative results   |                      |
|                      | (e.g., the           |                      |
|                      | Adolescent Brain     |                      |
|                      | Cognitive            |                      |
|                      | Development \[ABCD\] |                      |
|                      | study has high       |                      |
|                      | restrictions on      |                      |
|                      | re-release options). |                      |
+----------------------+----------------------+----------------------+
| Software/pipelines   | Does the researcher  | Low, Medium, High    |
|                      | have to develop      |                      |
|                      | their own            |                      |
|                      | cloud-compliant      |                      |
|                      | tools/analysis       |                      |
|                      | pipelines?           |                      |
+----------------------+----------------------+----------------------+
| Degree of data       | Will the data be     | Public, Controlled   |
| sharing              | shared with          | access, No sharing   |
|                      | others/made public?  |                      |
|                      | If so, will there be |                      |
|                      | any restrictions on  |                      |
|                      | access or usage of   |                      |
|                      | the shared data?     |                      |
+----------------------+----------------------+----------------------+
| Submission to third  | Will the data be     | Yes, No              |
| party repository     | deposited in a third |                      |
|                      | party repository?    |                      |
|                      | What are the         |                      |
|                      | requirements of the  |                      |
|                      | repository?          |                      |
+----------------------+----------------------+----------------------+
| IRB experience with  | Does the IRB have    | Yes, No              |
| neuroimaging and     | familiarity with     |                      |
| cloud data           | issues surrounding   |                      |
|                      | sharing data in a    |                      |
|                      | cloud computing      |                      |
|                      | environment?         |                      |
+----------------------+----------------------+----------------------+
| Informed consent     | The degree of        | Low, Medium, High    |
| data sharing         | sharing and use      |                      |
| coverage             | allowed by informed  |                      |
|                      | consent. Issues      |                      |
|                      | include the type of  |                      |
|                      | repository to which  |                      |
|                      | data can be shared,  |                      |
|                      | the nature of data   |                      |
|                      | use agreements       |                      |
|                      | requirements, and    |                      |
|                      | the degree or        |                      |
|                      | re-release allowed   |                      |
|                      | and whether the data |                      |
|                      | must be              |                      |
|                      | de-identified or     |                      |
|                      | anonymized.          |                      |
+----------------------+----------------------+----------------------+

## Use Case 

In the following section, we evaluate the user scenario against the
matrix in Table 1. We provide definitions for each of the value sets and
situate the user scenario within the matrix.

### Researcher Skills 

**[Description]{.ul}**: What computational skills and data handling
skills does the researcher have?

**[Value Set Definitions]{.ul}**:

-   **Low**: Researcher has basic familiarity with neuroimaging tools
    and workflows in a local environment, but little or no experience
    with Cloud Computing. Researchers who would label themselves as low
    on this dimension should consider carefully whether they have the
    time and resources needed to develop the necessary expertise in
    order to use cloud-based resources for their projects. Even though
    the research group may not have the necessary expertise now, the
    group will want to think about whether they need to develop this
    expertise for their future research efforts.

-   **Medium**: Researcher has good computational and data skills but
    only modest cloud computing experience.

-   **High**: Researcher has computational and data skills; has cloud
    computing experience.

**[Value of Use Case Example]{.ul}**: *Medium* - Jordan did a
postdoctoral fellowship in the lab of a mentor who was regularly engaged
in larger scale studies that sometimes utilized cloud-based computing
and engaged in broad data sharing. Jordan learned to do some analyses in
the cloud while a postdoctoral fellow, but was not responsible for
setting up any of the infrastructure and was not responsible for setting
up data sharing on any projects.

**[Discussion of Use Case Example]{.ul}**: The researcher is fortunate
that she has some experience with working in the Cloud, but probably not
enough to avoid common mistakes without additional training and access
to those with more expertise. Therefore, it is critical that Jordan
increase her level of training and familiarize herself with best
practices and what is available as whether or not she uses the Cloud
now, she may need to do so in the future.

**[Best Practices]{.ul}**:

-   Utilize available campus resources on cloud computing/data science.

-   Determine to what extent you, the researcher, will need to provide
    system administration for the cloud as opposed to having someone
    else take this on.

-   Look for existing tooling that meet the needs and skill level of the
    researcher (i.e., look at recent papers).

-   Participate in training courses for neuroscience data in the cloud.

-   Look within funding agencies for training or informational
    researcher resources on cloud computing.

**[Things to Avoid]{.ul}**:

-   "Hidden" costs and risks: educate yourself! Remember that things you
    may not be used to paying for (e.g., CPUs you own but do not use,
    may cost you in a cloud environment).

-   Reinventing the wheel: take advantage of what is already available.

-   Don\'t go it alone.

-   Don\'t be afraid to ask the cloud provider for help/support/money.

-   Focusing only on the short term: think about how your future needs,
    both for this study and future studies, and whether you need to
    invest in additional training now.

**[See Also]{.ul}**:

-   [[Costs]{.ul}](#costs)

-   [[Access to Computational Resources and
    Expertise]{.ul}](#access-to-computational-resources-and-expertise)

**[Resources and Tools]{.ul}**:

-   [[INCF training space:]{.ul}](https://training.incf.org/) Growing,
    centralized resource for training materials in neuroinformatics

    -   [[Current offerings relevant to the
        Cloud]{.ul}](https://training.incf.org/search?filter=cloud).

-   [[NeuroHack Academy]{.ul}](https://neurohackademy.org/): Summer
    school in neuroimaging and data science

    -   See [[NeuroHack Academy/OHBM: Cloud resources for
        neuroimaging]{.ul}](https://neurohackademy.org/course/cloud-computing-for-neuroimaging/)

-   [[CloudBank]{.ul}](https://www.cloudbank.org/): A cloud access
    entity that will help the NSF-supported computer science community
    access and use public clouds for research and education by
    delivering a set of managed services designed to simplify access to
    public clouds. Educational and training materials are available to
    all.

    -   [[Getting started using the
        Cloud]{.ul}](https://www.cloudbank.org/training/getting-started-using-cloud)

    -   [[Training materials]{.ul}](https://www.cloudbank.org/training)

-   [[STRIDES]{.ul}](https://datascience.nih.gov/strides): NIH program
    that includes educational materials, training opportunities and
    other resources

-   [[ReproNim]{.ul} [Training
    Materials]{.ul}](https://www.repronim.org/teach.html): ReproNim's (A
    Center for Reproducible Neuroimaging Computation) general training
    materials. Cloud examples in the [["How would ReproNim do]{.ul}
    [*That*?"]{.ul}](https://how-would.repronim.org/en/latest/search.html?q=Cloud)
    series of documents.

-   [[Neuroimaging Informatics Tools and Resources Collaboratory
    Computational Environment
    (NITRC-CE)]{.ul}](https://www.nitrc.org/plugins/mwiki/index.php/nitrc:User_Guide_-_NITRC_Computational_Environment_Main):
    NITRC-CE is an on-demand, virtual computing platform designed for
    neuroimaging researchers, incorporating many neuroimaging tools, and
    deployable on the Amazon Web Services (AWS) Elastic Cloud Computing
    (EC2) environment. The User Guide provides detailed instructions for
    using the NITRC-CE for cloud computing.

**[Relevant Articles:]{.ul}**

-   Science in the cloud (SIC): A use case in MRI connectomics

    -   [[https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5467033/]{.ul}](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5467033/)

-   Heads in the Cloud: A primer on neuroimaging applications of high
    performance computing

    -   [[https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4896536/]{.ul}](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4896536/)

-   Running neuroimaging applications on Amazon Services: How, when and
    at what cost

    -   [[https://www.frontiersin.org/articles/10.3389/fninf.2017.00063/full]{.ul}](https://www.frontiersin.org/articles/10.3389/fninf.2017.00063/full)

  --------------------------------------------
  **[User story]{.ul}**: Suggestions welcome
  --------------------------------------------

### Number of Institutions 

[**Description**:]{.ul} The more institutions involved, the greater the
challenge for coordinating and ensuring consistency of control over the
data and tools. Additional institutions means additional complexities
with data use agreements, HIPAA rules, IRB approvals and intellectual
property, as well as ensuring consistency of standards for data storage
and calibration of associated instruments used for evaluations and tools
used for data analyses.

**[Value Set Definitions]{.ul}**:

-   **Single Institution:** All key members of the research team are at
    the same institution

-   **Multiple Institutions:** Key members of the research team are at
    more than one institution

**[Value of Use Case Example]{.ul}**: *Single Institution* - Jordan
would like to conduct a study in which they would recruit between 200
individuals from the community to examine the relationship between
individual differences in facets of emotion regulation, and associated
individual differences in structural and functional neural connectivity.
She is also considering whether she will need a larger N, whether she
needs to join or launch a multi-institution study, or whether there may
be existing data that she can use.

**[Discussion of Use Case]{.ul}**: While in the past, Jordan may have
been able to justify the use of 200 subjects, given concerns about
reproducibility a power analysis may show that she needs to increase the
number of subjects in order to have confidence in any reported effects.
It is not inconceivable that the number may be \> 1000. Therefore, she
will have to consider whether she needs to either lead or participate in
a multi-institution study. Alternatively, she may be able to augment or
perform her study with existing publicly available data. When using the
Cloud, designing a multi-institutional study can add several levels of
complexity, as policies, practices, and cloud access may vary across
institutions. If institutions are international or comprise a mix of
types, e.g, academic, commercial, governmental, the situation may be
even more complex, as different countries have different privacy laws
regarding use of the Cloud. Different types of partners may also have
different requirements.

**[Best Practices]{.ul}**:

-   Single institution

    -   Ensure that all team members adhere to the institution\'s
        relevant policies and practices.

-   Multi-institution: Using lead institution as a starting and
    reference point and address the following

    -   Generate an inventory of all institutions\' relevant policies
        and practices.

    -   Consider whether different institutions within the project have
        different objectives, and whether and how those differences may
        impact the policies and practices for the project as a whole.

    -   Pick a reference set of policies and practices, and identify any
        deviations of the guidelines applicable to one or more
        participating institutions that are more or less stringent than
        the reference set, and then determine whether institutions that
        are more lenient in those policies or practices can comply with
        the most stringent ones.

    -   Negotiate failures to converge on the most stringent set,
        possibly using community-wide resources (such as this matrix!!)
        as additional reference points.

    -   Distribute final guidelines to all team members.

    -   The lead investigator at each institution should ensure
        adherence to guidelines at that institution.

    -   Address at the outset who owns which data and how this interacts
        with data sharing policies, both among the participating
        institutions and with outsiders (as outlined along other
        dimensions in this matrix).

    -   Ideally, all institutions should use the same cloud
        service/repository for the project, and one that is standard and
        appropriate for the type of data being collected (e.g.,
        dedicated to neuroimaging NITRC IR NIMH Data Archive \[NDA\]).
        If project- and/or institution-specific one(s) are
        preferable/necessary (e.g., for pilot / interim results and/or
        if there are special needs and/or restrictions, such as HIPAA
        restrictions, project-specific meta-data requirements, etc.,
        that are not met by existing standard services or repositories),
        then these should also be identified at the outset, and
        policies/practices established for how the affected information
        will eventually be migrated to the project-wide platform(s).

**[Things to Avoid]{.ul}**:

-   Do not assume that the lead institution is the **only one**
    responsible for determining and overseeing policies and practices
    related to the study.

-   Do not assume that all institutions have the same policies,
    practices, or even objectives.

-   Do not assume that each institution can operate independently.

-   Do not assume that the lead investigator at each institution is
    solely responsible for policies and practices regarding the part of
    the study at that institution alone and does not need to coordinate
    with the other involved institutions.

**[See Also]{.ul}**:

-   [[Software/Pipelines]{.ul}](#softwarepipelines)

-   [[Privacy]{.ul}](#privacy)

-   [[Security]{.ul}](#security)

-   [[IRB Experience with Neuroimaging and Cloud
    Data]{.ul}](#irb-experience-with-neuroimaging-and-cloud-datacomputing)

**[Resources and Tools]{.ul}**:

-   [ReproNim Statistics Module:](http://www.repronim.org/module-stats/)
    including power analysis to determine required study size

-   

**[Relevant Articles:]{.ul}**

-   Security and privacy requirements for a multi-institutional cancer
    research data grid: an interview-based study

    -   [[https://bmcmedinformdecismak.biomedcentral.com/articles/10.1186/1472-6947-9-31]{.ul}](https://bmcmedinformdecismak.biomedcentral.com/articles/10.1186/1472-6947-9-31)

-   Guidelines for Multi-Institutional/Collaborative Research

    -   [[https://journals.lww.com/academicmedicine/Fulltext/2015/03000/Guidelines_for_Multi_Institutional_Collaborative.33.aspx]{.ul}](https://bmcmedinformdecismak.biomedcentral.com/articles/10.1186/1472-6947-9-31)

-   Establishing a Multi-Institutional Quality and Patient Safety
    Consortium Collaboration Across Affiliates in a Community-Based
    Medical School

    -   [[https://journals.lww.com/academicmedicine/Abstract/9000/Establishing_a\_Multi_Institutional_Quality_and.97145.aspxEstablishing]{.ul}](https://bmcmedinformdecismak.biomedcentral.com/articles/10.1186/1472-6947-9-31)

  ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **[User story]{.ul}**: A real-time fMRI scanning project was carried out collaboratively between two major research universities, one with a medical center and the other without. This involved scanning at the institution with the medical center using protocols designed by the other, and with data delivered to a cloud based 'engine' for real-time analysis and feedback. In order to accomplish this, a variety of obstacles had to be hurdled. The respective institutional IRB's had to understand and approve the protocol. Network connections had to be developed in accordance with privacy protections (which were warranted by both institutions as well as the cloud vendor). Technical experts from both institutions had to arrive at a common understanding of what was to be accomplished, who owned what aspects of the data, and ultimately deliver a reproducible prototype that allowed the work to begin. This process took roughly a year, much of which was occupied by efforts to coordinate the independent policy reviews carried out by the various units at each institution.
  ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Access to Computational Resources and Expertise 

**[Description]{.ul}:** Access and degree of services provided by a
computer science department and/or data science center at the
investigator's institution.

**[Value Set Definitions]{.ul}**:

-   **Low**: Researcher has access to few institutional resources.
    Researchers who would label themselves as low on this dimension
    should consider carefully whether they have the time and resources
    needed to develop the necessary expertise in order to use
    cloud-based resources for their projects.

-   **Mixed**: Good neuroimaging expertise, but little institutional
    computer or data science support; or good computational expertise
    and resources but little neuroimaging expertise.

-   **High**: Good neuroimaging expertise and strong institutional
    computer and data science support using Cloud Computing.

**[Value of Use Case Example]{.ul}**: *Mixed* - Jordan's institute has a
high performance computing center for use by investigators with
expertise in using containerized (i.e., pre-packaged) computing tools,
and a data science center with "cloud office hours", i.e., a dedicated
help resource that can answer her questions about using the cloud.
Further, there is at least one investigator in another department that
regularly uses cloud based computing resources. However, no one in
Jordan's department does so. Jordan's institution has been involved in a
number of large scale clinical studies that involved data sharing of
clinical data, but has not done so with neuroimaging data in previous
studies.

**[Discussion of use case]{.ul}**: Based on the resources available to
Jordan, she should reach out to colleagues with specific expertise in
cloud-based neuroimaging or consider taking a training course that
provides training in cloud based use of neuroimaging tools.

**[Best Practices]{.ul}**:

-   Look to campus high-performance computing resources as a first
    start, if available.

-   If not, look to the Computer Science department for cloud-based
    computing courses.

-   Understand how others in the same field of research use cloud
    computing, and leverage their experience whenever possible.

-   Work with the cloud vendor to understand options, costs, and
    programs to support your work.

**[Things to Avoid]{.ul}**:

-   Do not assume you know what resources are available without
    checking. You need to do due diligence to check on resources.

-   Do not be limited by the computing power of your laptop. There are
    many resources that will get you computing for free or a low cost.

-   Do not invest in solutions that do not have a clear track record and
    evidence of some longevity.

**[See Also]{.ul}**:

-   [[Software/Pipelines]{.ul}](#softwarepipelines)

**[Resources and Tools]{.ul}**:

-   [[NeuroHack Academy]{.ul}](https://neurohackademy.org/): Summer
    school in neuroimaging and data science

    -   See [[NeuroHack Academy/OHBM: Cloud resources for
        neuroimaging]{.ul}](https://neurohackademy.org/course/cloud-computing-for-neuroimaging/)

-   [[CloudBank]{.ul}](https://www.cloudbank.org/): A cloud access
    entity that will help the NSF-supported computer science community
    access and use public clouds for research and education by
    delivering a set of managed services designed to simplify access to
    public clouds. Educational and training materials are available to
    all.

    -   [[Getting started using the
        Cloud]{.ul}](https://www.cloudbank.org/training/getting-started-using-cloud)

    -   [[Training materials]{.ul}](https://www.cloudbank.org/training)

-   [[STRIDES]{.ul}](https://datascience.nih.gov/strides): NIH program
    that includes educational materials, training opportunities and
    other resources

-   [[Neuroimaging Informatics Tools and Resources Collaboratory
    Computational Environment
    (NITRC-CE)]{.ul}](https://www.nitrc.org/plugins/mwiki/index.php/nitrc:User_Guide_-_NITRC_Computational_Environment_Main):
    NITRC-CE is an on-demand, virtual computing platform designed for
    neuroimaging researchers, incorporating many neuroimaging tools, and
    deployable on the Amazon Web Services (AWS) Elastic Cloud Computing
    (EC2) environment. The User Guide provides detailed instructions for
    using the NITRC-CE for cloud computing.

-   [[Jetstream Cloud Resources]{.ul}](https://jetstream-cloud.org/):
    NSF-supported project led by the Indiana University Pervasive
    Technology Institute (PTI) designed for those who have not
    previously used high performance computing and software resources.
    The system is particularly geared toward 21st-century workforce
    development at small colleges and universities -- especially
    historically black colleges and universities, minority serving
    institutions, tribal colleges, and higher education institutions in
    EPSCoR States.

-   [[Cloud Carpentry for
    Genomics]{.ul}](https://datacarpentry.org/cloud-genomics/):on-line
    course materials for a Data Carpentry course providing practical
    training in understanding and using the cloud for analysis

**[Relevant Articles:]{.ul}**

-   Suggestions welcome

  --------------------------------------------
  **[User story]{.ul}**: Suggestions welcome
  --------------------------------------------

### Data Size 

**[Description:]{.ul}** Number of participants, number of files per
participant, and size of files; number of copies of files, and whether
the data will be downloaded or not.

**[Value Set Definitions]{.ul}**: Yes or no, based on whether or not the
size of data are sufficient (\>= terabytes) to warrant pushing to cloud

**[Value of Use Case Example]{.ul}**: *Yes* - The size of the data for
the proposed study will be sufficiently large to warrant the use of the
cloud.

**[Discussion of Use Case]{.ul}**: A modest amount of data may not
warrant the use of cloud-based resources unless there are other
considerations that warrant the use of the cloud, such as a lack of
resources at the investigators home institution, the need to coordinate
data collection/processing across multiple sites, or the need to share
data in a way that cannot be supported by the home institution.

**[Best Practices]{.ul}**:

-   Do not maintain copies of data if not necessary (see number of
    copies, below).

-   Store data so that it can be queried/explored (see number of copies,
    below).

-   Organize data to make it easy to optimize cost of cloud storage by
    using different storage classes (set up rules so this can be done
    automatically).

-   Separate derived products from archival/raw data (using different
    folders, for example).

-   Use consistent naming conventions across projects (see BIDS format
    below).

-   Raw data should be saved with read-only permissions to avoid
    accidental changes or deletion.

-   Focusing on the short term: Consider how data sizes and
    ingress/egress may change over the course of the study. If you plan
    to remove your data from the cloud at the end of the project, it is
    a good idea to reserve money in the budget for that in advance.

**[Things to Avoid]{.ul}**:

-   Do not dump all files into a single tarball per participant.

-   Do not duplicate raw data across researchers working on the same
    project. Consider a shared raw data repository.

**[See Also]{.ul}**:

-   [[Data Complexity/Scope]{.ul}](#data-complexityscope)

-   [[Number of Copies]{.ul}](#number-of-copies)

**[Resources and Tools]{.ul}**:

-   [[BIDS]{.ul}](https://bids.neuroimaging.io/) format for data
    organization

-   AWS user guides for Cloud set up

    -   <https://aws.amazon.com/blogs/aws/s3-intelligent-tiering-adds-archive-access-tiers/>

    -   <https://docs.aws.amazon.com/AmazonS3/latest/user-guide/create-lifecycle.html>

**[Relevant Articles:]{.ul}**

-   The brain imaging data structure, a format for organizing and
    describing outputs of neuroimaging experiments

    -   [[https://www.nature.com/articles/sdata201644]{.ul}](https://www.nature.com/articles/sdata201644)

-   MEG-BIDS, the brain imaging data structure extended to
    magnetoencephalography

    -   [[https://www.nature.com/articles/sdata2018110]{.ul}](https://www.nature.com/articles/sdata2018110)

  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **[User Story]{.ul}**: Cloud providers typically charge fees for moving data out of the cloud, between regions, and between certain types of storage classes (for example, moving data out of archival storage may incur a fee). It is important to know the fee structure for these operations to avoid unexpected bills. If you plan to remove your data from the cloud at the end of the project, it is a good idea to reserve money in the budget for that in advance.
  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Data Complexity/Scope 

**[Description]{.ul}**: Number of modalities and data types; dimensions
of these data, e.g., different licenses, identifiability, and different
sharing, IRB and HIPAA controls.

**[Value Set Definitions]{.ul}**:

-   **Low**: A limited number of neuroimaging data types

-   **Medium**: Multiple structural and functional neuroimaging types
    coming from multiple sources-covered by different licenses

-   **High**: Multiple structural and functional neuroimaging types as
    well as other data types, such as behavioral data and/or sequence
    data

**[Value of Use Case Example]{.ul}**: *High* - Jordan will assess a
range of behavioral measures (individual differences in psychopathology,
personality and behavior) out of the scanner, as well as T1, T2, resting
state and diffusion imaging. They are also considering obtaining DNA
samples and the possibility of doing mobile sensing with participants,
collecting information about activity, sleep, geolocation, and
potentially even scraping information about app usage, frequency of
texts and calls, etc.

**[Discussion of Use Case]{.ul}**: The acquisition or use of only a
single data type, especially if not a large amount of data, may not
warrant the use of cloud-based resources unless there are other
considerations that warrant the use of the cloud, such as a lack of
resources at the investigators home institution, the need to coordinate
data collection/processing across multiple sites, or the need to share
data in a way that cannot be supported by the home institution. In
Jordan's case, the high complexity/scope of the data she proposes to
collect may make this project appropriate for the use of cloud-based
resources.

**[Best Practices]{.ul}**:

-   Organize data with sufficient metadata to be accessed/queried
    programmatically (a centralized data repository, or a data lake)[^2]
    and also to be readable/understandable by humans.

-   Generate metadata from pipelines.

-   Consider using a standardized data format, such as the BIDS data
    format.

-   Consider using file formats that can be organized and queried with
    SQL and easily parsed, such as CSV.

-   Use consistent naming conventions across projects and datatypes.
    Your life will be much easier if you adopt practices of wherever
    your data is going to end up or whatever the tools expect.

**[Things to Avoid]{.ul}**:

-   Thinking that you are going to \"organize the data later\" - it is
    best to be built into the pipelines from the start.

-   Do not keep metadata separately from data, assuming you will be able
    to integrate later.

**[See Also]{.ul}**:

-   [[Degree of Data Sharing]{.ul}](#degree-of-data-sharing)

-   [[Software/Pipelines]{.ul}](#degree-of-data-sharing)

**[Resources and Tools]{.ul}**:

-   [[BIDS]{.ul}](https://bids.neuroimaging.io/) format for data
    organization

**[Relevant Articles:]{.ul}**

-   The brain imaging data structure, a format for organizing and
    describing outputs of neuroimaging experiments

    -   [[https://www.nature.com/articles/sdata201644]{.ul}](https://www.nature.com/articles/sdata201644)

-   MEG-BIDS, the brain imaging data structure extended to
    magnetoencephalography

    -   [[https://www.nature.com/articles/sdata2018110]{.ul}](https://www.nature.com/articles/sdata2018110)

  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **[User Story]{.ul}**: A researcher was trying to conduct a metaanalysis of three datasets, each with multiple spreadsheet manifests that stored the metadata for different types of data (imaging and cognitive). It was very difficult to collect all the missing pieces (scanner parameters, correction of inconsistent identifiers) and have confidence that the final data set was correct.
  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Number of Copies

**[Description]{.ul}**: Will all data be accessed through a single cloud
instance or are local copies required? Issues include data integrity,
versioning, and archival storage.

**[Value Set Definitions]{.ul}**:

-   **1:** Single copy + backups, no downloading

-   **\>1 copy:** Data stored in cloud but must maintain single version
    of record for legal, ethical, or technical reasons

-   **\>1 copy+**: Copies can be made and distribution rights can be
    granted

**[Value of Use Case Example]{.ul}**: *\>1 copy+* - Jordan is planning
to share the data through NDA or another repository, but they want the
data to be reusable by other platforms.

**[Discussion of Use Case]{.ul}**: Jordan will benefit from planning
prospectively for the cost of sharing data data and providing multiple
copies both through the NDA and other repositories, and will need to
ensure sufficient resources.

**[Best Practices]{.ul}**:

-   Consider using a repository or cloud service that helps track data
    versions. For example, Amazon S3 and Dropbox track data versions.

-   Identify ways to explore data without downloading it (either open
    summaries, or platforms that support authentication and querying of
    data) Cloud providers will keep snapshots of version

-   Work with cloud vendors to see if they can host valuable data for
    free

-   Consider whether you really need backups given the durability of the
    cloud storage (i.e., many cloud providers have very robust redundant
    storage already, so data may be sufficiently protected through
    permissions and versioning)

-   Make sure any policies on copies will allow necessary computing
    (permanent vs transient copies).

**[Things to Avoid]{.ul}**:

-   Do not store unnecessary copies.

**[See Also]{.ul}**:

-   [[Data Size]{.ul}](#data-size)

-   [[Costs]{.ul}](#costs)

**[Resources and Tools]{.ul}**:

-   Cloud storage services often used by academics: Check whether your
    institution has an institutional account for these services. Note
    that these are storage only and do not include compute.

    -   [[Amazon Public AWS
        Datasets]{.ul}](https://aws.amazon.com/opendata/?wwps-cards.sort-by=item.additionalFields.sortDate&wwps-cards.sort-order=desc)

    -   [[Box]{.ul}](https://www.box.com/home)

    -   [[Dropbox]{.ul}](https://www.dropbox.com/business/landing-t61fl?_tk=paid_sem_goog_biz_b&_camp=142947702&_kw=dropbox%257Ce&_ad=389661549544%257C%257Cc&gclid=Cj0KCQjwtsv7BRCmARIsANu-CQdSvrt0_2CMjuPNmtRZh-1QJqo2dDxUPRuHVia7iksr1c4GnAcyeakaAkX1EALw_wcB)

    -   [[Google Drive]{.ul}](https://www.google.com/intl/en_in/drive/)

    -   [[iCloud]{.ul}](https://www.icloud.com/)

    -   Institutional Repositories: Many institutions offer cloud-based
        storage for their constituents

**[Relevant Articles]{.ul}**:

-   Suggestions welcome

  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **[User story]{.ul}**: An IT department took to heart the requirement that data should not be copied. This was implemented in software design and policies in a solution that assumed researchers would only access object storage. Unfortunately, object storage does not support POSIX file system operations that are used by most research software. Furthermore, it precluded copying data to local storage to process it using a compute cluster. It is critical to think about the entire research workflow and make sure that policies do not hinder natural data use.
  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

###  

### Privacy

**[Description]{.ul}:** Protections for human subjects or other types of
access control. Note that this will interact with the data complexity
issue because privacy concerns may change as more and more data accrue.

**[Value Set Definitions]{.ul}**:

-   **Low**: anonymized data with no PHI

-   **Medium**: de-identified data-no special access controls

-   **High**: Identifiable data with substantial PHI

**[Value of Use Case Example]{.ul}**: *High* - Jordan will assess a
range of behavioral measures (individual differences in psychopathology,
personality and behavior) out of the scanner, as well as T1, T2, resting
state and diffusion imaging. They are also considering obtaining DNA
samples and the possibility of doing mobile sensing with participants,
collecting information about activity, sleep, geolocation, and
potentially even scraping information about app usage, frequency of
texts and calls, etc.

**[Use Case Discussion]{.ul}:** Jordan will need to make sure that
whatever cloud-based computing or storage options she uses will provide
adequate privacy protection for the type of data she is proposing to
collect and use. She will also need to ensure prospectively that her
consent allows her to share all of the data she wishes to share in the
ways she wishes to share it using the platforms she wishes to use.

**[Best Practices]{.ul}**:

-   Go to the local IRB and align your consent with what is possible in
    your local environment and be sure that the practices with regards
    to policy align with informed consent policies from your
    institution.

-   Consult with the privacy officer on campus.

-   Consider \"right to be forgotten\" policies, e.g., the GDPR,
    [CCPA](https://oag.ca.gov/privacy/ccpa). **Right to be forgotten**
    refers to the **right** to have private information about a person
    be removed from Internet searches and other directories under some
    circumstances.

-   Have an explicit policy on how to deal with privacy issues.

-   Understand the level of privacy you must maintain (PHI). The more
    dimensions you collect, the higher the chance of reidentification.

-   Many believe that brain data can potentially be used to identify
    individuals and ought to be treated as such.

-   Ensure that your data collection procedures do not unintentionally
    embed PHI in the files. For example, make sure that no participant
    name or birthdate information is used for registering participants
    at the scanner, as this data can become embedded in dicom files.

-   Ideal if all operations are performed in the Cloud.

-   Be careful about downloading protected data onto your own systems,
    and if you do, ensure that they are secure and compliant with
    relevant privacy rules.

-   Stay abreast of the changing regulatory environment.

**[Things to Avoid]{.ul}**:

-   Failure to ensure that the consent made with the participants meets
    your data analysis/sharing needs

-   Assume that the policies you adhered to at the start of the project
    remain relevant throughout the project

-   Making copies and using them external to the system

**[See Also]{.ul}**:

-   [[Number of Copies]{.ul}](#number-of-copies)

-   [[Security]{.ul}](#security)

-   [[Length of Study]{.ul}](#length-of-study)

-   [[IRB Experience with Neuroimaging and Cloud
    Data]{.ul}](#irb-experience-with-neuroimaging-and-cloud-datacomputing)

-   [[Informed Consent/Data Sharing
    Coverage]{.ul}](#informed-consentdata-sharing-coverage)

**[Resources and Tools]{.ul}**:

-   [[Open Brain Consent]{.ul}: portable consent forms specifically for
    sharing human neuroimaging data, developed by
    the](https://open-brain-consent.readthedocs.io/en/stable/) Open
    Brain Consent Working Group. Preprint: https://psyarxiv.com/f6mnp/

-   [[Ethical
    Wearables]{.ul}](https://ethics.harvard.edu/ethical-wearables):
    White paper describing an ethical framework for wearable devices

-   [[Right to be
    forgotten](https://gdpr-info.eu/issues/right-to-be-forgotten/):]{.ul}The
    **right to be forgotten** is the **right** to have private
    information about a person be removed from Internet searches and
    other directories under some circumstances.)

-   [[Privacy Shield]{.ul}](https://www.privacyshield.gov/welcome):
    framework for regulating exchanges of personal data for commercial
    purposes between countries

-   [[ENIGMA Process for protecting
    privacy]{.ul}](https://enigma.com/privacy-policy)

**[Relevant Articles:]{.ul}**

-   Privacy Challenges to the Democratization of Brain Data, iScience

    -   [[https://www.sciencedirect.com/science/article/pii/S2589004220303199?via%3Dihub]{.ul}](https://www.sciencedirect.com/science/article/pii/S2589004220303199?via%3Dihub)

  --------------------------------------------
  **[User story]{.ul}**: Suggestions welcome
  --------------------------------------------

### Security

**[Description]{.ul}**: Issues include different regulatory policies
that would govern compliance and what the archive already have in place;
NIH Authority to Operate; FedRAMP and FISMA \[moderate, high\]
requirements/capabilities

**[Value Set Definitions]{.ul}**:

-   **Low**: ISO 27001

-   **Medium**: FISMA/FedRAMP moderate; NIST 800.53 rev4

-   **High**: FISMA/FedRAMP high or data residency & exfiltration
    controls (in/out)

**[Value of Use Case Example]{.ul}**: *Medium/High* - Platform will have
to comply with appropriate security standards which may change depending
on what types of data Jordan ends up collecting.

**[Discussion of Use Case]{.ul}**: Not all Cloud environments are HIPAA
compliant and even if they are, Jordan is still responsible for setting
it up and using it properly. Thus, it is critical that Jordan understand
the relevant security issues herself, or partner with the experts on her
campus to ensure that she has the appropriate security controls. It will
also be important for Jordan to regular review and update security
protocols as there may be changes in relevant requirements and policies
over time. Again, this can be accomplished in part by continued
engagement with experts on campus or elsewhere.

**[Best Practices]{.ul}**:

-   Should contact the University IT, Info Security or CIO, and
    determine what practices are in place for their university

-   Consult experts when filling out any requirements rather than doing
    it yourself

-   Document what services are in place for the study

-   Consider using an existing cloud platform that provides a secure
    environment for neuroimaging rather than setting up your own

-   Make sure that your local IT understands how to create a secure
    cloud environment by asking specific questions, e.g., do you have
    support for creating a FISMA moderate compliant environment in X
    cloud platform?

-   Consult any policies from the funding source around security

-   In the absence of clear security policies from either sources,
    return to the data owner for guidance as you should not move forward
    without clear policies.

-   Understand what level of security is required

-   Plan for regular compliance review as the project evolves

-   Since shared compute resources are built upon a specific OS, and
    OS\'s have security implications, it\'s important to keep your
    shared cloud compute resources with up-to-date OS security patches.

**[Things to Avoid]{.ul}**:

-   Do not have a graduate student be in charge of security.

-   Do not assume that you know the answer without consulting with the
    relevant agencies/resources: security policies and guidelines change
    all the time; need to confirm that you are right.

-   Avoid being shortsighted---establish a framework that is agile.

-   Do not assume that the cloud environment handles all your security
    concerns (e.g., a malicious web browser extension could send data in
    the browser anywhere).

-   Do not assume that additional security features are free or turned
    on by default.

-   Ensure that the settings you choose don\'t create avenues for data
    access that you didn\'t intend (e.g., external IPs that you didn\'t
    plan for).

**[See Also]{.ul}**:

-   [[Privacy]{.ul}](#privacy)

-   [[Data Generation Sources]{.ul}](#data-generation-sources)

**[Resources and Tools]{.ul}**:

-   Understanding Different Levels/Layers of Security

    -   [[Google Cloud
        FEDRAMP]{.ul}](https://cloud.google.com/blog/topics/customers/google-cloud-platform-is-now-fedramp-high-authorized)

    -   [[AWS FEDRAMP]{.ul}](https://aws.amazon.com/compliance/fedramp/)

    -   [[AZURE
        FEDRAMP]{.ul}](https://azure.microsoft.com/en-us/blog/all-us-azure-regions-now-approved-for-fedramp-high-impact-level/)

    -   [[ISO/IEC standard for information
        security]{.ul}](https://www.iso.org/isoiec-27001-information-security.html)

    -   [[Terra/FireCloud Security
        Posture]{.ul}](https://support.terra.bio/hc/en-us/articles/360030793091-Terra-FireCloud-Security-Posture)

-   Cloudbank: [[Introduction to Cloud
    Security]{.ul}](https://www.youtube.com/watch?v=oZSBlEK6grc&feature=youtu.be)

-   Security Trainings

    -   [[NIH Information Security And Information Management Training
        Courses](https://irtsectraining.nih.gov/publicUser.aspx)]{.ul}

**[Relevant Articles:]{.ul}**

-   Suggestions welcome

  -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **[User Stories]{.ul}:** A researcher accessed data from a European Biobank that requires data to remain in the EU. The researcher used a public cloud to create a virtual machine to access that data but didn\'t change the default configuration for their compute & storage resources, which in this cloud was for the US region (Iowa). The researchers therefore were in violation of the policy and had to spend much time proving that they were in compliance. There are penalties for being out of compliance. [[https://healthitsecurity.com/news/uw-medicine-hit-with-lawsuit-for-breach-impacting-974k-patients]{.ul}](https://healthitsecurity.com/news/uw-medicine-hit-with-lawsuit-for-breach-impacting-974k-patients)\
  \
  A researcher developed a visualization tool for analyzing some controlled-access data. When trying to share that tool with some colleagues, they used another tool to set up a tunnel to the VM inside their network that exposed an external IP to the public. On that VM there were private keys to controlled-access data that any malicious user could easily locate. The researcher also bundled up these tools into a docker image for other researchers to use and deploy within their networks. [[https://techbeacon.com/security/hackers-love-docker-container-catastrophe-3-2-1]{.ul}](https://techbeacon.com/security/hackers-love-docker-container-catastrophe-3-2-1)

  -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### 

### Data Generation Sources

**[Description]{.ul}**: Will all data be generated by the institutions
involved in the study or will some come from outside parties, e.g.,
wearables?

**[Value Set Definitions]{.ul}**:

-   **Yes**: At least some data will come from outside sources

-   **No**: All data will be generated by the institutions involved in
    the study

**[Value of Use Case Example]{.ul}**: *Yes -* Wearable device or other
type of data stored on some other cloud service (see also existing
data); from device to mobile phone app (via Bluetooth) to vendor cloud
(via WIFI or cellular network); some devices can communicate with the
vendor cloud directly via WiFi or even cellular network (like Apple
Watch).

**[Discussion of Use Case]{.ul}:** Jordan will need to ensure that any
cloud-based computing and/or storage resources that she chooses to use
will both be capable of handling these outside data sources, and will
provide the needed level of privacy and security for these data sources.

**[Best Practices]{.ul}**:

-   Where possible use searchable and indexable formats, such as:

    -   Json

    -   Csv

    -   xlsx/xls

    -   txt

    -   Determine whether and how harmonization across different devices
        and apps for a seemingly common data stream is possible and what
        work will be required to achieve it.

-   Determine data threshold to find signal in the data to be considered
    significant (e.g. power analysis, etc.)?

-   Keep the source data. It is important to maintain original data
    downloaded from device/vendor cloud without any pre-processing so
    any errors in the processing algorithms can be fixed in the future

**[Things to Avoid]{.ul}**:

-   Missing data/metadata (organize your data collection from the
    beginning to ensure inclusion)

-   Using non-standard data formats (e.g. PDF, Word)

**[See Also]{.ul}**:

-   [[Existing Data]{.ul}](#existing-data)

**[Resources and Tools]{.ul}**:

-   Raw Data Repositories

    -   [[NDA]{.ul}](https://nda.nih.gov/)

    -   [[OpenNeuro]{.ul}](https://openneuro.org/)

    -   [[DANDI]{.ul}](https://www.dandiarchive.org/)

    -   [[DABI]{.ul}](https://dabi.loni.usc.edu/)

    -   [[NEMAR]{.ul}](https://nemar.org/)

-   Clinical Trials and Mobile Technologies:
    [[https://feasibility-studies.ctti-clinicaltrials.org/resources]{.ul}](https://feasibility-studies.ctti-clinicaltrials.org/resources)

-   Platforms for remote assessment

    -   [[Radar-base]{.ul}](https://radar-base.org/index.php/home/about-us/)
        (Remote Assessment of Disease And Relapses): An open source
        platform to leverage data from wearables and mobile
        technologies. The main focus of RADAR-base is seamless
        integration of data streams from various wearables to collect
        sensor data in real time and store, manage and share the
        collected data with researchers for retrospective analysis

    -   [[Elektra
        Academy]{.ul}](https://www.elektralabs.com/solutions/education):
        Free curriculum, resources, and research for organizations
        considering the incorporation of remote health monitoring.

-   **[Relevant Articles:]{.ul}**

    -   Behavior, sensitivity, and power of activation likelihood
        estimation characterized by massive empirical simulation

        -   [[https://pubmed.ncbi.nlm.nih.gov/27179606/]{.ul}](https://pubmed.ncbi.nlm.nih.gov/27179606/)

  --------------------------------------------
  **[User story]{.ul}**: Suggestions welcome
  --------------------------------------------

### Length of Study

**[Description]{.ul}**: Longer studies may necessitate the use of
multiple scanner protocols over time or analysis strategies may change.
Issues include the complexities of managing a length of study and length
of time data required to be stored as well as versioning.

**[Value Set Definitions]{.ul}**:

-   **Short**: Data collected over relatively short time (e.g., 1-2
    years) and no need for active storage post study completion

-   **Medium**: Either data collected over longer time period (3-5
    years) and/or need for longer active storage post study completion
    (e.g., 3-5 years)

-   **Long**: Longitudinal study over many years (e.g., 5+ years) and/or
    long term active storage post study completion (e.g., 5+ years)

**[Value of Use Case Example]{.ul}**: *Long -* It is also possible that
they will want to follow these individuals longitudinally and conduct
follow-up imaging or behavioral studies and make these data available as
well.

**[Discussion of Use Case]{.ul}**: A potential challenge to the use of
cloud computing for long studies is that price and features of cloud
computing may change over time, leading to unexpected costs or technical
challenges. This is particularly the case if the researcher takes
advantage of features that are specific to a particular cloud provider;
this can lead to them being locked into that provider.

**[Best Practices]{.ul}**:

-   Develop a plan in advance for technical change over time (e.g. what
    do you do when BIDS 2.0 comes out?)

-   Pay off technical debt gradually over time (e.g. regularly check to
    ensure that any custom software is compatible with the latest
    version of the language and important libraries).

-   Understand the long-term support options for your operating system
    and analysis software.

-   Develop and actively maintain documentation for data and analysis
    procedures.

-   Develop a plan for archiving of unused data to less expensive
    storage platforms.

**[Things to Avoid]{.ul}**:

-   Waiting until incompatibilities or changes in platforms occur to
    develop a plan to deal with them

**[See Also]{.ul}**:

-   [[Data Size]{.ul}](#data-size)

-   [[Data Complexity/Scope]{.ul}](#data-complexityscope)

**[Resources and Tools]{.ul}**:

-   [[fMRIPrep: Versioning and Long-Term
    Support]{.ul}](https://reproducibility.stanford.edu/fmriprep-lts/)

**[Relevant Articles:]{.ul}**

-   Cold Storage Data Archives: More Than Just a Bunch of Tapes

    -   [[https://arxiv.org/pdf/1904.04736.pdf]{.ul}](https://arxiv.org/pdf/1904.04736.pdf)

  --------------------------------------------
  **[User story]{.ul}**: Suggestions welcome
  --------------------------------------------

### Costs

**[Description]{.ul}**: How many direct costs for compute, storage,
network costs are borne by the researcher? Issues include both
short-term (while doing the study and analysis) and long-term costs for
storage; cost of curation and organizing data, both the data you are
generating and the output; cost of complying and using standards; and
cost of computing.

**[Value Set Definitions]{.ul}**:

-   **Low**: Relative low costs (\$10,000 or less)

-   **Medium**: Greater than \$10,000, but less than \$25,000

-   **High**: \$25,000 or more

**[Value of Use Case Example]{.ul}**: *High -* The amount of data and
length of store and compute demands are likely to be considerable.

**[Discussion of Use Case]{.ul}**: Jordan will either need to ensure
prospectively that her budget includes sufficient resources for all
planned cloud computing and storage costs, or determine whether she will
have sufficient budget for the duration of the project and all needs
before embarking on the use of cloud computing and storage. If her
budget did not initially cover these costs, there may be additional
institutional or federal funds available to do so that she could pursue.
It will be particularly important for Jordan to plan for costs that will
be needed throughout the life of the project, including any longer term
archiving or sharing costs.

**[Best Practices]{.ul}**:

-   Use available tools to estimate storage and compute costs of the
    project.

-   Plan for ongoing costs.

-   Determine whether subsidies are available from the institution,
    granting agencies or other sources.

-   Remember that commercial cloud costs are "Pay as you go."

-   Estimate on the high side---include a cushion

**[Things to Avoid]{.ul}**:

-   Paying to store additional copies of data

-   Not taking advantage of archival/\"cold\" storage

-   Not accounting for network costs associated with copying data

-   Not accounting for access costs or not taking advantage of
    \"requester pays\" capabilities

-   Forgetting to turn off machine you are not using

-   Not accounting for the free-tier of compute resources

**[See Also]{.ul}**:

-   [[Number of
    Copies]{.ul}](https://help.objectiflune.com/EN/printshop-mail-user-guide/7.2/172.html)

-   [[Length of Study]{.ul}](#length-of-study)

**[Resources and Tools]{.ul}**:

-   [[How to control cloud
    costs]{.ul}](https://support.terra.bio/hc/en-us/articles/360029772212-Controlling-Cloud-costs-sample-use-cases)

-   [: Use cases and discussion by Terra[Cloudbank: Cost
    estimation]{.ul}](https://support.terra.bio/hc/en-us/articles/360029772212-Controlling-Cloud-costs-sample-use-cases)

-   Cost Calculators

    -   [[https://calculator.s3.amazonaws.com/index.html]{.ul}](https://calculator.s3.amazonaws.com/index.html)

    -   [[https://cloud.google.com/products/calculator]{.ul}](https://cloud.google.com/products/calculator)

    -   [[https://azure.microsoft.com/en-us/pricing/calculator/]{.ul}](https://azure.microsoft.com/en-us/pricing/calculator/)

    -   [[https://docs.aws.amazon.com/AmazonS3/latest/dev/RequesterPaysBuckets.html]{.ul}](https://docs.aws.amazon.com/AmazonS3/latest/dev/RequesterPaysBuckets.html)

-   [[Life Cycle Decisions for Biomedical
    Data]{.ul}](https://www.nap.edu/catalog/25639/life-cycle-decisions-for-biomedical-data-the-challenge-of-forecasting):
    National Academy of Sciences, Engineering, and Medicine Report (see
    in particular Chapter 4 and Appendix E)

**[Relevant Articles:]{.ul}**

-   Running Neuroimaging Applications on Amazon Web Services: How, When,
    and at What Cost?

    -   [https://docs.aws.amazon.com/AmazonS3/latest/dev/RequesterPaysBuckets.html]{.ul}

  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **[User Story]{.ul}**: "The committee heard from researchers about their ability to 'experiment' with data-intensive computations, at no additional cost to them, when data resources were hosted by their research institutions. However, when their data were moved to a commercial cloud, the same levels of experimentation resulted in unexpected and large computational bills at the end of the month. Once the cost consequences of their behaviors became transparent (requiring compute bills to be sufficiently granular)---and especially when they were responsible for some or all of those costs---the researchers learned to be more thoughtful and efficient. For example, they began to pilot their analyses before performing them on full data sets. Making people responsible for their costs, helping them understand that their actions generate costs for someone, and providing appropriate training might help reduce resource consumption with more efficient workflows. The information resource platform manager might develop a compelling narrative to alert researchers to storage and computational cost structures and the empowering benefits to researchers of forecasting their costs (Chodacki, 2019). The narrative could properly stress the researchers' larger responsibility to the research community.\"-*National Academy of Sciences, Engineering, and Medicine Report: Life Cycle Decisions for Biomedical Data: The Challenge of Forecasting Costs, Box 3.3, pg 53*
  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Existing Data

**[Description]{.ul}**: Will the researcher use other datasets in the
study (e.g., ABCD has high restrictions on re-release options, but HCP
has more open re-release options).

**[Value Set Definitions]{.ul}**:

-   **No**: No other datasets will be used

-   **Yes**: but the data has no re-release restrictions

-   **Yes**: and the data has re-release restrictions

**[Value of Use Case Example]{.ul}**: *Maybe -* Given that Jordan may
not be able to obtain enough subjects to test her hypothesis, she should
consider whether she can use an existing dataset.

**[Discussion of Use Case]{.ul}:** Jordan will need to determine whether
incorporation of other data sets will either necessitate the use of
Cloud resources (i.e., that is the only pathway for use), or whether
they put any limits on the use of Cloud resources (e.g., privacy or
security constraints).

**[Best Practices]{.ul}**:

-   Familiarize yourself with sharing, privacy, and security
    requirements of any existing data sources that you will use.

**[Things to Avoid]{.ul}**:

-   Data of questionable quality

-   Excessive variance in acquisition/analysis method across data

**[See Also]{.ul}**:

-   [[Data Size]{.ul}](#data-size)

-   [[Data Complexity/Scope]{.ul}](#data-complexityscope)

**[Resources and Tools]{.ul}**:

-   Raw Data Repositories

    -   [[NDA]{.ul}](https://nda.nih.gov/)

    -   [[OpenNeuro]{.ul}](https://openneuro.org/)

    -   [[DANDI]{.ul}](https://www.dandiarchive.org/)

    -   [[DABI]{.ul}](https://dabi.loni.usc.edu/)

    -   [[NEMAR]{.ul}](https://nemar.org/)

    -   [[Human Connectome Data]{.ul}](https://www.humanconnectome.org)

    -   [[1000 Functional
        Connectomes]{.ul}](https://www.nitrc.org/projects/fcon_1000)

-   Processed data archives:

    -   [[NeuroVault]{.ul}](https://neurovault.org/): NeuroVault is a
        public repository of unthresholded statistical maps,
        parcellations, and atlases of the brain. It complements the raw
        data stores listed above by providing a host for the raw derived
        (but unthresholded) statistical maps that accompany published
        (usually static) thresholded example images. This greatly
        facilitates metaanalysis from the complete brain space in
        contrast to foci of activation-based metaanalysis that the
        typically published (thresholded) tabular results support.

    -   [[ReproLake]{.ul}:](http://nidm.scicrunch.io:7200/) The
        ReproLake is the ReproNim publically accessible neuroimaging
        metadata store. It hosts metadata that facilitates search and
        discovery of information based upon experiment and acquisition
        details, analysis results, processing workflows, etc.

    -   [[Preprocessed Connectomes
        Project]{.ul}](http://preprocessed-connectomes-project.org/)[:
        The goal of the Preprocessed Connectomes Project is to
        systematically preprocess the data from the 1000 Functional
        Connectomes Project (FCP) and International Neuroimaging
        Data-sharing Initiative (INDI) and openly share the results.
        This effort greatly reduces the redundancy of the preprocessing
        that typically would have to be performed by each investigator
        accessing a particular
        dataset.](https://www.humanconnectome.org/)

**[Relevant Articles]{.ul}:**

-   Suggestions welcome

  --------------------------------------------
  **[User story]{.ul}**: Suggestions welcome
  --------------------------------------------

### Software/Pipelines

**[Description]{.ul}**: Does the researcher have to develop their own
cloud-compliant tools/analysis pipelines?

**[Value Set Definitions]{.ul}**:

-   **Low**: All necessary tools/analysis pipelines are already
    available and operating in the cloud computing environment.

-   **Medium**: Some, but not all, of the necessary tools/analysis
    pipelines are already available and operating in the cloud computing
    environment.

-   **High**: None of the necessary tools/analysis pipelines are already
    available and operating in the cloud computing environment and all
    must be developed by the researcher.

**[Value of Use Case Example]{.ul}**: *Medium -* Jordan can use some
existing tools; although, she may need to adapt some of her existing
tools and pipelines so they work in the cloud.

**[Discussion of Use Case]{.ul}:** Efficient use of cloud computing
resources requires a different set of skills and knowledge regarding the
implementation and orchestration of software execution on large
datasets.

**[Best Practices]{.ul}**:

-   Use existing, published and established validated pipelines for
    cloud computing.

-   Ensure software & pipelines are designed to be cost-efficient for
    cloud computing.

-   Develop and actively maintain documentation for all cloud
    procedures.

-   Use containerized software packages with specific versioning.

**[Things to Avoid]{.ul}**:

-   Using homegrown software written by a postdoc.

**[See Also]{.ul}**:

-   [[Access to Computational Resources and
    Expertise]{.ul}](#access-to-computational-resources-and-expertise)

**[Resources and Tools]{.ul}**:

-   [Using containers (Docker/Singularity) in
    science](https://neurohackweek.github.io/docker-for-scientists/)

    -   A set of tutorials from the 2016 Neurohackweek

-   [[Docker]{.ul}](https://www.docker.com/)

    -   This is a container system that can be used on one's local
        machine.

    -   It can also be used to develop containerized analysis that can
        be run on high-performance computing systems using Singularity.

    -   [[DockerHub]{.ul}](https://hub.docker.com/) is a resource that
        provides a collection of popular computational tools provided
        within ready to use Docker containerized environments.

-   [[Singularity]{.ul}](https://sylabs.io/docs/)

    -   This is the container system used by most high-performance
        computing systems

    -   [[SingularityHub]{.ul}](https://singularity-hub.org/) and
        [[ReproNim/containers]{.ul}](https://github.com/ReproNim/containers)
        are resources that provide a collection of popular computational
        tools provided within ready to use Singularity containerized
        environments.

-   [Pipelines](https://www.repronim.org/)

    -   [[Nipype]{.ul}](https://nipype.readthedocs.io/en/latest/): A
        workflow management tool for neuroimaging analysis.

    -   [[Neurodocker]{.ul}](https://github.com/ReproNim/neurodocker): A
        tool that generates custom Dockerfiles and Singularity recipes
        for neuroimaging and minimizes the size of existing containers.

    -   [[fMRIPrep]{.ul}](https://fmriprep.org/en/stable/): A BIDS-App
        that provides robust preprocessing for fMRI data. It has a
        long-term support (LTS) version that guarantees it to function
        with consistent results for at least 4 years. It can be run
        using Docker or Singularity containers providing easy cloud
        deployment. Outputs are stored according to the BIDS-Derivatives
        standard for ease of reuse.

**[Relevant Articles:]{.ul}**

-   Cloud computing applications for biomedical science

    -   [[https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006144]{.ul}](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006144)

-   Analysis of task-based functional MRI data preprocessed with
    fMRIPrep

    -   [<https://rdcu.be/ca108>]{.ul}

  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **[User Story]{.ul}**: A researcher transferred their data and existing code base from a local computer to a cloud system so that they could process a large number of datasets. The code is primarily composed of Python programs written by the students in the laboratory. The postdoc running the project arranged to create a number of virtual machine instances on the cloud computer, and then manually installed the software on each system. They then logged into each machine and manually started the analysis on a different subset of the data. Because the code was not built for parallel processing, and was executed directly on the system rather than using a workflow management system, most of the computational power of the virtual machines sat idle when the jobs were running, leading to much greater computing expenses than if they had been implemented using tools that support parallel execution of workflow components.
  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Degree of Data Sharing

**[Description]{.ul}**: Will the data be shared with others/made public?

**[Value Set Definitions]{.ul}**:

-   **Public**: open license

-   **Controlled access**: Shared with public but account or permission
    required

-   **No sharing**: accessible only to researcher

**[Value of Use Case Example]{.ul}**: *Controlled access* - Jordan plans
to submit to the NIMH Data Archive.

**[Discussion of Use Case]{.ul}**: Currently the use of cloud computing
resources neither facilitates or impedes the sharing of data with the
NIMH Data Archive. However, it will facilitate submission to the NIMH
Data Archive if Jordan ensures that any formats or processing streams
used are optimally compatible with what will be required by the NIMH
Data Archive. Jordan should consult with the NIMH Data Archive to
determine whether they are implementing any particular transfer pathways
that have any particular requirements.

**[Best Practices]{.ul}**:

-   Before you set up your data acquisition pipelines, determine if
    templates or protocols that match your goals already exist in the
    intended database (e.g., NDA) that you can use to facilitate data
    harmonization.

-   Ensure that you use a consent form broad enough to allow the
    intended data sharing and use for research questions other than
    those driving the initial data acquisition.

**[Things to Avoid]{.ul}**:

-   Avoid reinventing the wheel and having to engage in time-intensive
    post-hoc harmonization if it can be avoided.

-   Avoid methods that require you to remove PHI post hoc before data
    sharing.

-   Avoid using a consent form that limits data sharing and reuse for
    novel research questions.

**[See Also]{.ul}**:

-   [[Informed Consent/Data Sharing
    Coverage]{.ul}](#informed-consentdata-sharing-coverage)

-   [[Degree of Data Sharing]{.ul}](#degree-of-data-sharing)

-   [[Privacy]{.ul}](#privacy)

**[Resources and Tools]{.ul}**:

-   [[NIMH Data Archive (NDA)]{.ul}](https://nda.nih.gov/): Cloud-based
    repository that makes available human subjects data collected from
    hundreds of research projects across many scientific domains. NDA
    provides infrastructure for sharing research data, tools, methods,
    and analyses enabling collaborative science.

-   [[Human Connectome Project]{.ul}](https://www.humanconnectome.org/)

-   [[NiPype]{.ul}](https://nipype.readthedocs.io/en/latest/): a Python
    project that provides a uniform interface to existing neuroimaging
    software and facilitates interaction between these packages within a
    single workflow.

-   [[Open Neuro]{.ul}](https://openneuro.org/): Open data repository
    for sharing MRI, MEG, EEG, iEEG, and ECoG data

**[Relevant Articles:]{.ul}**

-   Suggestions welcome

  --------------------------------------------
  **[User story]{.ul}**: Suggestions welcome
  --------------------------------------------

###  Submission to Third-Party Repository

**[Description]{.ul}**: Will the data be deposited in a third-party
repository? What are the requirements of the repository?

[**Value Set Definitions**:]{.ul}

-   **Yes**

-   **No**

**[Value of Use Case Example]{.ul}:** *Yes* - Jordan has already decided
to use the NIMH Data Archive as her third-party repository.

**[Discussion of Use Case]{.ul}:** Jordan has chosen to use the NIMH
Data Archive because she wants to analyze her newly acquired data along
with data already in NDA. Sharing data in NDA will also bring her into
compliance with the data sharing expectations should this research be
funded by NIMH
([[NOT-MH-19-033]{.ul}](https://grants.nih.gov/grants/guide/notice-files/NOT-MH-19-033.html)).
Jordan has also noted that NIMH expects a certain set of clinical
measures to be collected for all of their funded studies
([[NOT-MH-20-067]{.ul}](https://grants.nih.gov/grants/guide/notice-files/NOT-MH-20-067.html)),
so she is planning on adding those measures when she collects data.

One additional factor in Jordan's decision to use NDA is the "study"
feature in that repository. NDA creates "collections" of data that are
related to a single research program. Generally, collections are
associated with a single grant award, either from NIMH, one of the other
NIH Institutes and Centers using the repository, or from non-federal
funding groups. The study feature will allow Jordan to create a data set
containing the exact data set used in a publication. The data in a study
can all come from her collection or can come from more than one NDA
collection. Studies allow others to run different data analysis
pipelines on the exact data Jordan has already published on.

All of the data in NDA is stored in a commercial cloud provider with
appropriate security. Data access is restricted qualified investigators
as determined by a Data Access Committee (DAC) convened by NIMH. The DAC
also checks whether users requesting access are planning on using the
data in a way that is consistent with the informed consent. In addition
to storing the data, NDA provides limited cloud computational credits.
That feature of the archive should be useful to a user like Jordan.

**[Best Practices]{.ul}**:

-   Choose a third-party data archive that is appropriate for the data
    being measured. Things to think about are data sharing expectations
    from the funder, whether similar data are already available in the
    archive, the funding stability of the archive, and whether the data
    will have appropriate security and access control.

-   Choose a third-party data archive that makes the data as widely
    available as possible. If Jordan's data were less sensitive, a
    repository like OpenNeuro would make the data more easily available.

[**Things to Avoid**:]{.ul}

-   Hosting data on your own website

**[See Also:]{.ul}**

-   [[Informed Consent/Data Sharing
    Coverage]{.ul}](#informed-consentdata-sharing-coverage)

-   [[Degree of Data Sharing]{.ul}](#degree-of-data-sharing)

**[Resources and Tools:]{.ul}**

-   [[NIMH Data Archive (NDA)]{.ul}](https://nda.nih.gov/): Cloud-based
    repository that makes available human subjects data collected from
    hundreds of research projects across many scientific domains. NDA
    provides infrastructure for sharing research data, tools, methods,
    and analyses enabling collaborative science.

-   [[Open Neuro]{.ul}](https://openneuro.org/): Open data repository
    for sharing MRI, MEG, EEG, iEEG, and ECoG data

**[Relevant Articles:]{.ul}**

-   Suggestions welcome

  --------------------------------------------
  **[User story]{.ul}**: Suggestions welcome
  --------------------------------------------

###  

### IRB Experience with Neuroimaging and Cloud Data/Computing

**[Description]{.ul}**: Does the IRB have familiarity with issues
surrounding sharing data in a cloud computing environment?

**[Value Set Definitions]{.ul}**:

-   **Yes**, the institution or the investigator does have IRB
    experience with neuroimaging and cloud data/computing.

-   **No**, the institution and the investigator do not have IRB
    experience with neuroimaging and cloud data/computing.

**[Value of Use Case Example]{.ul}**: *No* - Jordan's institution does
not have a history of IRB experience with neuroimaging and cloud
storage/computing.

**[Discussion of Use Case]{.ul}**: Jordan will need to ensure that their
institution's IRB consults with more experienced institutions or will
need to gather suggestions from other institutions with more experience
in order to ensure that the IRB can appropriately evaluate and advise on
issues surrounding analysis and sharing in a cloud computing
environment.

**[Best Practices]{.ul}**:

-   Engage the IRB in a discussion about data-sharing approvals at the
    start of the project

-   Identify a colleague at an institution with good experience with
    data-sharing in a cloud environment to determine if you can provide
    a consultant from their IRB to your IRB

-   Provide your IRB with sample copies of approved consent forms and
    procedures from other institutions and projects that have
    successfully engaged in data-sharing in a cloud environment

**[Things to Avoid]{.ul}**:

-   Avoid having your IRB create a policy or set of procedures not
    in-line with the broader community

**[See Also]{.ul}**:

-   [[Informed Consent/Data Sharing
    Coverage]{.ul}](#informed-consentdata-sharing-coverage)

-   [[Degree of Data Sharing]{.ul}](#degree-of-data-sharing)

**[Resources and Tools]{.ul}**:

-   [[Open Brain Consent]{.ul}: portable consent forms specifically for
    sharing human neuroimaging data, developed by
    the](https://open-brain-consent.readthedocs.io/en/stable/) Open
    Brain Consent Working Group (preprint:
    [[https://psyarxiv.com/f6mnp/]{.ul}](https://psyarxiv.com/f6mnp/))

**[Relevant Articles:]{.ul}**

-   Suggestions welcome

  --------------------------------------------
  **[User story]{.ul}**: Suggestions welcome
  --------------------------------------------

### Informed Consent/Data Sharing Coverage

**[Description]{.ul}**: The degree of sharing and use allowed by
informed consent. Issues include the type of repository to which data
can be shared, the nature of data use agreements requirements, and the
degree or re-release allowed and whether the data must be de-identified
or anonymized.

**[Value Set Definitions]{.ul}**:

-   **Low**: The informed consent does not allow any data sharing.

-   **Medium**: The informed consent allows data sharing under
    restricted conditions.

-   **High**: The informed consent allows broad and open data sharing.

**[Value of Use Case Example]{.ul}**: *NA* - Jordan is just starting her
project and can work prospectively to ensure that the consent allows the
degree of sharing that she wishes for, which should be "High."

**[Discussion of Use Case]{.ul}**: Whether or not the informed consent
allows data sharing likely does not have an impact on the use of
cloud-based resources for analysis and storage of the data if Jordan
does not wish to share the data. However, given that Jordan would like
to be able to share data, it is critical that they ensure that the
consent allows for broad data sharing.

**[Best Practices]{.ul}**:

-   If you are still engaged in data collection, consider modifying the
    consent form to allow data sharing without restrictions, though this
    will not apply to already consented individuals

-   Identify databases for sharing that can meet your necessary
    restrictions-If you will be sharing directly from your own cloud
    based platform, develop a data use agreement that outlines the
    restrictions

**[Things to Avoid]{.ul}**:

-   Avoid using a consent form with more restrictive sharing and re-use
    than needed for your project

**[See Also]{.ul}**:

-   [[IRB Experience with Neuroimaging and Cloud
    Data]{.ul}](#irb-experience-with-neuroimaging-and-cloud-datacomputing)

-   [[Degree of Data Sharing]{.ul}](#degree-of-data-sharing)

**[Resources and Tools]{.ul}**:

-   [[Open Brain Consent]{.ul}: portable consent forms specifically for
    sharing human neuroimaging data, developed by
    the](https://open-brain-consent.readthedocs.io/en/stable/) Open
    Brain Consent Working Group (preprint:
    [[https://psyarxiv.com/f6mnp/]{.ul}](https://psyarxiv.com/f6mnp/))

**[Relevant Articles:]{.ul}**

-   Ethical aspects of data sharing and research participant protections

    -   [[https://pubmed.ncbi.nlm.nih.gov/29481107/]{.ul}](https://pubmed.ncbi.nlm.nih.gov/29481107/)

-   The ethics of secondary data analysis: Considering the application
    of Belmont principles to the sharing of neuroimaging data

    -   [[https://pubmed.ncbi.nlm.nih.gov/23466937/]{.ul}](https://pubmed.ncbi.nlm.nih.gov/23466937/)

  --------------------------------------------
  **[User story]{.ul}**: Suggestions welcome
  --------------------------------------------

[^1]: The collaborative is an ad hoc activity convened under the
    auspices of the Forum on Neuroscience and Nervous System Disorders
    at the National Academies of Sciences, Engineering, and Medicine
    (the National Academies). The work it produces does not necessarily
    represent the views of any one organization, the Forum, or the
    National Academies, and is not subjected to the review procedures
    of, nor is it a report or product of, the National Academies.

[^2]: A data lake is a centralized repository that allows you to store
    all your structured and unstructured data at any scale. You can
    store your data as-is, without having to first structure the data,
    and run different types of analytics---from dashboards and
    visualizations to big data processing, real-time analytics, and
    machine learning to guide better
    decisions.-[[AWS]{.ul}](https://aws.amazon.com/big-data/datalakes-and-analytics/what-is-a-data-lake/)
