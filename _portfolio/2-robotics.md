---
title: "<i>ME 5286 Robotics:</i> CNN-based robotic tool sorting"
excerpt: "Final lab for <i>ME 5286 Robotics</i>. A convolutional neural network-based tool sorting procedure, implemented on a UR5 robotic arm.<br/><img src='/images/identified_bins.jpg' width='50%'>"
collection: portfolio
customdate: "Spring 2024"
---

<p class="page__date"><strong><i class="fa fa-fw fa-calendar" aria-hidden="true"></i> </strong>Spring 2024</p>

For our final lab in <i>ME 5286 Robotics</i>, we implemented an automated tool sorting procedure on a UR5 robotic arm. Tensorflow (keras) was used to design and train a convolutional neural network for identifying different types of tools. Corresponding bins for each tool were marked with unique april tags. A camera and Robotiq gripper were mounted on the end effector of the UR5. Starting with tools laid on a table, the UR5 used the pre-trained CNN to identify each tool. The gripper picked up each identified tool and placed it in its corresponding bin, referring to the unique april tag identifying the proper bin. Our procedure was implemented using RoboDK and its corresponding Python libraries, in conjunction with the Tensorflow and OpenCV Python libraries. A demonstration of the sorting process is shown below, along with still images from the UR5-mounted camera during the sorting process.

<iframe width="100%" height="500px" src="https://drive.google.com/file/d/1exLWsvlgdfYCr6B9uaJRwn-kgL4yVPbg/preview"></iframe>

<img src="/images/identified_bins.jpg" width="50%">

<img src="/images/identified_Pliers.jpg" width="50%">
