---
title:  "Introduction to Genetic Algorithm"
date:   2020-04-05
layout: single
author_profile: true
comments: true
tags: [Algorithm]
---


# Genetic Algorithm Tutorial

## Introduction
Genetic Algorithm is a numerical approach to solve a optimization problem. You could maximize or minimize some loss functions to find the best/optimized set of parameters. The logic of this algorithm is inspired by nature and natural selection involving in population genetical heredity activities. 

## Algorithms
### Population Initialization


### Genetic Operators
1. Selection <br/>
Selection is the means of choosing two chromosomes as parents to generate offspring. Among these two selected chromosomes, the better fit one will be set as "Dad" and another one will be set as "Mom". There exist several different approaches for the selection probability calculation. The most generally used one is "linear Ranking". Also, "roulette wheel" approach could help to determine how likely the chromosomes is to be seleted with consideration of all chromosomes' fitness.
2. Crossover <br/>
Once two chromosomes are slected, corssover operator will be implemented to produce the offsprings. Crossover can be single point, twp points, or many points of interchange of information among the chromosomes. The decision of passing to next generation will be made based on some criterion, such as meeting a minimum fitness or replace the worst fittness chromosomes in the related population. Possible cross-over operators are listed in the followings:
  * Copying the better fit into next generation (Single or Multiple parameters);
  * Taking average value between "dad" and "mom" (Single or Multiple parameters);
  * Interchanging the chromosomes' information (Multiple parameters Only);
3. Mutation  <br/>
There exist possibility that the chromosome's information not inherit from parents. You can set your own rules for mutation. For example, randomly adding a random or fixed amount values to the exited chrosome or randomly selected from other possible candidates in parameter space;
4. Inversion (Optional) <br/>
For some of the application example, Inversion could be another oeprator, which is randomly shuffling of genes within a chromosome. Inversion has not been used in most genetic algorithms since the crossover and mutation have already effectively catch the similar information from the population;

### Termination Criterion


### Hyperparameter Tunning
You need to specify few hyperparameters before the natural selection started, such as population size, ratio of offspring with changed parameters, mutation rate, number of maximum migration and so on. It is not easy to find the best set of hyperparameters since the computational burden. The followings will have information about how to tunning the hyper-parameters.<br/>
Generally, we have the following hyper-parameters to tune:
- Number of Generations;
- Number of population;
- Mutation Rate;
- Mutation percentage on population;
- Crossover percentage on population;

Among these parameters mutation rate must be very low, as low as 0.05 or even smaller. Because the higher value could destroy the solution. Mutation percentage and crossover percentage are depends on the problem and their own efficiency that you could find an optimal value for them by different runs. If you could settle an optimal value for these three parameters, the other first two parameters would be settled simply.

## Summary
### Advantages
### Dsiadvantages
