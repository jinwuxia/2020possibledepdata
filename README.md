# depdata

This repository stores the data collected in our ASE2020 paper and ongoing work：

## [Jin etal., Exploring the architectural impact of possible dependency in Python software, ASE,2020].

We provided the benchmarks collected from 105 open source projects for continued research of possible dependencies due to dynamic typing in Python software

## Please reference our paper when you use this dataset.




## 1. 105-project-data

The 105 folders under this directory correspond to the dependency file and history data of 105 projects.

Under each folder,

1)**$projectname$_dep_explicit.json** 

It stores the file-level dependencies extracted by Understand tool, that we call **explicit dependencies**.

2)**$projectname$_dep_P$i$.json** (i=1,2,...,10) 

It stores the  **possible dependencies**.

In particular,  $projectname$_dep_P11.json file stores the $P_{i>10}$ possible dependencies among files. 

3)**$projectname$_gitlog.txt** and **$projectname$_history.csv** store the revision history collected from git.



## 2. depverify-benchmarks

**P1-Pn-benchmarks.csv** 

This file lists the benchmarks collected from execution traces.
 
