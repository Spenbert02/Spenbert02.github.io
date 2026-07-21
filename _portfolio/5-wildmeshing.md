---
title: "Wildmeshing Toolkit"
excerpt: "<img src='/images/jaw_pic.png' width='50%'>"
header:
  teaser: "jaw_pic.png"
collection: portfolio
order: 1
codeurl: "https://github.com/wildmeshing/wildmeshing-toolkit/tree/main"
references:
  - 'Zint, D., Chen, Z., Zhu, Y., Zorin, D., Schneider, T., Panozzo, D. "Topological Offsets." arXiv:2407.07725 (2024). <a href="https://doi.org/10.48550/arXiv.2407.07725" target="_blank">https://doi.org/10.48550/arXiv.2407.07725</a>'
---

The Wildmeshing Toolkit is a declarative framework for mesh generation, mesh adaptation, and geometric modeling algorithms that edit mesh connectivity. Rather than hand-coding each mesh editing algorithm from scratch, the toolkit lets users specify per-element invariants, operation scheduling, and attribute transfer rules at a high level; the toolkit itself handles enforcing those invariants, transferring attributes, rolling back failed operations, and parallelizing execution across shared-memory architectures. Many widely used mesh editing algorithms (edge collapse, edge split, edge swap, vertex smoothing, and more) can be compactly expressed in this abstraction, making implementations simpler, safer, and easier to customize.

I implemented the <code>topological_offset</code> and <code>manifold_extraction</code> components of this repository. The <code>topological_offset</code> module computes manifold, watertight, self-intersection-free offset surfaces that are topologically equivalent to an infinitesimally close offset of the input, following the approach in Topological Offsets <span class="citation">{% include cite.html n=1 %}</span>. The <code>manifold_extraction</code> module extracts a manifold surface mesh from the (possibly non-manifold) output of the offsetting procedure, resolving non-manifold vertices and edges so the result can be used directly in downstream geometry processing applications.

<img src="/images/jaw_pic.png" width="75%">

{% include references.html %}
