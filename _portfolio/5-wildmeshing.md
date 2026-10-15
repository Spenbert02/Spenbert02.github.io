---
title: "SimWild"
excerpt: "<img src='/images/jaw_pic.png' width='50%'>"
header:
  teaser: "jaw_pic.png"
collection: portfolio
order: 1
codeurl: "https://github.com/wildmeshing/wildmeshing-toolkit/tree/main"
references:
  - 'Zint, D., Chen, Z., Zhu, Y., Zorin, D., Schneider, T., Panozzo, D. "Topological Offsets." arXiv:2407.07725 (2024). <a href="https://doi.org/10.48550/arXiv.2407.07725" target="_blank">https://doi.org/10.48550/arXiv.2407.07725</a>'
---

SimWild, part of the open-source Wildmeshing Toolkit, turns imperfect geometry (3D scans, CAD models, medical images) into meshes ready for physical simulation.

Its offset component grows a layer of uniform thickness around the input that never opens holes or merges separate parts, building on Topological Offsets <span class="citation">{% include cite.html n=1 %}</span> and the TetWild meshing algorithm. At its core are a volumetric energy formulation, closed-form integration, and Newton-based mesh optimization, in 2D and 3D. A manuscript is in preparation.

<img src="/images/jaw_pic.png" width="75%">

{% include references.html %}
