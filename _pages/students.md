---
layout: page
permalink: /students/
title: Open Thesis Topics 
nav: false
nav_order: 2
---



If you are interested in any of the topics below or have an idea of your own, please feel free to send an e-mail to [droege@cs.uni-bonn.de](mailto:droege@cs.uni-bonn.de).

---

## **3D Animal Reconstruction**
### Gaussian Splatting for Realistic Fur Textures  


This thesis project focuses on creating more visually realistic 3D animal models by improving existing reconstruction techniques. While models like [CASA (Category-Agnostic Skeletal Animal Reconstruction, NeurIPS 2022)](https://ivenwu.com/CASA/) have made significant progress in generating accurate skeletons and body shapes from 2D images, they lack fine surface details.

To address this, this thesis explores the use of Gaussian splatting to simulate intricate textures, such as fur, on CASA-generated meshes. The primary objectives include developing and optimizing a Gaussian splatting method for fur textures to improve the appearance of 3D animal models. Furthermore, there are also options for extending the system to include animations and/or capturing videos.

<!-- ![Alt text](/assets/img/casa.png){: style="width: 100%; height: auto;"} -->

<!-- *3D animal reconstruction. Image partly taken and modified from Wu, Yuefan, et al. "Casa: Category-agnostic skeletal animal reconstruction." Advances in Neural Information Processing Systems 35 (2022): 28559-28574.* -->

---

## **Deep Image Matting**
<!-- ## **Infrared Information for Real-Time Image Matting** -->
### Real-Time Matting: Improving Accuracy with Infrared Data

Real-time deep image matting is an important first step for many real-time reconstruction methods and an important part of the pipeline in the Capture-Dome. The objective is to improve real-time matting accuracy by incorporating additional infrared (IR) image data.

This approach builds on [Real-Time High-Resolution Background Matting](https://grail.cs.washington.edu/projects/background-matting-v2/) by encoding IR information alongside color data in the base structure of the matting network. This extra layer of IR data provides detail that color data alone can't capture, resulting in a much cleaner separation of foreground and background. To make this possible, we'll use the Mitsuba Renderer to simulate IR and color data, creating a realistic training dataset for the network.

<!-- ![Alt text](/assets/img/g1881.png){: style="width: 100%; height: auto;"}

*IR-assisted image matting. Image partly taken and modified from Lin, Shanchuan, et al. "Real-time high-resolution background matting." Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2021.* -->
![Alt text](/assets/img/IR.png){: style="width: 85%; height: auto;"}

*Camera Rig with two IR-Cameras (left, right), RGB-Camera (center left), and projector (center right).*


---

<!-- ## **Vision Transformer for Accurate Image Matting** -->
### Cross-Attention for Improved Background Integration


In contrast to real-time deep image matting, which prioritizes speed, offline methods focus on achieving the highest possible quality. In a capture-dome setup, where background matting benefits from capturing an additional empty scene, a robust solution is crucial for offline reconstruction approaches.

In this thesis the objective is to extend [Vision Transformer (ViT)-based matting](https://github.com/hustvl/ViTMatte) by replacing the traditional trimap input with a background image. Through the introduction of cross-attention between foreground and background embeddings, this approach aims to deliver more precise, context-aware matting. The key objectives include designing an effective cross-attention mechanism and achieving state-of-the-art performance in background replacement.

---

## **3D Pose Estimation**
### Multi View Landmark Detection
(Bachelorthesis)


In this thesis, we aim to integrate the [MediaPipe Pose Landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/pose_landmarker) into the Capture-Dome software for multiview 3D pose estimation. By utilizing MediaPipe’s robust 2D landmark detection across multiple synchronized camera views, the goal is to reconstruct accurate 3D poses.

<!-- ![Alt text](/assets/img/ViTMatte.png){: style="width: 100%; height: auto;"}

*Vision Transformer (ViT)-based matting. Image taken from Yao, Jingfeng, et al. "Vitmatte: Boosting image matting with pre-trained plain vision transformers." Information Fusion 103 (2024): 102091.*
 -->
