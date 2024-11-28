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

![Alt text](/assets/img/casa.png){: style="width: 100%; height: auto;"}

*3D animal reconstruction. Image partly taken and modified from Wu, Yuefan, et al. "Casa: Category-agnostic skeletal animal reconstruction." Advances in Neural Information Processing Systems 35 (2022): 28559-28574.*

---

## **Infrared Information for Real Time Image Matting**
### Enhancing accuracy with infrared data

Real-time deep image matting is an important first step for many real-time reconstruction methods and an important part of the pipeline in the Capture-Dome. The objective is to improve real-time matting accuracy by incorporating additional infrared (IR) image data.

This approach builds on [Real-Time High-Resolution Background Matting](https://grail.cs.washington.edu/projects/background-matting-v2/) by encoding IR information alongside color data in the base structure of the matting network. This extra layer of IR data provides detail that color data alone can't capture, resulting in a much cleaner separation of foreground and background. To make this possible, we'll use the Mitsuba Renderer to simulate IR and color data, creating a realistic training dataset for the network.

![Alt text](/assets/img/g1881.png){: style="width: 100%; height: auto;"}

*IR-assisted image matting. Image partly taken and modified from Lin, Shanchuan, et al. "Real-time high-resolution background matting." Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 2021.*

---

## **Preview-Image-Interpolation**
### Smoother Transitions in Static Scenes

In the capture-dome setup, where multiple cameras capture static images of a subject from different angles, we need a smooth preview function for visualizing the subject dynamically. Currently, we are limited to static frame-by-frame previews, which lack the user experience. 

To address this, our goal is the development of an interpolation technique that generates intermediate frames between captured images. Given a static scene and fix camera positions, this thesis is supposed to adapt existing frame interpolation techniques as [https://film-net.github.io/](https://film-net.github.io/) to the given setting by e.g. integrating a three-image interpolation.
