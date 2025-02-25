---
title: Depth Completion
summary: Developed a learning structure to estimate a dense depth image from sparse depth measurements.
tags:
- Depth Completion
- Computer Vision
- Machine Learning
date: "2020-03-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

#image:
#  caption: Photo by rawpixel on Unsplash
#  focal_point: Smart


# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---
{{< figure library="true" src="model.png" title="Fig. 1 Two Pathway" lightbox="true" >}}

## Abstract
We develop the learning architecture that can effectively complete the dense depth from a **color image** and **sparse LiDAR** data. 

Our model consists of two pathways: the **local pathway** and the **global pathway** which is illustrated in Fig 1. The local pathway aims to extract high-resolution features, and it is made up of 2D blocks, which is illustrated in Fig. 2(b). The global pathway extracts low-resolution features, and it comprises our proposed U-Block, as shown in Fig. 2(a). The structure of the pathway is illustrated in Fig 3. 

Also, we improve the performance of the local pathway by concatenating binary mask to the sparse LiDAR data, because the binary mask can help our model to indicate the valid values of sparse LiDAR data. 

Finally, to combine the results of the local and global pathways, we apply the attention mechanism (confidence map) to integrate the predicted dense from two pathways. 

{{< figure library="true" src="block.png" title="" lightbox="true" >}}

{{< figure library="true" src="pathway_struct.png" title="" lightbox="true" >}}



{{< figure library="true" src="confidence.png" title="" lightbox="true" >}}

{{< figure library="true" src="performance.png" title="" lightbox="true" >}}