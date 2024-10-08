---
title: "An Orientation Field-Based Toolpath Generation Algorithm for Nonplanar, Fiber-Oriented 3D Bioprinted Cardiac Constructs"
collection: publications
permalink: /publication/2024-04-30-undergrad-thesis
excerpt: 'My undergraduate honors thesis, proposing a toolpath generation algorithm for fiber-oriented 3D bioprinting. Unanimously graded <i>summa cum laude</i>.'
date: 2024-04-30
venue: 'University of Minnesota'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://drive.google.com/file/d/1cS0lh9MMRoNei8rpnAYBNYr-8fQZtgO7/view?usp=sharing'
citation: 'Bertram, S E. (2024). An orientation field-based toolpath generation algorithm for fiber-oriented 3D bioprinted cardiac constructs [Unpublished undergraduate honors thesis]. University of Minnesota.'
---

Fiber architecture is key to the function of many biological tissues. This is particularly true of the myocardium, which has a highly complex and nonplanar fiber structure that is central to the function of the heart. Diffusion tensor magnetic resonance imaging (DTMRI) is a clinical imaging modality capable of extracting the complex fiber geometry of the heart; however, cardiac biomanufacturing processes have yet to take advantage of the directional information DTMRI provides. Previous studies attempting to 3D bioprint functional cardiac ventricle constructs have been limited by planar, layer-by-layer approaches - based on biologically uninformed 3D printing processes - that do not fully capture the directional complexity of the myocardium. We propose a DTMRI-informed toolpath generation algorithm that outputs a sequence of 3D printable, non-interfering toolpaths, such that the resulting print-line architecture of the organoid matches the fiber architecture of the native myocardium. To validate the algorithm, fiber paths were extracted from a DTMRI scan of an ex-vivo, fixed human heart. A representative subset of those fiber paths was selected via a novel thinning procedure. Paths in the representative subset were ordered for printing so as to eliminate interference during material deposition. The resulting path sequence was translated to G-code and used to fabricate an acellular, silicone model of the isolated left ventricle. Computational volumetric coverage analysis was also conducted on the output toolpaths. Our novel toolpath generation procedure marks a paradigm shift in 3D printing toolpath generation, enabling the fabrication of fiber-oriented biological constructs that accurately recapitulate fiber structure and function of the native tissue.
