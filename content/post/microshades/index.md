---
title: 'Do you see what I see? '
subtitle: 
summary: "Introducing microshades: An R package for improving color accessibility and organization of complex data"
authors:
- admin
tags:
- academia
categories: []
date: "2021-03-19T00:00:00Z"
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
image:
  focal_point: "Center"
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []

# Set captions for image gallery.
gallery_item:
- album: gallery
  caption: Default
  image: theme-default.png
- album: gallery
  caption: Ocean
  image: theme-ocean.png
- album: gallery
  caption: Forest
  image: theme-forest.png
- album: gallery
  caption: Dark
  image: theme-dark.png
- album: gallery
  caption: Apogee
  image: theme-apogee.png
- album: gallery
  caption: 1950s
  image: theme-1950s.png
- album: gallery
  caption: Coffee theme with Playfair font
  image: theme-coffee-playfair.png
- album: gallery
  caption: Strawberry
  image: theme-strawberry.png
---

Approximately 300 million people in the world have Color Vision Deficiency (CVD), which is comparable to the most recent estimate of the US population. Individuals with CVD do not experience a complete loss of color vision, though the ability to distinguish different colors is reduced.  When creating  figures and graphics that use color, it is important to consider that people with CVD will interact with this material, and may not perceive all of the information tied to the colors correctly.  There are multiple CVD friendly color palettes available on R to apply to visuals, however they are restricted to 8 different colors.  When working with complex data, such as microbiome data, this is insufficient.  

To overcome this limitation, we developed the microshades R package to provide custom color shading palettes that improve accessibility and data organization. Each color palette contains six base colors with five incremental light to dark shades, for a total of 30 available colors per palette type that can be directly applied to any plot. This package includes two crafted color palettes,  microshades_cvd_palettes and microshades_palettes.   The microshades_cvd_palettes contain colors that are universally CVD friendly. The individual microshades_palettes are CVD friendly, but when used in conjunction with multiple microshades_palettes, are not universally accessible.  

In addition to color palettes, the microshades package contains functions to aid in data visualization including functions for creating stacked bar plots organized by a data-driven hierarchy. The microshades package can be used in conjunction with common microbiome R packages, such as phyloseq, to enhance microbiome data visualization. In the case of microbiome data, the base colors correspond with a higher order taxonomic group (e.g. phylum) and shades of the base color represent subgroups of the taxonomic group (e.g. genus). Subgroup shading is determined by the abundance in the dataset. Darker shades indicate the most abundant subgroup for each group, and lighter shades represent less abundant subgroups. To further assist users with data storytelling, we have functions to sort data both vertically and horizontally based on ranked abundance or user specification.  The accessibility and advanced color organization features described help data reviewers and consumers notice visual patterns and trends easier. Examples of microshades in action are available on our website, for both microbiome and other datasets. 

 https://karstenslab.github.io/microshades 
