+++
# Project title.
title = "Predictors: Geographical Processes"

# Date this page was created.
date = 2018-12-01T00:00:00

# Project summary to display on homepage.
summary = "A set of tools for generating predictive hotspots of geographical point processes"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Predictors"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Photo by Toa Heftiba on Unsplash"

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++


# Introduction

This section introduces a set of predictive tools for certain geographical processes, such as crime and footfalls. The links to downloading these tools are also provided.

# 1. Grid-based Crime Hotspot Predictors

*Crime Hotspot* refers to an area with a high risk of crime. In practice, police are interested in crime hotspot in order to inform crime intervention. However, it requires the use of an analytical technique to identify hotspot areas and be able to rank them according to their level of severity. In a short-term crime intervention, the term *predictive hotspot* has been coined to represent hotspot types where crimes are expected to occur in a very near future, such as within one or two days. A number of analytical tools have been developed in order to model this type of hotspot - these are the types provided here. In addition, we provide an idea of the relative accuracies of these techniques.        

	**Self-Exciting Point Process**

	**Prospective Space-time Scan Statistics**

	**Prospective Kernel Density Estiamtion Method**

	**Prospective Hotspotting**

# 2. Footfall Predictor

This tool was developed as a part of the [Surf Project](http://surf.leeds.ac.uk/) funded by [ESRC Future Research Leaders](https://esrc.ukri.org/funding/funding-opportunities/future-research-leaders/) scheme. The tool, named as *Leeds Footfall Predictor*, built on the work led by [Dr. Nick Malleson](http://www.nickmalleson.co.uk/) which determined that the daily footfall rates observed in the Leeds city centre can be explained in terms of external variables, such as temperature, rainfall and holidays (See [here](https://github.com/nickmalleson/lcc-footfall/blob/master/LCC_Footfall.ipynb)). The research involved the application of different machine learning algorithms to a combination of these variables (predictors) and subsequently compared the accuracies of the former. It was established that the *Random Forest* algorithm by [Breiman, 2001](https://link.springer.com/article/10.1023/A:1010933404324) is the most accurate for forecasting footfall rates. Thus, the algorithm, as implemented in R by [Liaw and Wiener, 2002](https://www.r-project.org/doc/Rnews/Rnews_2002-3.pdf), was employed in the development of the Leeds Footfall Predictor. The tool was then deployed using the *RShinydashboard* platform. 



**Figures here (Developed by Monsuru Adepeju)**

Figure above shows the homepage of the tool. For further details about [Surf Project](http://surf.leeds.ac.uk/), please contact [Dr. Nick Malleson](http://www.nickmalleson.co.uk/) 




