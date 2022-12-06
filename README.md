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
- [Architechture](#architechture)
  - [Main](#main)
  - [Class](#class)
  - [Generator](#generator)
  - [Algorithm](#algorithm)
  - [Test](#test)
    - [Generator](#generator-1)
    - [Test akgorithm](#test-akgorithm)
- [Running instruction](#running-instruction)
  - [Run several test](#run-several-test)
  - [Display Solutions](#display-solutions)
- [Data result](#data-result)
  - [Export data result](#export-data-result)
  - [Architecture of the result folder](#architecture-of-the-result-folder)
  - [Import data to excel](#import-data-to-excel)


# Installation

## Jupiter Lab

## Python

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

## Generator
## Algorithm
## Test
### Generator
### Test akgorithm

# Running instruction

## Run several test
## Display Solutions
# Data result
## Export data result

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
## Import data to excel