---
title: "<i>CSCI 4511W Intro. to Artificial Intelligence:</i> Final Project"
excerpt: "Final project for CSCI 4511W: Intro. to Artificial Intelligence, titled <i>Sequencing Tissue-Imitating 3D Printer Toolpaths for Time-Optimal Printing Under Printability Constraints</i>. <br/><img src='/images/sample_tiling_44.jpg' width='50%'>"
collection: portfolio
customdate: "Fall 2022"
---

<p class="page__date"><strong><i class="fa fa-fw fa-calendar" aria-hidden="true"></i> </strong>Fall 2022</p>

This was my final project for <i>CSCI 4511W Intro. to Artificial Intelligence</i>. To explore the fundamental principles behind toolpath ordering for non-planar 3D printing, the problem was reduced to two dimensions. In the image shown below, the y-axis lies perpendicular to the build plate, and the x-axis lies parallel to the build plate. A set of 2D toolpaths was created throughout a grid, with each section assigned an orientation angle according to a random walk, simulating slight directional variance common in biological tissues. The toolpaths were ordered using a hill-climbing search algorithm to minimize inter-toolpath distance. Along each step of the search, available actions were restricted to "printable" toolpaths, which would not result in interference during printing. A final toolpath sequence is shown below, with extruding paths shown in red and non-extruding paths shown in blue. All code was implemented in Python using the <a href="https://github.com/aimacode/aima-python" target="_blank">aima-python</a> package. The source code for this project can be found <a href="https://github.com/Spenbert02/CSCI-4511W-Final-Project" target="_blank">here</a>.

<img src="/images/sample_tiling_44.jpg" width="50%">
