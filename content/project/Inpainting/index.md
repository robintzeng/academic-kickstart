---
title: Video Inpainting Benchmark
summary: Divide the videos’ motion into binary labels and evaluated those videos’ difficulties for the video inpainting task.
tags:
- Computer Vision
date: "2020-12-27T00:00:00Z"

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
When evaluating video inpainting methods, people often use different video sources. Commonly-used datasets are video segmentation datasets like DAVIS 2017 and YouTube-VOS  because  they  provide  foreground  masks. However, they are not specifically designed for video inpainting: they don’t give labels to indicate whether the video is hard for video inpainting, and if so, why. 

For this reason, we propose attributes that are likely to affect the video inpainting model performance — camera motion, foreground motion, background scene motion, and foreground displacement — and  label  them  on  DAVIS  2017. This can help us evaluate those videos’ difficulties for the video inpainting task. However, labeling a video objectively is a challenge for humans since everyone has their own criterion; therefore, we propose a set of automatic classifiers. We hope the new-annotated dataset will be a guide for researchers to improve their algorithms.



## Classifier Performance 
In the new dataset, we divide the videos’ motion into binary labels. It will be either high motion video or low motion video and evaluate the performance on the DAVIS dataset.
1. **Camera motion**
{{< figure library="true" src="VP_camera_motion.png" title="" lightbox="true" >}}  

In low camera motion video, most of the background textures are observed in both frames and that they are completely different on the right.
{{< figure library="true" src="VP_camera_motion_curve.png" title="Camera Motion Performance" lightbox="true" >}}  

2. **Foreground motion**
{{< figure library="true" src="VP_foreground_motion.png" title="" lightbox="true" >}}
In a low foreground motion video, the foreground object’s appearance is consistent across the frames. However, in high foreground motion video, the object tends to change its posture very much.
{{< figure library="true" src="VP_foreground_motion_curve.png" title="Foreground Motion Performance" lightbox="true" >}}

3. **Background scene motion**
{{< figure library="true" src="VP_scene_motion.png" title="" lightbox="true" >}}
The high scenic motion video will obtain moving components like water in the background, and the low scenic motion video will obtain static backgrounds like rock and trees.
{{< figure library="true" src="VP_bg_scene_motion_score.png" title="Background Scene Motion Performance" lightbox="true" >}}

4. **Foreground displacement**
{{< figure library="true" src="VP_foreground_displacement.png" title="" lightbox="true" >}}
The high foreground displacement videos can often reveal different parts of the occluded background over time.

{{< figure library="true" src="VP_fg_displacement_score.png" title="Foreground Displacement Performance" lightbox="true" >}}