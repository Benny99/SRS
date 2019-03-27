.. _topics-列表:

=========
1.Introduction
=========
::
    This SRS describes the development process of wed online application
     for OMG(Oh My Genes), which not only gives us a preliminary 
     understanding of how to write SRS, but more importantly, enables 
     biologists to quickly find differences in the numerous and complex gene 
     expression documents.

----------------
1.1 Purpose
----------------
::The differentially expressed genes were rapidly and accurately screened 
and expressed in the gene expression files of the two cells.
----------------
1.2 Scope
----------------
::The OMG's application is currently limited to two gene files that contain 
samples from different cells, but its scope covers all known genes in 
    nature, even those that have not been discovered, because they are all the 
    result of different sequences of four base pairs 
----------------
1.3 Acronyms and Abbreviations
----------------
::  The acronym and abbreviation of this Web application is OMG.It means 
On My Genes. But I want to name the file by WAO.It means web 
application OMG.
----------------
1.4 Overview
----------------
::   With the continuous progress of computer technology and its application 
in the field of biological information, it is becoming more and more
 convenient and practical to use computer programs to update gene
  expression files and screen gene files with expression differences. The 
  application of OMG related programs is bound to promote biologists' 
  research on genes.
----------------
1.5 Terminologies
----------------
Log2 FC & Log2 CPM:
----------------
::   Log2 CPM are the log counts per million, which can be understood as 
measuring expression level. Log2 FC is the log fold-change, which is the
 log difference between your groups.
 Edger is giving you the output appropriate for whatever you gave it. You 
 gave it 30,000 genes, so it gave you 30,000 results. Presumably you have 
 a bunch of non-coding genes in there.

=========
2.Generic Requirement
=========
----------------
2.1Features
----------------
::  The OMG application must be simple, fast, and intuitive to run, and it can
 be used by biologists to analyze data, process data, and sift through it.The 
 OMG also have a submit button.It is Filtrate.After importing the data of 
 the two gene files, we only need to click this button lightly to realize the 
 rapid screening of the data.
----------------
 2.2Sample Input
----------------
::   We use our imported gene files and click the screen button to achieve 
perfect screening.The content format of the imported gene file must be 
the same as the format given below.The sample input as follows:

+------------+------------+-----------+ 
|Gene_Id  	|Control Sample|	Knock Out Sample|
+============+============+===========+
|AT1G01010	|1.198558083	|2.036161827|
+------------+------------+-----------+ 
|AT1G01020	|13.75736234	|13.370796|
+------------+------------+-----------+ 
|AT1G01030	|0.833779536|	0.203616183|
+------------+------------+-----------+ 
|AT1G01040	|9.58846466	|7.126566394|
+------------+------------+-----------+ 
|AT1G01046	|0         |	0|
+------------+------------+-----------+ 
|AT1G01050	|23.81482799	|21.10821094|
+------------+------------+-----------+ 
|AT1G01060	|0.625334652|	1.221697096|
+------------+------------+-----------+ 
|AT1G01070	|1.719670292	|0.950208853|
+------------+------------+-----------+ 
|AT1G01080	|28.34850421	|25.24840665|
+------------+------------+-----------+ 
|AT1G01090	|58.26034505	|42.96301455|
+------------+------------+-----------+ 
|AT1G01100	|1066.508249	|1308.030358|
+------------+------------+-----------+ 
|AT1G01110	|2.709783491|	1.425313279|
+------------+------------+-----------+ 
|AT1G01120	|51.32955266	|44.32045576|
+------------+------------+-----------+ 
|AT1G01130	|1.094335641	|0.814464731|
+------------+------------+-----------+ 
|AT1G01140	|18.1347049	|15.20334164|
+------------+------------+-----------+ 
|AT1G01150	|0.104222442	|0|
+------------+------------+-----------+ 
|AT1G01160	|21.93882403	|20.09013002|
+------------+------------+-----------+ 
|AT1G01170	|43.35653585	|36.58304082|
+------------+------------+-----------+ 
|AT1G01180	|2.13656006	|5.022532506|
+------------+------------+-----------+ 
|AT1G01183	|0	|          0|
+------------+------------+-----------+ 
|AT1G01190	|4.064675236	|3.732963349|
+------------+------------+-----------+ 
|AT1G01200	|0.729557094	|0.135744122|
+------------+------------+-----------+ 
|AT1G01210	|4.950565993	|6.787206089|
+------------+------------+-----------+ 
|AT1G01220	|5.523789424	|4.818916323|
+------------+------------+-----------+ 
----------------
2.3Sample Output
----------------
::  Output results must be concise, if the input data does not meet the format 
requirements, the program will warn and prompt to re-enter the data in 
the correct format, otherwise it will not run.The format of the output is 
preferably tabular.Like this:
+------------+------------+-----------+ 
|Gene_Id  	|Control Sample|	Knock Out Sample|
+============+============+===========+
|AT1G01010	|1.198558083	|2.036161827|
+------------+------------+-----------+ 
=========
3.Special Requirements
=========
----------------
3.1Supportability
----------------
::  This application supports the processing of files containing cell gene data,
 but these files must be imported according to a certain format.
  The format is as follows: gene name is Gene_Id, control group name is Control 
  Sample , sample name is Knock Out Sample. Failure to follow this format 
  will return to the input page until the correct format is entered.
----------------
3.2Response time
----------------
  ::    Ideal response time is less than 8 seconds
----------------
3.3Matters Need Attention
----------------
*Because it involves the processing of genetic data, website 
applications must be stable and the network environment must be
 secure.
*The style of the website application must be simple, the application 
must be easy to use, and it will not cost the users much to learn and
 use.
*In order to make the results of data processing have scientific value 
and high reference value, the data sources must be reliable, preferably
 the data of research institutes.
*Use this website application program according to the requirements, 
imported data please do a good backup, this website only get the final
 result, in the process may lose data.
=========
4.Limits
=========
----------------
4.1Space
----------------
::The application space required by the website should not exceed 2G.
----------------
4.2Budget
----------------
::The budget for the development of the website application is about
 55,000 yuan.
----------------
4.3Browser
----------------
::Website applications should support the current mainstream browsers on 
the market and should be optimized accordingly.
----------------
4.4Frequency
----------------
::Web applications should be available at any time and can withstand heavy 
workloads.
=========
5.Change Cases
=========
::  The content of SRS is not unchanged. As time goes on, the user's needs 
may change at any time in the development process. At this time, it is
 necessary to make appropriate modifications to SRS to meet the user's 
 requirements, and even the direction of development will change. At this 
 time, the latest documents should prevail.
=========
6.Appendices
=========
=========
7.References
=========
1.https://blog.csdn.net/a201577f0546/article/details/78867756?tdsourcetag=s_pctim_aiomsg
2.http://avnpc.com/pages/writing-best-documentation-by-sphinx-github-readthedocs 
3.https://www.jianshu.com/p/78e9e1b8553a 
4.http://www.sphinx-doc.org/en/stable/config.html