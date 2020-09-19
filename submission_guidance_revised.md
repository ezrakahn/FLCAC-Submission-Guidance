![](./media/image1.jpg)


Thank you for your interest in providing access to your life cycle inventory (LCI) data through the LCA Commons. To facilitate accurate interpretation and reuse, data sets submitted to the LCI repository must adhere to specific data documentation, formatting, and nomenclature requirements.
# What is the Federal LCA Commons?
The Federal LCA Commons is an interagency community-of-practice focused on building synergies around sustainability research and policy within the United States government. The mission of the LCA Commons is to advance LCA data, research, and information systems; improve modelling methods and consistency; and increase public access to Federal LCA data and resources.  This handbook and the www.lcacommons.gov web repository are key tools for improving consistency and insuring access to federal LCA products.
# Who can publish on the LCA Commons?
Members of the federal government and their official agents, employed in the development and distribution of Federal Data Products, may publish their work through the Federal LCA Commons.

Representatives of industry groups and academia interested in publishing with the LCA Commons should consider submitting data with the USLCI, operated by the National Renewable Energy Lab. Additionally, LCA data products produced through USDA funding can be published on the LCA Commons through the National Agricultural Library.

Publishing data on the LCA Commons comes with the expectation that data submitters have sufficient capacity to prepare data to be compliant with this guidance, and to study and successfully operate the publication workflow.  
# What can be published on the LCA Commons?
The Federal LCA Commons is an access point for Federal Data Products: products of federally funded and internally executed LCA research. They have been subject to internal, agency review and clearance processes, which confer additional value through quality assurance.

Datasets should represent novel contributions to the LIfe Cycle Assessment field.  Gate-to-gate unit processes and collections of processes associated as product systems are preferred to vertically aggregated cradle-to-gate inventories, to facilitate transparency and promote reuse.   Multifunctional unit processes should include all co-products, and may also include allocation factors or displaced products (according to the discretion of the submitter). 

Data from industry and other research efforts may be appropriate for the USLCI or other specialty repositories accessable through the LCA Commons web portal.  Please contact the LCA Commons staff to determine if the LCA Commons is right for you.

# How to publish on www.lcacommons.gov
The www.lcacommons.gov web repository is directly integrated into openLCA modeling software (both the repository and openLCA are developed and maintained by GreenDelta GMH [LINK]).  The openLCA desktop LCA tool is used for the preparation and submission of datasets to the LCA Commons.

Download the latest version of openLCA here [LINK]

Tutorials for using openLCA and importing data from other software and formats can be found here [LINK]

## Key terminology
(Do we need this?)
## Overview of the preparation and publication process
If you are interested in publishing your LCA data on www.lcacommons.gov, please contact Ezra Kahn at the National Agricultural Library to get started.  (ezra.kahn@usda.gov)

The publication workflow has two main components -- openLCA desktop software for data preparation, and the LCA Collaboration server (the repository at www.lcacommons.gov) for data publication.  Those that are interested in publishing their datasets on the LCA Commons must either develop their models using openLCA, or export their datasets from their preferred modeling software and import them into openLCA.  Instructions for doing this can be found on the openLCA documentation [LINK].  Once datasets are in openLCA, submitters should review them for consistency in representation and the results they produce, and then complete their documentation by filling out the metadata fields as described in this guidance.  Once datasets are ready for publication, they can be "committed" to the LCA Commons through the openLCA repository management feature, and the LCA Commons staff at the National Agricultural Library will make them public.

The LCA Commons organizes datasets into repositories, and groups of repositories.  A **repository** is typically a collection of datasets that are related.  The relation could be context or application focused, such as unit processes belonging to a larger gate-to-gate system.  The datasets in a repository could also be related through an administrative focus, such as unit processes developed as part of a particular grant or research project.  **Groups** on the LCA Commons are collections of repositories owned or maintained by a single organization.  Typically, a group will have one or several people who maintain all of the repositories of an organization.  Examples of different groups currently on the LCA Commons are the National Renewable Energy Laboratory and US EPA, two organizations that manage various context specific repositories.

The National Agricultural Library will create groups and repositories for new and returning users upon request.

 
## Roles and Actors
Data publication on the LCA Commons involves serveral recurring activities classified as *roles*.  Here, roles describe a set of responsilbilities or requisite skill sets.  A single person can have multiple roles.  It is suggested that a role is limited to a single person, though multiple people may perform the same role for the same submission if necessary.
	
### Data submitter roles
- Data owner: The data owner is a person or organization that funded, oversaw, or controls the project or program responsible for the creation of the submitted dataset.

- Data generator: The data generator is a person who was directly involved in the development of the datasets. This person has knowledge of the representativness of the models, the underlying assumptions, and the goal and scope of the study they were produced for.  This person would also serve as a point of contact for technical questions regarding appropriate interpretation and reuse of the data.

- Data documenter: the data documenter is the person who prepared the datasets for publication.  This person is expected to be familiar with the datasets being submitted, with the LCA Commons metadata convetions, with the openLCA information structure, and the Collaboration Server workflow.  The data documenter will serve as the point of contact for LCA Commons staff regarding data publication issues.

### LCA Commons roles
- Metadata librarian: the metadata librarian at the LCA Commons can assist data submitters with interpreting and preparing their LCA datasets for submission.

- Repository manager: the repository manager controls access to the LCA Commons Collaboration Server, including making new repositories, creating user accounts and managing permissions, and making datasets public.	

## Introduction to Preparation of Data for Publication
The following section presents an introduction to the metadata descriptors and conventions LCA Commons uses to implement ISO 14048 guidance using available conventions where possible.  Datasets are prepared using the openLCA desktop LCA modeling software.  

## Metadata descriptors and publication conventions
This section gives an overview on conventions for preparing and documenting data for publication on the LCA Commons.  Fields for metadata and LCA descriptors are accessible through the openLCA interface.  Detailed specifications for metadata and instructions for entering them into openLCA can be found in the Appendicies.
### Naming Conventions
#### Naming Conventions: Unit Processes
In the naming of processes and flows, the LCA Commons treats processes as activities performing one or more functions, and flows as materials, energy, or services that can be exchanged.  Process names shall describe the activity and any qualities specific to it.  Flow names shall describe the flow and any qualities specific to it, and *shall be considered independent from any activity and process*, thus process qualities or references will not be included in the flow name or documentation.  
##### Origianl Unit Process Nomenclature
Name all *original* ***Unit Processes*** that you submit to the LCA Commons according to the ILCD naming convention (see Metadata Guidelines[Link] below for element definitions).  The name should reflect the **process or activity** as follows: *base name; treatment, routes, standards; production type, location type; quantitative flow properties*

For example:
<div align="center"><em>
Clinker; average mineral mix, at kiln, 1415 kg/m3
</em></div>

##### External Database Unit Process Nomenclature
DO NOT submit unit processes which belong to commercial databases. For guidance on dealing with flows from external database unit processes, see the External Database Product/Intermediate Flow Nomenclature section [LINK].

##### Modified External Database Unit Process Nomenclature
If you have modified or customized a unit process from a commercial database, submit the process named like the original process with an indication that it is a modified version of the original. Document the source of the original process and detail the changes in the process documentation. Be sure to review your database license or contact your data vendor if there are any questions about publishing modified commercial datasets. 

For example, a modified ecoinvent process should look like this:
<div align="center"><em>
carbon dioxide liquid, at plant/RER U with US electricity
</em></div>

#### Naming Conventions: Flows
The LCA Commons supports three classes of flows: technosphere, elementary, and waste, consistent with the openLCA data model.
##### Technosphere Flows
Technosphere flows (also commonly known as product flows, or intermediate flows) represent goods, services, or energy exchange between processes.  Technosphere flows *remain in the system boundary* and have *economic or social value*.

Name all original product and intermediate flows according to the ILCD naming convention (see Process Metadata for instructions [LINK]).  The name should reflect the product or service (i.e., not the activity which produced it) as follows: *base name; treatment, routes, standards; production type, location type; quantitative flow properties.*

All four components of the above naming convention are required as applicable to a flow.  In cases where a naming component is not applicable, simply exclude it from the flow name.

For example:
<div align="center"><em>
corn grain; average tillage practice mix; at farm; 15% moisture
</em></div>
<br />

*External Database Technosphere Flows*<br />
When technosphere flows belong (or link to) an external software package or database, use exactly the same name, location, and units that are used in the external datasbase, and categorize them according to their provenance (see "Categories"[LINK] section for more detail).

##### Elementary Flows
Elementary flows (also commonly known as environmental flows) originate or terminate "in nature", outside the economic system boundary.  They are typically included in an inventory and contribute to the LCIA analysis.

The LCA Commons employs the Federal Elementary Flow List (FEDEFL) for elementary flow nomenclature and organization.  The FEDEFL is intended as a comprehensive, canonical list of flows compatible with all open LCIA methods.  Details on how to access and use the flow list can be found in Appendix [XXX] [LINK].  Additional details on the list and available workflows for translating to other nomenclatures can be accessed on the FEDEFL [<span class="underline">github repository wiki page](https://github.com/USEPA/Federal-LCA-Commons-Elementary-Flow-List/wiki) or the [<span class="underline">FEDEFL guidance document](https://cfpub.epa.gov/si/si_public_record_report.cfm?Lab=NRMRL&dirEntryId=341199).

##### Waste Flows
Waste flows are substances that must be handled by additional activities or processes.  They are within the system boundary but they do not have economic value.

The LCA Commons does not currently have guidance on documenting waste flows.

#### Product Systems
OpenLCA names product systems based on the name of reference process within the product system. Creating the product system from the reference unit process in openLCA will confer the name of that process. 

### Categorization
Unit process and technosphere flows are categorized using the North American Industry Classification System (NAICS).  More general categories correspond to a 2 digit code, and sub-categories have a 4 digit code.  Documentation and a full list of codes can be found at: [<span class="underline">https://www.census.gov/eos/www/naics/</span>](https://www.census.gov/eos/www/naics/).

### Parameters
Quantities of exchanges can be defined by parametric equations in unit process datasets submitted to the LCA Commons.  The LCA Commons does not maintain specifications for the preparation and publication of parameters.  Parameters, parametric equations, their relationships with exchanges, and appropriate and intended use should be well documented and made available through an appropriate repository, and referenced from the unit process documentation.  Please contact LCA Commons staff with any questions regarding parameters.
### Locations
Use the highest level of resolution when identifing locations, and document locations using standardized nomenclature.  For example, if documenting the US state of Colorado, use ISO 3166-2 to identify the Colorado as US-CO, and refernce ISO 3166-2 in the geography description field.
### DOIs
#### Basics
A DOI, or Digital Object Identifier, is a persistent and unique identifier assigned to an object. This DOI permanently identifies content and related metadata for an object over the course of its lifecycle. DOI strings, in combination with a URL prefix, resolve to internet locations. Information about a digital object may change over time, including where to find it and who owns it, but its DOI will not change. The benefits of a DOI include greater discoverability and access to uniquely identified content, accessibility for long-term use, and citation of publications and research data for impact analysis.
DOIs require a commitment from the provider to maintain the URL associated with the DOI.
#### DOIs on the LCA Commons
Currently, the LCA Commons does not mint or issue DOIs.  To obtain a DOI, a researcher must submit a request for a DOI with an issuing repository, which will often be the authoritative landing page for the dataset.  For example, USDA funded research can obtain a DOI by submitting a request to the Ag Data Commons (data.nal.usda.gov) which will create a record (with extensive metadata) and persistent URL for the datatset.  The Ag Data Commons will then mint a DOI that will resolve to this record.  

Datasets with existing DOIs can be directlly linked to the LCA Commons through the creation of a "source" object in openLCA.  An openLCA source is a reference to an external resource, and can be directly associated with an openLCA process in the Modeling and Validation section of the process's metadata. 

#### How to create a source DOI and associate it with an openLCA process
To associate an existing DOI to an openLCA process, the first step is to create a new DOI source from the navigation tree.  Give the source a suitable name using the convention:

Name: "Data citation: [The Dataset Title]"

In the URL field, enter the complete DOI, for example:
URL:https://doi.org/10.15482/USDA.ADC/1504010

Enter the preferred citation in the "Text reference" field and the year of publication, and save the source.  Users will now be able to access the dataset URL directly from the openLCA source page.

With the DOI source created, it can be associated to an openLCA process by adding it to the sources table in the Modeling and Validation section of the metadata.


# Collaboration Server How-to
# Getting started with the Starter Database
# Metadata Tables and Guidance
# Publication Workflow descriptions
# References
https://www.iso.org/obp/ui/#iso:std:iso:26324:ed-1:v1:en
