# M. Sc. Thesis: Temporal Dynamics in Generative Models

This repo contains the TeX sourcecode, figures, bibliography and the final pdf of my Master's thesis titled "Temporal Dynamics in Generative Models". 

The thesis was submitted in April, 2020 as the final part of my M. Sc. degree in Mathematics at the University of Freiburg, Germany. 

It was [awarded the Bernd Streitberg Award](http://www.biometrische-gesellschaft.de/en/nachwuchs/bernd-streitbergpreis/die-preistraeger.html)  of the German Region of the International Biometric Society (IBR-DR) in March, 2021.

## Abstract

Uncovering underlying development patterns in longitudinal biomedical data is a first step towards understanding disease processes, but is complicated by the sparse time grid and individual-specific development patterns that often characterise such data. In epidemiological cohort studies and clinical registries, we are facing the question of what can be learned from the data in an early phase of the study, when only a baseline characterisation and one follow-up measurement are available. Specifically, we considered a data scenario where an extensive characterisation is available at a baseline time point for each individual, but only a smaller subset of variables is measured again at an individually differing second time point, resulting in a very sparse (only two time points) and irregular time grid. 

Inspired by recent advances that allow to combine deep learning with dynamic modelling, we employed a generative deep learning model to capture individual dynamics in a low-dimensional latent representation as solutions of ordinary differential equations (ODEs). Here, the variables measured only at baseline are used to infer individual-specific ODE parameters. 

Additionally, we enriched the information of each individual by linking groups of individuals with similar underlying trajectories, which then serve as proxy information on the common temporal dynamics. Irregular spacing in time can thus be used to gain more information on individual dynamics by leveraging individuals’ similarity. 

Using simulated data, we showed that the model can recover individual trajectories from linear and non-linear ODE systems with two and four unknown parameters and infer groups of individuals with similar trajectories. The results illustrate that dynamic deep learning approaches can be adapted to such small data settings to provide an individual-level understanding of the dynamics governing individuals’ developments. 

## Code 

The model developed in the thesis is written in [Julia](https://julialang.org). Code for training the model and for reproducing (most) figures in the thesis is available [here](https://github.com/maren-ha/DeepDynamicModelingWithJust2TimePoints). 
