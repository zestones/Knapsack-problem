# Knapsack problem 
The objective of this project is to implement some algorithms for solving the Knapsack Problem and to provide an experimental study of their running time and quality.
The algorithm implemented in this document are the followings: 
<ul>
    <li> The brute-force algorithm that explore all the possible solutions in a systematic way,</li>
    <li> Multiple branch and bound version </li>
    <ul>
        <li> DFS </li>
    </ul>
</ul> 

# Table of Contents
- [Knapsack problem](#knapsack-problem)
- [Table of Contents](#table-of-contents)
- [Installation](#installation)
  - [Jupiter Lab](#jupiter-lab)
  - [Python](#python)
- [Data \& Analyse](#data--analyse)
- [Architechture](#architechture)
  - [Main](#main)
  - [Class](#class)
  - [Source data](#source-data)
  - [Architecture of the result folder](#architecture-of-the-result-folder)


# Installation

## Jupiter Lab
To launch this you need Jupiter lab, we advice you to use it in VSCode.

## Python
You will need to have python on your machine and have or install the package listed in the main section in the project.

# Data & Analyse

For each algorithm we provide curves and tables inside the pdf files that are joined with this report, we give the references of these documents inside all the sections below. 
The curves and the graphs are in the folder ```results data/analysis/all```

# Architechture

The project is separated in different section, each section has a different purpose. You will find below the details of the architechture of this project.

## Main

The main section have all the import needed to run the program, we also define some constant and global variable.

## Class

In this section we will reference all the class used in the program
We can find the two principle class of the project, the item and solution class.

The Item class, is the class that represent an object that we will put in the knapsack, thus each item have a weight and value.
We will differentiate the items by their "id" (their position), inside the array named "choosed_items"

The Solution class, is the class that will store the solution computed by the alogorithm, this class will store the name of the algorithm that have solved the problem, the solution founded and some data about the memory usage during the computation of the algorithm. We will solve a probleme multiple time with different algorithm, that is why we created an array, called "problem_solutions" that will store the Solutions object.

## Source data
<p>There is two possibilities to test the algorithm. The data can be provided by the user from the terminal or the user can load the data from a dataset file that are in the dataset folder. </p>

> **NOTE**\
> If you load data from the dataset you musn't launch the generators.



## Architecture of the result folder
```
result-data
│   
│ 
└─── analysis.xlsx
│   
└─── raw
│   │   
│   │
│   └─── RANDOM
│   │   │   
│   │   └─── BRUTE FORCE   
│   │   │   │ 
│   │   │   └─── small 
│   │   │   │ res-10-10
│   │   │   │ res-10-100
│   │   │   │ res-10-1000
│   │   │   │
│   │   │   └─── medium
│   │   │   │ res-100-10
│   │   │   │ res-100-100
│   │   │   │ res-100-1000
│   │   │   │
│   │   │   └─── large
│   │   │   │ res-1000-10
│   │   │   │ res-1000-100
│   │   │   │ res-1000-1000
│   │   │
|   │   └───DYNAMIQUE
│   │   │    │ 
│   │   │    └─── small 
│   │   │    │ res-10-10
│   │   │    │ res-10-100
│   │   │    │ res-10-1000
│   │   │    │
│   │   │    └─── medium
│   │   │    │ res-100-10
│   │   │    │ res-100-100
│   │   │    │ res-100-1000
│   │   │    │
│   │   │    └─── large
│   │   │    │ res-1000-10
│   │   │    │ res-1000-100
│   │   │    │ res-1000-1000
│   │   │
│   │   └─── ...
│   │  
│   └─── NORMAL
│   │   │   
│   │   └─── BRUTE FORCE   
│   │   │   │ 
│   │   │   └─── small 
│   │   │   │ res-10-10
│   │   │   │ res-10-100
│   │   │   │ res-10-1000
│   │   │   │
│   │   │   └─── medium
│   │   │   │ res-100-10
│   │   │   │ res-100-100
│   │   │   │ res-100-1000
│   │   │   │
│   │   │   └─── large
│   │   │   │ res-1000-10
│   │   │   │ res-1000-100
│   │   │   │ res-1000-1000
│   │   │
│   │   └─── ...
│   └─── ...
```