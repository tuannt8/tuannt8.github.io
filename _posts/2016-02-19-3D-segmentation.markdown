---
title: 3D segmentation with tetrahedral mesh
date: 2016-02-19 09:13:03 Z
categories:
- paper
- dsc
- segment
- 3D
layout: paper
conf: on going
separateSum: 'yes'
description: 
---

{% include image-caption.html  img="/assets/paper/3D-hamster-thumbnail.jpg" width="400"%}
<!--more-->

This research segments CT scan images. We use tetrahedral mesh to represent the regions and deform the mesh to the desired solution. Mesh deformation is performed by `DSC` ([Deformable Simplicial Complex][DSC]).

## 3D segmentation
![](/assets/paper/3D-hamster.jpg)

## Slices from 3D scan
![](/assets/paper/hamster-scan.jpg)

[DSC]: https://github.com/janba/DSC
