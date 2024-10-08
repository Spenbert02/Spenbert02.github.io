---
title: "Freeform three-dimensional orientation field-aligned 3D printing"
excerpt: "Toolpath generation algorithm for field-aligned 3D printing. The topic of my undergraduate honors thesis and my main focus as a staff researcher.<br/><img src='/images/ventricle_print_preview.png' width='50%'>"
collection: portfolio
customdate: "September 2022 - Present"
---

<p class="page__date"><strong><i class="fa fa-fw fa-calendar" aria-hidden="true"></i> </strong>September 2022 - Present</p>

During my last two years of undergraduate, and currently as a staff researcher, my main focus in the McAlpine Lab has been this project. We are developing a toolpath generation procedure for 3D printing along specified fully-3D vector fields. Our primary motivation is bioprinting for tissue engineering; in particular, we want to bioprint a fiber-oriented model of the human left ventricle, obtained from diffusion MRI data. However, our current instantiation is fully generalizable. We have implemented a computational pipeline that converts a boundary surface and internal vector field into a sequence of non-interfering toolpaths that yield a contiguous print. For cardiac bioprinting, we manually segment a diffusion MRI scan of a healthy human heart, and implement tensor fitting using the DiPy Python library to effectively yield a voxel mask of the left ventricle and a primary fiber orientation field within the voxel mask.

The algorithm operates by first generating a dense set of contours through numerical vector field integration. This set of 3D contours (example for the heart shown below) is reduced to a uniformly spaced representative subset and ordered through a series of novel computational procedures, yielding a non-interfering, 3D printable toolpath sequence.

<img src="/images/ventricle_streams_ha.png" width="75%">

A major novel development is a thinning procedure that selects a uniformly spatially distributed subset of an initially overdense contour set. The thinning procedure executed on a human left ventricle model is shown below.
