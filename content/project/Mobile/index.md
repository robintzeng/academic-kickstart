---
title: Visual Inertia Navigation
summary: Navigate the drone with Openvins and the  learning based feature extractor -- Superpoint
tags:
- Robotics
- Computer Vision
- Machine Learning
date: "2020-03-27T00:00:00Z"

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
This project aims to adapt an open source visual
inertial navigation framework with two modifications. First, an
alternative visual descriptor and extractor, SuperPoint, is tested
in place of ORB features. Secondly, an invariant error state is
implemented in order to more effectively track the IMU pose
uncertainty while maintaining the visual feature correction step
in a ”dual track” system. Each of these changes is evaluated
separately on three datasets obtained from the [EuRoC MAV
dataset](https://projects.asl.ethz.ch/datasets/doku.php?id=kmavvisualinertialdatasets). Our code repository is located [here](https://github.com/robintzeng/EECS568_team_14_open_vins).

## Performance 
Evaluate the performance on the EuRoC  MAV dataset
{{< figure library="true" src="Traj.png" title="" lightbox="true" >}}  
{{< figure library="true" src="Table_RMSE.png" title="" lightbox="true" >}}  
{{< figure library="true" src="Error_med.png" title="" lightbox="true" >}} 
{{< figure library="true" src="Error_diff.png" title="" lightbox="true" >}}
{{< figure library="true" src="Table_Time.png" title="" lightbox="true" >}}
## Video
{{< youtube RPiYuu_pLAU >}}
