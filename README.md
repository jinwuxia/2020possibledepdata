# depdata

This repository stores the data collected in our previous ASE work and ongoing work.

We provided the benchmarks collected from 105 open source projects for continued research of possible dependencies due to dynamic typing in Python software


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
 
 
 
## Please reference our paper when you use this dataset.
@inproceedings{2020ase-jin,
	title={Exploring the Architectural Impact of Possible Dependencies in Python Software},
	author={Jin, Wuxia and Cai, Yuanfang and Kazman, Rick and Zhang, Gang and Zheng, Qinghua and Liu, Ting},
	booktitle={2020 35th IEEE/ACM International Conference on Automated Software Engineering (ASE)},
	pages={1--13},
	year={2020},
	organization={IEEE}
}

