+++
# Project title.
title = "Akmedoids v.0.1.5: for longitudinal data clustering"

# Date this page was created.
date = 2019-03-15T00:00:00

# Project summary to display on homepage.
summary = "A statistical package for grouping trajectories based on the similarities of their long-term trends "

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["akmedoids"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Featured image
# To use, add an image named `akmedoids.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  # caption = "Credit: terraimaging.com"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

# Introduction

Longitudinal clustering analysis is ubiquitous in social and behavioural sciences for investigating the developmental processes of a phenomenon over time. Examples of the commonly used techniques in these areas include group-based trajectory modelling (GBTM) and the non-parametric kmeans method. Whilst kmeans has a
number of benefits over GBTM, such as more relaxed statistical assumptions, generic implementations render it more sensitive to outliers and short-term fluctuations, which minimises its ability to identify long-term linear trends in data. 
In crime and place research, for example, the identification of such long-term linear trends may help to develop some theoretical understanding of criminal victimisation within a geographical space (Weisburd et al. [2004](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1745-9125.2004.tb00521.x); Griffith and Chavez [2004](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1745-9125.2004.tb00541.x)). In order to address this sensitivity problem, we advance a novel technique named anchored kmedoids ('akmedoids') which implements three key modifications to the existing longitudinal kmeans approach. First, it approximates trajectories using ordinary least square regression (OLS) and second, anchors the initialisation process with median observations. It then deploys the medoids observations as new anchors for each iteration of the expectation-maximisation procedure (Celeux and Govaert [1992](https://www.sciencedirect.com/science/article/pii/016794739290042E)). These modifications ensure that the impacts of short-term fluctuations and outliers are minimised. By linking the final groupings back to the original trajectories, a clearer delineation of the
long-term linear trends of trajectories are obtained.

# Application of 'akmedoids'

We encourage the use of 'akmedoids'
package outside of criminology, should it be appropriate. The R user manual and the vignette demonstrating the general application
of the package for longitudinal data clustering can be downloaded from [here](https://cran.r-project.org/web/packages/akmedoids/index.html).
