---
title:  "Introduction to Genetic Algorithm"
date:   2020-04-05
layout: single
author_profile: true
comments: true
tags: [Algorithm]
---

Genetic Algorithm is a numerical approach to solve a optimization problem. You could maximize or minimize some loss functions to find the best/optimized set of parameters. The logic of this algorithm is inspired by nature and natural selection involving in population genetical heredity activities. 

## Algorithms




## Hyperparameter Tunning
You need to specify few hyperparameters before the natural selection started, such as population size, ratio of offspring with changed parameters, mutation rate, number of maximum migration and so on. It is not easy to find the best set of hyperparameters since the computational burden. The followings will have information about how to tunning the hyper-parameters.<br/>
Generally, we have the following hyper-parameters to tune:
- Number of Generations;
- Number of population;
- Mutation Rate;
- Mutation percentage on population;
- Crossover percentage on population;

Among these parameters mutation rate must be very low, as low as 0.05 or even smaller. Because the higher value could destroy the solution. Mutation percentage and crossover percentage are depends on the problem and their own efficiency that you could find an optimal value for them by different runs. If you could settle an optimal value for these three parameters, the other first two parameters would be settled simply.
