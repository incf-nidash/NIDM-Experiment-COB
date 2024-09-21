# NIDM-Experiment-Based on BFO/COB

**Overview**

The possibility of data reuse is predicated upon the availability of sufficient metadata that enables the end user to understand the methods and acquisition parameters used in the acquisition and processing of that data. These metadata may come in the form of file header information, but often information not captured by the acquisition hard- or software is necessary for reuse to occur. This means that data must be annotated or tagged with additional terms that provide the missing information.

A crucial part of data annotation is the use of unambiguous terms, and this generally requires both that the terms are defined and that terms be chosen in a manner that follows standard practice in a particular domain. To create logically consistent term collections and to model the relationships between the terms, ontologies have been created. Ontologies can be general, such as the Information Artifact Ontology (IAO), domain specific such as the Alzheimer's Disease Ontology (ADO), or foundational such as the Basic Formal Ontology (BFO).

Reusing terms from established and actively-maintained ontologies, rather than creating new terms for each project, is considered good ontological practice. Term reuse, however, is not necessarily an easy task as term tenses, term variations, and how the term fits into a domain-specific ontology may determine whether it can be reused. Domain-specific terms are usually not included in existing general or foundational ontologies, but rather are gathered to create a separate ontology. One potential issue for domain-specific ontologies is the lack of a formal basis (ontological view) which can lead to inconsistencies between terms and therefore can restrict the ease or ability of expansion of the domain-specific ontology. 

**NEC and NIDM-Experiment**

NEC (NIDM-Experiment based on COB) is an effort to construct a sound ontological basis for the NIDM-Experiment ontology, by using the Basic Formal Ontology as the foundational term set. We also have leveraged and the Core Ontology for Biology and Biomedicine (COB) which has been created as a “starter set” ontology – a smaller subset of terms from BFO that adheres to the BFO organization and adds some terms commonly used in biology and biomedicine. By basing a new ontology on BFO/COB, we can leverage a wide array of ontologies such as the Ontology of Biomedical Investigations (OBI), which contains many terms useful in describing neuroscientific experiments. This means that all the data in an experiment which collects MRI, PET, CT, blood samples, and neuropsychological instrument data can be modeled by NEC to an arbitrary level of detail and within the same framework, which facilitates all the data to be Findable, Reusable, and Interoperable – part of the FAIR Principles. 

NEC is an ontology that can be used to describe neuroscience-related experiments. While NIDM-E was initially constructed to describe MRI-based neuroimaging studies, it has since been expanded to include both general terms needed to describe experiments using other non-MRI data acquisition modalities.

The conversion of NIDM-E from an earlier version as a PROV-based controlled terminology to a BFO-based ontology is ongoing. It is built from collections of terms from existing BFO-related ontologies and augmented only when a needed term either does not exist in an active or recent ontology or the existing terms have a different meaning or usage from that relevant for NIDM-E. NIDM-E also contains collections of terms that are used in the Brain Imaging Data Structure (BIDS) and terms that represent the full set of DICOM tags.

All terms in NIDM-E contain either definition or, in the case of the BIDS terms, descriptions (which are not formal definitions). Terms imported into NIDM-E keep the definition from the parent ontology. Terms created specifically for NIDM-E, all have definitions in the form of "X is a Y which Zs", where X is the term, Y is the genus and Z are the differentia (Seppala, Ruttenburg, Smith. Ci.Inf., Brasília, DF, v.46 n.1, p.73-88, jan./abr. 2017).
The terms in NIDM-E are broken into several categories: classes, datatype properties, object properties, annotation properties, and named individuals. Terms considered to be classes are general terms that often describe what an experimental variable is "about", e.g., "age". Datatype properties connect numerical values to Entities, while object properties connect Entities and annotation properties are used to attach a note to an Entity that describes something about the Entity.

NEC should also be considered "under construction". As noted above, the initial terms in NIDM-E were related to MRI-based neuroimaging, but NIDM-E (and now NEC) has been constructed such that "hooks" exist that can be used to add terms needed to annotate terms from other modalities. 

NIDM-E was built by selecting terms needed to annotate real datasets and has expanded as new datasets are considered. As such, NEC is a "practical", rather than "theoretical" terminology and so terms may be missing that may be useful, but were not needed for the datasets upon which NIDM-E was built to describe. Suggestions for new terms, edits to term parentage, and term definitions are welcome. These can be suggested using the Issues function in GitHub. Click on "Issues" -> "New issue" and a list of issue-type templates will become available. These can be used to make suggestions and track the discussion and resolution of each issue. We are also actively working to provide feedback to other ontologies on the terms we have imported in NEC.

A set of GitHub pages are available for NEC. First a set of [term resolution pages](https://incf-nidash.github.io/NIDM-Experiment-COB/) provides a URL for each term that can be used in semantic web applications. Each term source has its own page. Second, is a [Schema Browser](https://incf-nidash.github.io/NIDM-Experiment-COB/schema_menu.html) that displays an expandable view on the tree for each type of terms (Classes and Properties). There is a search function within the Schema Browser, which searches within each term-type page.

