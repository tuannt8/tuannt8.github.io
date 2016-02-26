---
layout: paper
title:  "3D segmentation with tetrahedral mesh"
conf: "on going"
separateSum: "yes"
date:   2016-02-19 10:13:03 +0100
description:
categories: paper dsc segment 3D
---
{% include image-caption.html  img="/assets/paper/3D-hamster-thumbnail.jpg" width="400"%}
<!--more-->

This research segments CT scan images. We use tetrahedral mesh to represent the regions and deform the mesh to the desired solution. Mesh deformation is performed by `DSC` ([Deformable Simplicial Complex][DSC]).

## 3D segmentation
![](/assets/paper/3D-hamster.jpg)

## Slices from 3D scan
![](/assets/paper/hamster-scan.jpg)

[DSC]: https://github.com/janba/DSC
