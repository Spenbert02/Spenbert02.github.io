---
title: "NAATIV3"
# excerpt: "Toolpath generation algorithm for field-aligned 3D printing. The topic of my undergraduate honors thesis and my main focus as a staff researcher.<br/><img src='/images/ventricle_print_preview.png' width='50%'>"
excerpt: "<img src='/images/ventricle_print_preview.png' width='50%'>"
header:
  teaser: "ventricle_print_preview.png"
collection: portfolio
order: 2
codeurl: "https://license.umn.edu/product/3d-vector-field-guided-toolpathing-for-3d-bioprinting"
---

NAATIV3 plans 3D-printing paths that follow a fully three-dimensional direction field, for bioprinting tissue whose function depends on its fiber orientation. From a diffusion MRI scan of a human heart, it traces the muscle fibers, thins them to evenly spaced paths, and orders the paths so the nozzle never collides with printed material. At its core are Runge–Kutta streamline integration, swept-volume collision detection, NP-hard graph optimization, and heuristic search, implemented in Python and C. It was used to print a fiber-oriented model of a human left ventricle, published in <a href="https://doi.org/10.1038/s44172-025-00489-0" target="_blank">Nature Communications Engineering</a>.

<img src="/images/printed_ventricle.png" width="75%">

<img src="/images/ventricle_streams_ha.png" width="75%">

The thinning step on a left ventricle model:

<!-- <iframe width="100%" height="500px" src="https://drive.google.com/file/d/1Zdr8TbQE6sfnC8JQvKBkxoWaAPP8g-ou/preview"></iframe> -->
<!-- <iframe src="https://drive.google.com/file/d/1Zdr8TbQE6sfnC8JQvKBkxoWaAPP8g-ou/preview" width="100%" height="480"></iframe> -->

<!-- <iframe src="https://drive.google.com/file/d/1Zdr8TbQE6sfnC8JQvKBkxoWaAPP8g-ou/preview" width="600" height="480"></iframe> -->
<!-- <iframe src="https://drive.google.com/file/d/1Zdr8TbQE6sfnC8JQvKBkxoWaAPP8g-ou/preview" frameborder="0" scrolling="no" onload="resizeIframe(this)" ></iframe> -->

<!-- <object width="100%" height="500px" data="https://drive.google.com/file/d/1Zdr8TbQE6sfnC8JQvKBkxoWaAPP8g-ou/preview"> -->

<iframe src="https://www.youtube.com/embed/xvew__NEOqs" frameborder="0" scrolling="no" onload="resizeIframe(this)" ></iframe>
