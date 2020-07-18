+++
# Project title.
title = "Under Review"
subtitle = "sdfsdfds"

# Date this page was created.
date = 2018-12-01T00:00:00

# Project summary to display on homepage.
summary = "Click to see list"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Delineators"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = " "
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

# Introduction

This section describes a set of analytical tools for delineating a geographical space. A *geographical space* refers to a large geographical area, such as a town or a  city, subdivided into a set of smaller administrative or non-administrative units.  An example of an administrative unit is a district, neighbourhood, county or ward demarcation, while an example of a non-administrative unit is a system of regular grid or street network.

In spatial analysis, it is often required to **modify** an existing geographical delineation or **create** a new one, based on a given specification. The following subsection will talk about two tools, one for creating a new geographical delineation (demarcation), and the other for modifying an existing geographical delineation. The link to download the tools are also provided.

# 1. Spatial grid generator: 
This tool creates a regular grid system over a geographical space. The tool requires a user to supply a spatial boundary of an area (in Esri format - .shp) and specify the grid size. The tool detects the spatial extent of the boundary and automatically create a system of regular grids, of the size specified, over the area. Although, it is possible to create regular grids in the existing GIS software, such as [*ArcGIS*](http://desktop.arcgis.com/en/) or [*QGIS*](https://www.qgis.org/en/site/), however, the process in these software is not straightforward. Therefore, the key purpose of our *Spatial grid generator* is to simplify this process. Below are examples regular grid systems of varying sizes, created by this tool, over the City of Chicago.

**Insert figs. here:**

**Potential Applications:**

The use of arbitrary grid system is common in crime analytics for some special reasons, which include confidentiality protection and as alternative in absence of a reasonably small adminstrative units. In particular, the grid systems have been used in hotspot policing in order to enable a more focussed targetting of problematic areas (Mohler et al. 2011).

This tool can be **downloaded** directly from [here](https://github.com/MAnalytics/Creating-a-spatial-grid-system-over-an-area)   

# 2. BDC_GeoConverter: 

This tool is developed to complement an online tool called [`Geoconverter`] (http://geoconvert.mimas.ac.uk/index.html). The Geoconverter is used for matching changed geographical units, or apportioning a dataset from an original geographical demarcation to a modified/changed geographical demarcation. For example, during 2011 UK census, it is observed that some census units, namely LSOAs and OAs, have been modified (either merged or split) when compared to their corresponding 2001 units. In Birmingham city for example, 10%* of 2011 LSOA units were affected. In a longitudinal analysis as an example, the aforementioned changes is *problematic*. 

In an effort to address this issue, the online Geoconverter tool is created, in order to apportion any data from 2001 census demarcation to 2011 census demarcation, or vice versa. Alternatively, the tool can be used to generate a *look-up table* that provides the details those changes that have occured for the entire UK. For example, for any given 2001 unit code, the look-up table provides the corresponding (set of) 2011 unit codes and the share (ratio) of 2001 unit that each has got. The table will give "1" for any unit that remain the same in both years.  

The look-up table is particularly useful for anyone who might wish to carry out the apportioning task programmatically.

Now, the *BDC_Geoconverter* is created to deal with one key problem that is not addressed by the online Geoconverter. The online Geoconverter fails to capture some OAs that exist in 2001 and still exist in 2011, but have now been renamed (i.e. re-coded). This scenario is most common in Scotland area where high-rise buildings were demolished and re-built as smaller building units.

**Please note** that the work of BDC_Geoconverter still depends largely on the look-up table generated from the online Geoconverter.

This tool was originally developed for the [Crime & Well_Being Big Data Centre](https://www2.mmu.ac.uk/crime-and-policing/big-data-centre/) and can be **downloaded** [here](https://github.com/MAnalytics/BDC-Geoconverter).








