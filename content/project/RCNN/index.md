---
title: Improvements on Object Detection (Faster R-CNN)
summary: Modified the backbone, detection head and RPN to imporve the performace of Faster R-CNN
tags:
- Computer Vision
- Machine Learning
date: "2020-12-30T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart


# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---
## Abstract
In this project, the main goal is to investigate the object detection model architecture to improve the mean Average Precision (mAP). In the past, researchers are dedicated to proposing new ideas in each part of the network architecture to enhance model performance. However, each method is a stand-alone little piece. It remains unclear if we can take advantage of these little pieces to push the model performance. Therefore, we aim to combine these refinements made in each architecture to investigate whether the model performance can be even better.  Our modifications are based on Faster R-CNN with Feature Pyramid Network (FPN) to improve the model performance, including backbone, Region Proposal Network, feature maps refinement and RoI head.

Our code repository is located [here](https://github.com/robintzeng/mask-rcnn-Pytorch).

## Performance 
Evaluate the performance on the PASCAL 2007 dataset
{{< figure library="true" src="FAST_RCNN_result.png" title="" lightbox="true" >}}  
{{< figure library="true" src="FAST_RCNN_result1.png" title="" lightbox="true" >}}  


