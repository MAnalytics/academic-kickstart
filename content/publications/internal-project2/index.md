+++
# Project title.
title = "Published"

# Date this page was created.
date = 2018-12-01T00:00:00

# Project summary to display on homepage.
summary = "Click to see list"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Simulators"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Credit: terraimaging.com"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

# Introduction

Geographical processes such as crime, diseases, and pedestrian footfalls are extremely difficult to synthesise - they are inherently complex, and the theories for describing them are constantly evolving. 

Researchers often find themselves in a very precarious situation when carrying out real-life research projects, where data required to complete such projects are unavailable. Evidently, there are a number of legitimate reasons why such data might not be available, including confidentiality issues and the lack availability of usable data formats. 

To the credit of some computer/geospatial scientists, certain successes have been achieved in the areas of geographical modelling through computer simulation approach. However, many of these simulations are often too tailored towards a single problem and may not be extensible to other related problems. 

In this section, I introduce a *dynamic microsimulation framework* for simulating *crime patterns*. Patterns, arising from offenders routines activities have both spatial and temporal signatures of different types. Thus, this framework is aimed at allowing different combinations of these spatio-temporal signatures to be simulated.  

This framework was originally described [here](http://eprints.whiterose.ac.uk/128602/1/monsuru_adepeju_gisruk2018.pdf).  


# A dynamic microsimulation framework for simulating different spatio-temporal crime patterns (DMfC).

In the field of animal ecology, *foraging animals* are known to act cautiously in relation to the locations they prey - while in pursuit of food, they do not want to become foods for others.  In the field of criminology, this behavioural pattern has been likened to that of a human offender who carefully chooses his victims while, at the same time, avoiding being arrested. In constrast to criminology, a considerable progress has been made in modelling these foraging behaviours in animal ecology using computer simulation (Morales et al., [2004]( https://esajournals.onlinelibrary.wiley.com/doi/full/10.1890/03-0269); McClintock et al., [2012]( https://esajournals.onlinelibrary.wiley.com/doi/abs/10.1890/11-0326.1)). This *DMfC* builds on this progress and adapt the [*SimRiv*]( https://cran.r-project.org/web/packages/SiMRiv/SiMRiv.pdf) R-package (Quaglietta and Porto, [2017]( https://cran.r-project.org/web/packages/SiMRiv/SiMRiv.pdf)) to synthesise a set of offenders and their potential victims within a hypothetical, constraint environment. 

The DMfC allows the user to specify the levels of spatial clustering and the type of temporal patterns to simulate. The interaction between spatial and temporal specifications results into a unique spatio-temporal pattern, which can be used for further crime studies. The *DMfC* tool can be downloaded from [here](https://github.com/MAnalytics/DMfC/blob/master/DataSynthUsingR/SyntheticData_OptimalForaging.Rmd).

