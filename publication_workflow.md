# Federal LCA Commons Publication Workflow


## Section for Federal LCA Commons submission handbook


## Ezra Kahn, February 4, 2020


# Publication Cases

Publishers are organizations with an ongoing LCA program.  Publishers maintain internal expertise in the LCA Commons publication workflow and technology.  The publication cases represent the types of scenarios organizations may encounter when publishing data.


## Case 1: Regular updates to an existing collection (USLCI case)

In this case, a repository represents a regularly updated collection.  A Product Owner will receive submissions from a range of actors with varying levels of data preparation competency.  The Product Owner acts as an agent to the Commons for any data producers / researchers who submit and publish data through the repository.  The Product Owner will execute several workflows from the original submission to final publication including, but not limited to:



*   receiving a data submission
*   transferring submission from original format into openLCA data model
*   performing a range QA on the submission
*   communicating with submitter on design intent, presentation, representativeness, documentation, etc
*   integrating submission into data product for release
*   aligning data product to conventions and standards defined in the FLCAC Data Submission Guidelines
*   etc.


## Case 2: Irregular updates / additions to an existing collection (Forest Products Lab case)

In this case, a repository represents a collection of context specific individual datasets that are published and/or updated incrementally.  Datasets may be updated to reflect temporal changes, technical changes, data model / descriptors, etc.  Updates may be applied to individual datasets on a case by case basis, and may not represent a new version of the collection as a whole.  New datasets may be added to the collection, and the new additions may also require changes to existing datasets.  This repository will be managed by a Product Owner who will be working directly with or for the organization producing the datasets, and acts as an agent to the Commons for a single organization.


### Case 2.1: Creating a new collection in a new repository


### _See Case 3: Stand-alone data collection_


### Case 2.2: Performing minor updates to published datasets on an existing repository

Minor updates are changes made to a data set or element that do not modify the representation of the concept modeled and its intended use.  Some reasons for performing minor updates could be to improve discoverability, revise a metadata descriptor, or bring documentation into closer conformance with a standard.  Minor updates could include for example: changes to flow or process metadata, repairing broken links or references, fixing units, or adjusting errors in calculations.  These changes typically do not require archiving the unrevised dataset.


### Case 2.3: Performing major updates or adding new datasets to a collection on an existing repository 

Major updates change the representativeness of a dataset or its intended use.  Major updates may be made to reflect changes in technology, temporal boundaries, changes in goal and/or scope.  A dataset undergoing a major revision is in some respects a new dataset and requires a new UUID.  The preceding dataset and/or collection may be archived to facilitate reproduction and reuse.


## Case 3: Stand-alone data collection (NETL coal data case)

In this case, the repository represents a single, context specific collection that is published as a unit.  Updates will be infrequent, and will typically be applied to the entire collection and published as a new version.  This repository will be managed by a Product Owner who will be working directly with or for the organization producing the datasets, and acts as an agent to the Commons for a single organization


## Case 4: Publishing specific “state” of a working repository

In some special cases, the LCA Commons may choose to support an organization with working repositories for version control and intra-organizational collaboration.  The development of a dataset or collection would be committed to a repository on the LCA Commons and many of the versions on the Commons would represent a work-in-progress.  Ready-to-be-published data would exist on a specific commit, future commits representing additional work to the same or different datasets.  An organization may want to make only specific “states” or versions of the working repository public.


## Case 5: Rolling back to a previously published version

Circumstances may require “rolling back” a public repository to a previously published version.  For all of the above cases, the commit history should include all of the previous public versions of the repository.  Rolling back to a previous version is essentially creating a clone of the current repository at a previous state, and making that clone public.


##  


# Workflows

The following workflows describe the steps necessary for a Product Owner to publish data on the LCA Commons.


## Case 1: Regular updates to an existing data product (USLCI case)


### Actors



*   Product Owner


### Conditions



*   The Product Owner is assumed to have “owner” privileges within a Group on LCA Commons.  These are elevated privileges, assigned on a case-by-case basis by the LCA Commons Manager.  
*   A public facing repository exists for which a regular update will be performed


### Steps:



*   Create a working copy of current public version
*   Add / make updates to create a new version
*   Publish the updated repository
1. Create a working copy of current public version
    1. Log in to the [LCA Commons](www.lcacommons.gov/lca-collaboration/login)
    2. Navigate to the public repository to be updated
    3. Create a new working repository, named appropriately, for example:”USLCI_2020_Q1_Update”
    4. ~~Clone the repository into the current Group, rename the copy appropriately, for example:”USLCI_2020_Q1_Update”~~
    5. ~~De-select “This repository can be accessed publicly” (This will be selected if the current repository is publicly accessible).~~
2. Add / make updates to create a new version
    6. Create a new “empty database” in openLCA
    7. Connect to the current public repository
    8. Checkout the latest commit to the database
    9. Disconnect from the public repository, and commit to the new working repository
    10. Import the new dataset into the database while connected to the repository
    11. Commit changes to the new repository at appropriate intervals (with descriptive commit messages)
3. Publish the updated repository

_Note: Collaboration server can have only one repository for each name.  We must remove the current repository from the server before publishing the new one_.



    12. Navigate to the current public repository
    13. De-select “This repository can be accessed publicly”
    14. Export the current repository and save it for a backup
    15. Delete the current repository
    16. Navigate to the updated repository
    17. Clone the repository into the same group, enter the appropriate repository name, for example: “USLCI”
    18. Select “This repository can be accessed publicly”
    19. Delete the copied “working” repository (optional)


## Case 2: Irregular updates / additions to an existing data product (Forest Products Lab case)


## Case 2.1: Creating a new collection in a new repository

_See Case 3: Stand-alone data collection_


## Case 2.2: Updating published datasets on an existing repository


### Actors



*   Product Owner
*   LCA Commons Manager


### Conditions



*   A public data collection exists on a LCA Commons repository
*   Product Owner has “contributor” privileges on LCA Commons on the existing repository
*   A set of known updates are to be committed to a new version of a repository


### Steps



1. Request a copy of the current repository from LCA Commons Manager
2. Checkout latest public version into openLCA
3. Make updates to the dataset
4. Publish the dataset
1. Request a copy of the current repository from LCA Commons Manager
    1. Send an email to [ARS-NAL-LCACommonsEditor@USDA.GOV](mailto:ARS-NAL-LCACommonsEditor@USDA.GOV) and request a private repository copy
    2. Specify the Group and Repository name to be updated
    3. LCA Commons Manager should name the copied repository appropriately, for example: [CURRENT REPOSITORY]_flow_update
    4. LCA Commons Manager de-selects “This repository can be accessed publicly”.
    5. LCA Commons Manager adds Product Owner as a member with “contributor” privileges.
2. Checkout latest public version into openLCA. The Product Owner will:
    6. Create a new empty database in openLCA
    7. Connect to the copied repository on LCA Commons
    8. Checkout the latest commit to the database
3. Make updates to the dataset. The Product Owner will:
    9. Perform the planned modifications to the datasets in openLCA
    10. Make regular commits after each change (with descriptive commit messages)
    11. Notify LCA Commons Manager after last change is completed
4. Publish the dataset, the LCA Commons Manager will:
    12. Navigate to the current public repository
    13. De-select “This repository can be accessed publicly”
    14. Export the current repository and save it for a backup
    15. Delete the current repository
    16. Navigate to the updated repository
    17. Clone the repository into the same group, enter the appropriate repository name, for example: “USLCI”
    18. Select “This repository can be accessed publicly”
    19. Delete the copied “working” repository


### Case 2.3: Performing major updates or adding new datasets to a collection on an existing repository 


### Actors



*   Product Owner
*   LCA Commons Manager


### Conditions



*   A public data collection exists on a LCA Commons repository
*   Product Owner has “contributor” privileges on LCA Commons on the existing repository
*   A set of known major updates or new datasets are to be committed to a new version of a repository


### Steps



1. Request a copy of the current repository from LCA Commons Manager
2. Checkout latest public version into openLCA
3. Make major updates / additions to the dataset
4. Publish the dataset
1. Request a copy of the current repository from LCA Commons Manager
    1. Send an email to [ARS-NAL-LCACommonsEditor@USDA.GOV](mailto:ARS-NAL-LCACommonsEditor@USDA.GOV) and request a private repository copy
    2. Specify the Group and Repository name to be updated
    3. LCA Commons Manager should name the copied repository appropriately, for example: [CURRENT REPOSITORY]_flow_update
    4. LCA Commons Manager de-select “This repository can be accessed publicly”.
    5. LCA Commons Manager adds Product Owner as a member with “contributor” privileges.
2. Checkout latest public version into openLCA. The Product Owner will:
    6. Create a new empty database in openLCA
    7. Connect to the copied repository on LCA Commons
    8. Checkout the latest commit to the database
3. Make major updates / additions to the dataset.  The Product Owner will:
    9. Import or create the revised / new dataset
    10. For revised / new processes, select the appropriate referenced flows in the exchange table, assign providers as necessary
    11. For revised / new flows, replace existing flows globally within the collection using the bulk replace tool
    12. Commit the additions to the repository (with a descriptive commit message)
    13. Delete obsolete or irrelevant data elements
    14. Commit deletions to the repository (with a descriptive commit message)
4. Publish the dataset, the LCA Commons Manager will:
    15. Navigate to the current public repository
    16. De-select “This repository can be accessed publicly”
    17. Export the current repository and save it for a backup
    18. Delete the current repository
    19. Navigate to the updated repository
    20. Clone the repository into the same group, enter the appropriate repository name, for example: “USLCI”
    21. Select “This repository can be accessed publicly”
    22. Delete the copied “working” repository


## Case 3: Stand-alone data collection (NETL coal data case)


### Actors



*   Product Owner
*   LCA Commons Manager


### Conditions



*   The data collection is in openLCA, and conforms with the LCA Commons metadata guidance
*   Product Owner has “contributor” privileges.  
    *   Product Owner’s organization already has a Group established on LCA Commons
    *   New repository will need to be requested from the LCA Commons Manager.
    *   Final publication will be at discretion of LCA Commons Manager
*   This collection is a new publication, a version has not been previously published on LCA Commons


### Steps



1. Request a new repository from LCA Commons Manager
2. Upload the collection to the repository
3. Review / edit the data
4. Publish the collection
1. Request a new repository from LCA Commons Manager
    1. Send an email to [ARS-NAL-LCACommonsEditor@USDA.GOV](mailto:ARS-NAL-LCACommonsEditor@USDA.GOV) and request a new repository
    2. Specify the Group, Repository name, and describe the context of the collection.
2. Upload the collection to the repository.  The Product Owner will:
    3. Connect to the repository from openLCA
    4. Commit the collection to the repository (with a descriptive commit message)
    5. Review the collection on LCA Commons
    6. Make any necessary corrections in openLCA, making a commit to the repository after each major change
3. Publish the collection. 
    7. The Product Owner sends an email to [ARS-NAL-LCACommonsEditor@USDA.GOV](mailto:ARS-NAL-LCACommonsEditor@USDA.GOV) and request the repository be made public
    8. LCA Commons manager selects “This repository can be accessed publicly”
    9. The Product Owner will review the public repository on [www.lcacommons.gov/lca-collaboration](www.lcacommons.gov/lca-collaboration)


## Case 4: Publishing specific “state” of a working repository


### Actors



*   Product Owner
*   Product collaborators
*   LCA Commons manager


### Conditions



*   Product Owner and collaborators have “contributor” privileges
*   Collection has been developed in openLCA, with regular commits to an existing LCA Commons repository
*   Product Owner’s organization has a Group on the LCA Commons
*   A commit represents a publishable state, ready for public access


### Steps



1. Request a repository cloned from the publishable state
2. LCA Commons manager creates the publishable repository
3. Publish the repository
1. Request a repository cloned from the publishable state. The Product Owner will:
    1. Send an email to [ARS-NAL-LCACommonsEditor@USDA.GOV](mailto:ARS-NAL-LCACommonsEditor@USDA.GOV) and request a new repository
    2. Specify the Group, Repository name, public Repository name, and describe the context of the collection
    3. Specify the commit id and description associated with the publishable state
2. LCA Commons manager creates the publishable repository
    4. Clone the working repository to the organization’s Group
    5. Select the publishable commit from the Clone dialog
    6. Add the Product Owner to as a member with “reviewer” privileges to the new repository
    7. Product Owner reviews the new repository and verifies its integrity, then notifies LCA Commons manager either:
        1. Repository is ready to publish
        2. Changes need to be made to working repository, and new publishable commit will be specified
3. Publish the collection
    8. The Product Owner sends an email to [ARS-NAL-LCACommonsEditor@USDA.GOV](mailto:ARS-NAL-LCACommonsEditor@USDA.GOV) and request the repository be made public
    9. LCA Commons manager selects “This repository can be accessed publicly”
    10. The Product Owner reviews the public repository on [www.lcacommons.gov/lca-collaboration](http://www.lcacommons.gov/lca-collaboration)


## Case 5: Rolling back to a previously published version


### Actors



*   Product Owner
*   LCA Commons Manager


### Conditions



*   A public repository exists on LCA Commons
*   The public repository includes a commit history with a commit of the required previous state


### Steps



1. Request a repository to be rolled back
2. Create a clone of a previous commit
3. Publish the cloned repository
1. Request a repository to be rolled back. The Product Owner will:
    1. Send an email to [ARS-NAL-LCACommonsEditor@USDA.GOV](mailto:ARS-NAL-LCACommonsEditor@USDA.GOV) and request a repository roll-back
    2. Specify the Group, Repository name, 
    3. Specify the commit id and description associated with the required publishable state
2. LCA Commons manager creates the rolled-back repository
    4. Clone the current repository to the organization’s Group
    5. Select the requested commit from the Clone dialog
    6. Add the Product Owner to as a member with “reviewer” privileges to the new repository
    7. Product Owner reviews the new repository and verifies its integrity, then notifies LCA Commons manager if ready to publish
3. Publish the collection
    8. The Product Owner sends an email to [ARS-NAL-LCACommonsEditor@USDA.GOV](mailto:ARS-NAL-LCACommonsEditor@USDA.GOV) and request the repository be made public
    9. LCA Commons manager selects “This repository can be accessed publicly”
    10. The Product Owner reviews the public repository on [www.lcacommons.gov/lca-collaboration](http://www.lcacommons.gov/lca-collaboration)

<!-- Docs to Markdown version 1.0β18 -->
