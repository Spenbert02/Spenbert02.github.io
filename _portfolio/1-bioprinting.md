---
title: "NAATIV3: Nonplanar Architecture-Aligned Toolpathing for In-Vitro 3D Bioprinting"
# excerpt: "Toolpath generation algorithm for field-aligned 3D printing. The topic of my undergraduate honors thesis and my main focus as a staff researcher.<br/><img src='/images/ventricle_print_preview.png' width='50%'>"
excerpt: "<img src='/images/ventricle_print_preview.png' width='50%'>"
collection: portfolio
customdate: "September 2022 - June 2025"
---

<p class="page__date"><strong><i class="fa fa-fw fa-calendar" aria-hidden="true"></i> </strong>September 2022 - Present</p>

NAATIV3 is a path planning algorithm for 3D printing along specified fully-three-dimensional vector fields. The primary motivation is bioprinting for tissue engineering; in particular, NAATIV3 was used to 3D print a fiber-oriented human left ventricle model, obtained from diffusion MRI data.

<img src="/images/printed_ventricle.png" width="75%">

At a high level, NAATIV3 converts a boundary surface and internal vector field into a sequence of non-interfering toolpaths that yield a contiguous printed construct. For diffusion MRI-based printing, a scan must be segmented to obtain a boundary surface. Tensor fitting can then be implemented using a tractography suite (e.g. the DiPy Python library), yielding a primary fiber orientation field.

The algorithm operates by first generating a dense set of contours through numerical vector field integration (this process is identical to tractography). This set of 3D contours (example for the heart shown below) is reduced to a uniformly spaced representative subset via a cylinder-intersection based iterative exclusion procedure. The resulting subset is further reduced via graph-based interference prediction and finally ordered using heuristic search techniques, yielding a non-interfering, 3D printable toolpath sequence.

<img src="/images/ventricle_streams_ha.png" width="75%">

A major development is our novel thinning procedure that reduces an initially overdense contour set to a subset possessing a specified uniform inter-contour spacing. The thinning procedure executed on a human left ventricle model is shown below.

<!-- <iframe width="100%" height="500px" src="https://drive.google.com/file/d/1Zdr8TbQE6sfnC8JQvKBkxoWaAPP8g-ou/preview"></iframe> -->
<!-- <iframe src="https://drive.google.com/file/d/1Zdr8TbQE6sfnC8JQvKBkxoWaAPP8g-ou/preview" width="100%" height="480"></iframe> -->

<!-- <iframe src="https://drive.google.com/file/d/1Zdr8TbQE6sfnC8JQvKBkxoWaAPP8g-ou/preview" width="600" height="480"></iframe> -->
<!-- <iframe src="https://drive.google.com/file/d/1Zdr8TbQE6sfnC8JQvKBkxoWaAPP8g-ou/preview" frameborder="0" scrolling="no" onload="resizeIframe(this)" ></iframe> -->

<!-- <object width="100%" height="500px" data="https://drive.google.com/file/d/1Zdr8TbQE6sfnC8JQvKBkxoWaAPP8g-ou/preview"> -->

<iframe src="https://www.youtube.com/embed/xvew__NEOqs" frameborder="0" scrolling="no" onload="resizeIframe(this)" ></iframe>
