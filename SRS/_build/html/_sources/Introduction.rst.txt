Introduction
=========

This SRS describes the development process of wed online application
for OMG(Oh My Genes), which not only gives us a preliminary 
understanding of how to write SRS, but more importantly, enables 
biologists to quickly find differences in the numerous and complex
gene expression documents.

Purpose
----------------
The differentially expressed genes were rapidly and accurately screened 
and expressed in the gene expression files of the two cells.

Scope
----------------
The OMG's application is currently limited to two gene files that contain 
samples from different cells, but its scope covers all known genes in 
nature, even those that have not been discovered, because they are all the 
result of different sequences of four base pairs 

Acronyms and Abbreviations
----------------
The acronym and abbreviation of this Web application is OMG.It means 
On My Genes. But I want to name the file by WAO.It means web 
application OMG.

Overview
----------------
With the continuous progress of computer technology and its application 
in the field of biological information, it is becoming more and more
convenient and practical to use computer programs to update gene
expression files and screen gene files with expression differences. The 
application of OMG related programs is bound to promote biologists' 
research on genes.

Terminologies
----------------
Log2 FC & Log2 CPM:

Log2 CPM are the log counts per million, which can be understood as 
measuring expression level. Log2 FC is the log fold-change, which is the
log difference between your groups. 

Edger is giving you the output appropriate for whatever you gave it. You 
gave it 30,000 genes, so it gave you 30,000 results. Presumably you have 
a bunch of non-coding genes in there.