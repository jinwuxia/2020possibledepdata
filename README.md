# DataSet

This repository stores the data collected for our previous ASE work and ongoing work.

We provided the benchmarks collected from 105 open source projects for continued research of possible dependencies due to dynamic typing in Python software


## 1. 105-project-data

The 105 folders under this directory correspond to the dependency file and history data of 105 projects.

In each folder,

1)**$projectname$_dep_explicit.json** 

It stores the file-level dependencies extracted by Understand tool, that we call **explicit dependencies**.

2)**$projectname$_dep_P$i$.json** (i=1,2,...,10) 

It stores the  **possible dependencies**.

In particular,  $projectname$_dep_P11.json file stores the $P_{i>10}$ possible dependencies among files. 

3)**$projectname$_gitlog.txt** and **$projectname$_history.csv** store the revision history collected from git.



## 2. depverify-benchmarks

**P1-Pn-benchmarks.csv** 

This file lists the benchmarks collected from execution traces.
 
 
## 3. dependencies-from-stubs

This folder contains the data for several projects and the corresponding stub projects. The stub projects contains Python code with type annotations.

1)**projects-with-stubs.csv**

It lists the projects which have stub files. 
The code URLs, Stub URL, and versions are also provided.

2)**stub-deps**

Each subfolder corresponds to one project, including:
 
$*-P1.json$ contains the $P_1$ possible dependencies extracted from the methods in ASE work.

$*-stub-P1.json$ contains the $P_1$ possible dependencies extracted from the stub files.

3)**dependency-summary.csv**

This file illustrates the dependency extraction results, comparing ASE method (see (D(ase)) vs. the updated method (see D(ase+stub)).

# Tool
You can use [ENRE](https://github.com/jinwuxia/ENRE) to collect possible dependencies.

# Reference

You can reference the following papers if you use this dataset and our ENRE tool, or feel interested in knowing more.


    @inproceedings{2020ase-jin,
        title={Exploring the Architectural Impact of Possible Dependencies in Python Software},
		
        author={Jin, Wuxia and Cai, Yuanfang and Kazman, Rick and Zhang, Gang and Zheng, Qinghua and Liu, Ting},
        booktitle={2020 35th IEEE/ACM International Conference on Automated Software Engineering (ASE)},
        pages={1--13},
        year={2020},
        organization={IEEE}
        }

    @inproceedings{2019icse-jin,
      title={ENRE: a tool framework for extensible eNtity relation extraction},
	  
      author={Jin, Wuxia and Cai, Yuanfang and Kazman, Rick and Zheng, Qinghua and Cui, Di and Liu, Ting},
      booktitle={Proceedings of the 41st International Conference on Software Engineering: Companion Proceedings},
      pages={67--70},
      year={2019},
      organization={IEEE Press}
    }

