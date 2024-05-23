---
title: "ME 5286 Robotics: CNN Assisted Tool Sorting"
excerpt: "Final lab for ME 5286: Robotics. A convolutional neural network assisted automated tool sorting process, implemented on a UR5 robotic arm.<br/><img src='/images/identified_bins.jpg' width='50%'>"
collection: portfolio
customdate: "Spring 2024"
---

<p class="page__date"><strong><i class="fa fa-fw fa-calendar" aria-hidden="true"></i> </strong>Spring 2024</p>

For our final lab in ME 5286: Robotics, we implemented an automated tool sorting procedure on a UR5 robotic arm. Tensorflow (keras) was used to design and train a convolutional neural network for identifying various types of tools. Corresponding bins for each tool were marked with april tags. A camera and Robotiq gripper were mounted on the end effector of the UR5. Starting with tools laid on a table, the UR5 used the pre-trained CNN to identify each tool. The gripper picked up each identified tool, and placed it in its corresponding bin based on the unique april tag for each bin. Our procedure was implemented using RoboDK and its corresponding Python libraries, in conjunction with the Tensorflow and OpenCV Python libraries. A demonstration of the sorting process can be found <a href="https://drive.google.com/file/d/1Zr_ByIFtwjkY2D6BDI7U6QIm2Pjh3QEK/view?usp=sharing" target="_blank">here</a>. Shown below are images from the UR5-mounted camera during the sorting process.

<img src="/images/identified_bins.jpg" width="50%">

<img src="/images/identified_Pliers.jpg" width="50%">
