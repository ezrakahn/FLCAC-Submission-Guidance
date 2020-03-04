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

 
