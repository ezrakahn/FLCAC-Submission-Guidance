# FLCAC-Submission-Guidance
This repository is for maintaining a draft of the data submission guidance for Federal LCA Commons



## History of document
This document was first created in Google Docs and pandoc was used to convert to to github-flavored
markdown.

Starting with the version 'FLCAC 2019 Data Submission Guidelines - marked up' last edited on Feb 5, 2020,
the document was exported as a .docx and renamed to FLCAC.docx and saved in this repository directory. Word-generated
 table of contents and lists of tables and figures were removed.
Then the following command was used to convert it to markdown with embedded image files:

> pandoc -f docx -t gfm  --extract-media=. -o FLCAC_Submission_Guidance.md FLCAC.docx

The result was the [FLCAC_Submission_Guidance](FLCAC_Submission_Guidance.md) Markdown file with embedded links to images found in the `media` directory. 

 ## Current development
 The content in the [FLCAC_Submission_Guidance](FLCAC_Submission_Guidance.md) reflects the best and accepted guidance for publishing data on lcacommons.  There is a need to reorganize and edit the content for the Federal LCA Commons context, and there is additional content necessary as noted in the issues section.
 
 The [submission_guidance_revision](submission_guidance_revision.md) document is the current work in progress, containing the new outline of material present in the original document as well as some new content.
