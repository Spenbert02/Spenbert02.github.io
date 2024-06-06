---
title: "Bioprinting Toolpath Determination"
excerpt: "Toolpath generation algorithm for 3D bioprinting fiber-oriented cardiac constructs. The topic of my undergraduate honors thesis and my main focus as a staff researcher.<br/><img src='/images/bioprinting_portfolio_orig.png' width='50%'>"
collection: portfolio
customdate: "September 2022 - Present"
---

<p class="page__date"><strong><i class="fa fa-fw fa-calendar" aria-hidden="true"></i> </strong>September 2022 - Present</p>

During my last two years of undergraduate, and currently as a staff researcher, my main focus in the McAlpine Lab has been this project. We are developing a toolpath generation procedure for 3D bioprinting fiber-oriented cardiac constructs. We have implemented an array of computational procedures in Python and C to convert a diffusion MRI scan of a healthy human heart into a sequence of non-interfering toolpaths that yield a contiguous, fiber-oriented left ventricle. We manually segment a diffusion MRI scan of a healthy human heart, and implement tensor fitting using the DiPy Python library to effectively yield a voxel mask of the left ventricle and a primary fiber orientation field within the voxel mask. We generate a dense set of contours by integrating the primary fiber orientation field using numerical methods. This set of 3D contours (shown below) is reduced to a representative subset and ordered through a series of novel computational procedures, yielding a non-interfering, bioprintable toolpath sequence. We have demonstrated the feasibility of the algorithm by fabricating acellular silicone left ventricles in gelatin microparticle support baths.

<img src="/images/ventricle_ha.png" width="75%">
