# depdata
This repository stores the data collected in our ASE2020 paper-[Jin etal., Exploring the architectural impact of possible dependency in Python software, ASE,2020].
We provided the benchmarks collected from 105 open source projects for continued research of possible dependencies due to dynamic typing in Python software

Please reference this paper when you use our data.




## 1. 105-project-data

The 105 folders under this directory correspond to the dependency file and history data of 105 projects.

Under each folder,

1)**$projectname$_dep_explicit.json** 

It stores the file-level dependencies extracted by Understand tool, that we call **explicit dependencies**.

2)**$projectname$_dep_P$i$.json** (i=1,2,...,10) 

It stores the dependencies extracted by PyDepExtractor, that we call **possible dependencies**.

In particular,  $projectname$_dep_P11.json file stores the $P_{i>10}$ possible dependencies among files. 

3)**$projectname$_gitlog.txt** and **$projectname$_history.csv** store the revision history collected from git.



## 2. 105-project-analysis-summary
This directory include the analysis data of co-change capturing results, maintenance scores by DL and PC, dependency structure comparison, sub-space comparison, maintenance-groundtruth.

1)**python-projects-105.csv** 

This file lists the basic information of the projects that we investigated.


2)**dependency_structure_mojofm.csv** 

This file  lists the similarity between dependency structures created by D_e \union D_p1 and D_e only.


3)**cochange-capturing.csv** 

This file lists the  precison, recall, etc. measurements against 20 co-change benchmarks.

4)**The files whose name start with subspace-** 

These files list the detail and summarized data related to sub-spaces extracted by DRSpace technique. 

5)**DL_PC.xlxs** and **maintenance** 

They contain the dependency-based DL and PC maintenance scores, maintenance effors measured by six metrics mined from revision history.

## 3. PyDepExtractor-benchmarks

It includes the execution traces collected from 4 projects. See the four folders under this directory.

**P1-Pn-benchmarks.csv** 

This file lists the benchmarks collected from execution traces.
 
