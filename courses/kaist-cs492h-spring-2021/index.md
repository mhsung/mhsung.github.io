---
layout: page

title:  "CS492(H): Machine Learning for 3D Data"

class_info: <a href="http://mhsung.github.io/" target="_blank">Minhyuk Sung</a>, <a href="https://www.kaist.ac.kr/" target="_blank">KAIST</a>, Spring 2021

slug: index

date: 2021-01-15
---


## {{ page.title }}
{:.title}
#### {{ page.class_info }}
{:.title}

<br />
![]({{site.baseurl}}/{{page.path}}/../images/teaser.png)

### Description
3D Data (both 3D scans captured by depth sensors and 3D models created by designers) are widely used in many applications in computer vision, computer graphics, and robotic, such as autonomous driving, AI-assisted 3D object/scene design, augmented reality, and physical robot interaction. Along with the recent increasing demands on processing and analyzing such 3D data, there has been tremendous progress in developing novel technologies, especially based on deep learning. In this course, we will cover the recent advances in machine learning techniques for 3D data and also discuss the remaining challenges. Most of the course material will be less-than-5-year-old research papers in CVPR/ICCV/ECCV (Vision), SIGGRAPH/SIGGRAPH Asia (Graphics), and NeurIPS/ICML (Machine Learning). The course will be project-oriented (no exam, no paper-and-pencil homework, but easy programming assignment), and it will combine pedagogical lectures and seminar-style reading group presentations (followed by interactive discussions). Lectures will be held online via zoom.
<br />


### Prerequisites
This course is intended for undergraduate/master students who have a basic background in deep learning and experience with PyTorch. But there will be jump-start lectures/sessions for students who do not have any background in deep learning.
<br />


### Time & Location
Time: Tue/Thu 9:00am - 10:15am (KST)  
Location: Zoom
<br />

<span style="background-color:#FFC107">**Come join the course introduction session!**</span><br>
<!--
<a href="https://kaist.zoom.us/meeting/tZAocuyoqzkvEtzxtAaGKOjCGvAlnUZGxbAN/calendar/google/add" target="_blank">**Google Calendar Link**</a>
-->
Mar 02 (Tue) 9:00am - 10:15am (KST)<br>
<a href="https://kaist.zoom.us/j/84555052588?pwd=Q0xvSUczcU1aQmtNeVZyNFU3ZFJvQT09" target="_blank">https://kaist.zoom.us/j/84555052588?pwd=Q0xvSUczcU1aQmtNeVZyNFU3ZFJvQT09</a><br>
Passcode: cs492-3dml

**You'll need a KAIST email address to join.**


### Course Staff
**Instructor**: <a href="http://mhsung.github.io/" target="_blank">Minhyuk Sung</a>
- Email: <a href="mailto: {{site.email}}">{{site.email}}</a>
- Office hours: By appointment (See #announcements channel in slack.)
<br />

**TA**: Kisoo Kim
- Email: <a href="mailto: k014520@kaist.ac.kr">k014520@kaist.ac.kr</a>
<br />


### Links
- Course Website: <a href="http://mhsung.github.io/courses/kaist-cs492-3dml-2021-spring" target="_blank">http://mhsung.github.io/courses/kaist-cs492-3dml-2021-spring</a><br>
- Zoom Links & Submission & Grading: <a href="https://klms.kaist.ac.kr" target="_blank">KLMS</a><br>
- Discussion and Q&A: Slack (An invitation will be sent to the registered students by email.)<br>


### Grading 
- Project: 50%
    - <a href="{{site.baseurl}}/{{page.path}}/../project-pitch-video.html" target="_blank">Project Pitch Video</a>
    - <a href="{{site.baseurl}}/{{page.path}}/../project-submission-guidelines.html" target="_blank">Project Submission Guidelines</a>
    - <a href="{{site.baseurl}}/{{page.path}}/../poster-sessions.html" target="_blank">Poster Sessions</a>
- <a href="{{site.baseurl}}/{{page.path}}/../paper-review-presentation.html" target="_blank">Paper Review Presentation</a>: 30%
- Programming Assignments: 10%
    -  KCloud Setup Instruction: <a href="{{site.baseurl}}/{{page.path}}/../kcloud-setup.html" target="_blank">Link</a>
    - PointNet Code: <a href="{{site.baseurl}}/{{page.path}}/../pointnet-classification.html" target="_blank">Link</a>
- In-Class Participation: 10%
<br />


### Course Logistics
<a href="https://kaistackr-my.sharepoint.com/:b:/g/personal/mhsung_kaist_ac_kr/Ec0TrNbsVpRDuOaN6zmas1cB8C4ajsooup5WUWqfKNfwuQ?e=ai2KpX" target="_blank">Link</a> (Last Updated: Mar 01)


### Important Dates
(ALL ASSIGNMENTS ARE DUE 23:59 KST. **NO LATE DAYS!**)

- Project Sign-Up: <span style="background-color:#FFC107">~~Due Mar 11 (Thu)~~ Due Mar 05 (Fri)</span>
- 1st Programming Assignment: <span style="background-color:#FFC107">Due Mar 23 (Tue) </span>
- 2nd Programming Assignment: <span style="background-color:#FFC107">Due Apr 01 (Thu) </span>
- Project Proposal: <span style="background-color:#FFC107">Due Apr 01 (Thu) </span>
- Project Pitch Video: <span style="background-color:#FFC107">Due Apr 13 (Tue) </span>
- Presentation Preparation Check-In: <span style="background-color:#FFC107">Due two weeks before your presentation date
- Presentation Slides: <span style="background-color:#FFC107">Due 4 days before your presentation date
- Project Midterm Check-In: <span style="background-color:#FFC107">Due May 13 (Thu) </span>
- Project Report/Poster/Code: <span style="background-color:#FFC107">Due Jun 06 (Sun) </span>
- Project Review: <span style="background-color:#FFC107">Due Jun 17 (Thu) </span>
- Project Rebuttal & Final Decision: <span style="background-color:#FFC107">Due Jun 20 (Sun) </span>


### Schedule

<!---
    https://uxdesign.cc/dark-mode-ui-design-the-definitive-guide-part-1-color-53dcfaea5129
--->
<details>
  <summary><i class="fa fa-arrow-circle-o-right" aria-hidden="true"></i> <b>Click for details.</b></summary>

<span style="color:#00897B;font-weight:bold">Green</span>: Lectures<br>
<span style="color:#C62828;font-weight:bold">Red</span>: Student presentations

<style>
table th:first-of-type {
    width: 4%;
}
table th:nth-of-type(2) {
    width: 8%;
}
table th:nth-of-type(3) {
    width: 40%;
}
table th:nth-of-type(4) {
    width: 8%;
}
table th:nth-of-type(5) {
    width: 40%;
}
table th {
  text-align: center;
  vertical-align: center;
}
table td {
  text-align: center;
  vertical-align: center;
}
</style>


<table style="width:100%;">
  <tr style="background-color:#F5F5F5">
    <th>Week</th>
    <th>Tue</th>
    <th>Topic</th>
    <th>Thu</th>
    <th>Topic</th>
  </tr>

  <!-- Week 01 -->
  <tr><td>01</td>
  <td>Mar 02</td><td>
    <span style="color:#00897B;font-weight:bold">Course Introduction</span>
  </td>
  <td>Mar 04</td><td>
    <span style="color:#00897B;font-weight:bold">Deep Learning Jump-Start Session 1</span><br>
    Material: <a href="http://cs231n.stanford.edu/" target="_blank">Stanford CS231n</a> 
  </td>
  </tr>

  <!-- Week 02 -->
  <tr><td>02</td>
  <td>Mar 09</td><td>
    <span style="color:#00897B;font-weight:bold">Deep Learning Jump-Start Session 2</span><br>
    Material: <a href="http://cs231n.stanford.edu/" target="_blank">Stanford CS231n</a>
  </td>
  <td>Mar 11</td><td>
    <span style="color:#00897B;font-weight:bold">Neural Networks for Point Cloud Data</span><br>
    <a href="https://arxiv.org/abs/1612.00593" target="_blank">PointNet (CVPR 2017)</a><br>
    <a href="https://arxiv.org/abs/1706.02413" target="_blank">PointNet++ (NeurIPS 2017)</a><br>
    <a href="https://arxiv.org/abs/1612.00603" target="_blank">Point Set Generation (CVPR 2017)</a><br>
    <span style="background-color:#FFC107">Project Sign-Up Due Date</span>
  </td>
  </tr>

  <!-- Week 03 -->
  <tr><td>03</td>
  <td>Mar 16</td><td>
    <span style="color:#00897B;font-weight:bold">PyTorch / PointNet Session</span>
  </td>
  <td>Mar 18</td><td>
    <span style="color:#00897B;font-weight:bold">Examples of Supervised / <br>Weakly-Supervised Learning</span><br>
    <a href="https://arxiv.org/abs/1811.08988" target="_blank">SPFN (CVPR 2019)</a><br>
    <a href="https://arxiv.org/abs/1805.09957" target="_blank">Deep Functional Dictionaries (NeurIPS 2018)</a>
  </td>
  </tr>

  <!-- Week 04 -->
  <tr><td>04</td>
  <td>Mar 23</td><td>
    <span style="color:#00897B;font-weight:bold">Spectral Geometry Processing</span><br>
    Material: <a href="http://school.geometryprocessing.org/summerschool-2016/summerschool/talks/course6.pdf" target="_blank">SGP Summer School 2016 (Laplace-Beltrami)</a><br>
    <a href="https://hal.inria.fr/inria-00331894/document" target="_blank">Spectral Geometry Proceesing (Eurographics 2008)</a><br>
    <span style="background-color:#FFC107">1st Programming Assignment Due Date </span>
  </td>
  <td>Mar 25</td><td>
    <span style="color:#00897B;font-weight:bold">Functional Map / Deep Spectral Processing</span><br>
    <a href="http://www.lix.polytechnique.fr/~maks/fmaps_SIG17_course/index.html">Tutorial (SIGGRAPH 2017)</a><br>
    <a href="http://www.lix.polytechnique.fr/~maks/papers/obsbg_fmaps.pdf" target="_blank">Functional Maps (SIGGRAPH 2012)</a><br>
    <a href="https://arxiv.org/abs/1704.08686" target="_blank">Deep Functional Maps (ICCV 2017)</a><br>
    <a href="https://arxiv.org/abs/1612.00606" target="_blank">SyncSpecCNN (CVPR 2017)</a>
  </td>
  </tr>

  <!-- Week 05 -->
  <tr><td>05</td>
  <td>Mar 30</td><td>
    <span style="color:#00897B;font-weight:bold">Guest Lecture 1</span><br>
    <b><a href="https://cseweb.ucsd.edu/~haosu/" target="_blank">Hao Su (UCSD)</a></b><br>
    <a href="{{site.baseurl}}/{{page.path}}/../guest-lecture-hao-su" target="_blank">Title: Compositional Generalizability in Geometry, Physics, and Policy Learning</a>
  </td>
  <td>Apr 01</td><td>
    <span style="color:#C62828;font-weight:bold">Neural Networks for Volumetric Data</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1712.01537" target="_blank">O-CNN (SIGGRAPH 2017)</a></span><br>
    <b>Presenter: Byeoli Choi</b><br>
    <a href="https://arxiv.org/abs/1611.05009" target="_blank">OctNet (CVPR 2017)</a><br>
    <a href="https://arxiv.org/abs/1809.07917" target="_blank">Adaptive O-CNN (SIGGRAPH Asia 2018)</a><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/1706.01307" target="_blank">SparseConvNet (arXiv)</a></span><br>
    <b>Presenter: Kyounga Woo</b><br>
    <a href="https://arxiv.org/abs/1711.10275" target="_blank">SparseConvNet (CVPR 2018)</a><br>
    <span style="background-color:#FFC107">2nd Programming Assignment Due Date </span><br>
    <span style="background-color:#FFC107">Project Proposal Due Date </span>
  </td>
  </tr>

  <!-- Week 06 -->
  <tr><td>06</td>
  <td>Apr 06</td><td>
    <span style="color:#00897B;font-weight:bold">Guest Lecture 2</span><br>
    <b><a href="http://www.vovakim.com/" target="_blank">Vladimir G. Kim (Adobe Research)</a></b><br>
    <a href="{{site.baseurl}}/{{page.path}}/../guest-lecture-vova-kim" target="_blank">Title: Neural Mesh Processing</a>
  </td>
  <td>Apr 08</td><td>
    <span style="color:#C62828;font-weight:bold">Neural Networks for Implicit Functions</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1901.05103" target="_blank">DeepSDF (CVPR 2019)</a></span><br>
    <b>Presenter: Wonkwang Lee</b><br>
    <a href="https://arxiv.org/abs/1812.02822" target="_blank">IM-NET (CVPR 2019)</a><br>
    <a href="https://arxiv.org/abs/1812.03828" target="_blank">Occupancy Networks (CVPR 2019)</a><br>
    <a href="https://arxiv.org/abs/1908.06277" target="_blank">Deep Meta Functionals (ICCV 2019)</a><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/2006.09661" target="_blank">Sirens (NeurIPS 2020)</a></span><br>
    <b>Presenter: Andréas Meuleman</b><br>
  </td>
  </tr>

  <!-- Week 07 -->
  <tr><td>07</td>
  <td>Apr 13</td><td>
    <span style="color:#C62828;font-weight:bold">Neural Networks for Meshes</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1809.05910" target="_blank">MeshCNN (SIGGRAPH 2019)</a></span><br>
    <b>Presenter: Dahyun Kang</b><br>
    <a href="https://arxiv.org/abs/1811.11424" target="_blank">MeshNet (AAAI 2019)</a><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/2004.01002" target="_blank">DualConvMesh-Net (CVPR 2020)</a></span><br>
    <b>Presenter: Juil Koo</b><br>
    <span style="background-color:#FFC107">Project Pitch Video Due Date</span>
  </td>
  <td>Apr 15</td><td>
    <span style="color:#C62828;font-weight:bold">Project Pitches</span>
  </td>
  </tr>

  <!-- Week 08 -->
  <tr><td>08</td>
  <td>Apr 20</td><td>
    Midterm Week (No Class)
  </td>
  <td>Apr 22</td><td>
    Midterm Week (No Class)
  </td>
  </tr>

  <!-- Week 09 -->
  <tr><td>09</td>
  <td>Apr 27</td><td>
    <span style="color:#C62828;font-weight:bold">Supervised 2D-to-3D</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1804.01654" target="_blank">Pixel2Mesh (ECCV 2018)</a></span><br>
    <b>Presenter: Chaeyeon Chung</b><br>
    <a href="https://arxiv.org/abs/1908.01491" target="_blank">Pixel2Mesh++ (ICCV 2019)</a><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/1905.05172" target="_blank">PIFu (CVPR 2019)</a></span><br>
    <b>Presenter: Whie Jung</b><br>
    <a href="https://arxiv.org/abs/2004.00452" target="_blank">PIFuHD (CVPR 2020)</a>
  </td>
  <td>Apr 29</td><td>
    <span style="color:#C62828;font-weight:bold">Unsupervised 2D-to-3D</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1904.01786" target="_blank">Soft Rasterizer (ICCV 2019)</a></span><br>
    <b>Presenter: Hakyung Kim</b><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/1911.11130" target="_blank">Unsup3D (CVPR 2020)</a></span><br>
    <b>Presenter: Minsoo Lee</b><br>
    <!--
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1901.02970" target="_blank">NOCS (CVPR 2019)</a></span><br>
    <a href="https://arxiv.org/abs/1907.01085" target="_blank">X-NOCS (NeurIPS 2019)</a><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/2102.09105" target="_blank">DeepMetaHandles (CVPR 2021)</a></span><br>
    <b>Presenter: Doyeon Kim</b><br>
    -->
  </td>
  </tr>

  <!-- Week 10 -->
  <tr><td>10</td>
  <td>May 04</td><td>
    <span style="color:#C62828;font-weight:bold">Shape Parsing / Abstraction</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1612.00404" target="_blank">Volumetric Primitives (CVPR 2017)</a></span><br>
    <b>Presenter: Taegyu Jin</b><br>
    <a href="https://arxiv.org/abs/1904.09970" target="_blank">Superquadrics Revisited (CVPR 2019)</a><br>
    <a href="https://isunchy.github.io/projects/cuboid_abstraction.html" target="_blank">Hierarchical Cuboid Abstractions (SIGGRAPH Asia 2019)</a><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/1911.06971" target="_blank">BSP-Net (CVPR 2020)</a></span><br>
    <b>Presenter: Jihyun Lee (Auditor)</b><br>
    <a href="https://arxiv.org/abs/1909.05736" target="_blank">CvxNet (CVPR 2020)</a><br>
  </td>
  <td>May 06</td><td>
    <span style="color:#C62828;font-weight:bold">Shape Alignment</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1905.03304" target="_blank">Deep Closest Point (ICCV 2019)</a></span><br>
    <b>Presenter: Shinjeong Kim</b><br>
    <a href="https://arxiv.org/abs/1905.04153" target="_blank">DeepICP (ICCV 2019)</a><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/2004.11540" target="_blank">Deep Global Registration (CVPR 2020)</a></span><br>
    <b>Presenter: Jaesung Choe</b><br>
  </td>
  </tr>

  <!-- Week 11 -->
  <tr><td>11</td>
  <td>May 11</td><td>
    <span style="color:#C62828;font-weight:bold">Learning 3D Structure 1</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1705.02090" target="_blank">GRASS (SIGGRAPH 2017)</a></span><br>
    <b>Presenter: Hankyu Jang</b><br>
    <a href="https://arxiv.org/abs/1804.05469" target="_blank">Im2Struct (CVPR 2018)</a><br>
    <a href="https://arxiv.org/abs/1809.05398" target="_blank">SCORES (SIGGRAPH Asia 2018)</a><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/1908.00575" target="_blank">StructureNet (SIGGRAPH Asia 2019)</a></span><br>
    <!-- <b>Presenter: Ramazan Abdikarimuly</b><br> -->
    <b>Presenter: Inhee Lee (Auditor)</b><br>
    <a href="https://arxiv.org/abs/1812.02713" target="_blank">PartNet (CVPR 2019)</a><br>
    <a href="https://arxiv.org/abs/1911.11098" target="_blank">StructEdit (CVPR 2020)</a>
  </td>
  <td>May 13</td><td>
    <span style="color:#C62828;font-weight:bold">Learning 3D Structure 2</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1712.08290" target="_blank">CSGNet (CVPR 2018)</a></span><br>
    <b>Presenter: Chanhyeok Park</b><br>
    <a href="https://arxiv.org/abs/2006.09102" target="_blank">UCSG-Net (NeurIPS 2020)</a><br>
    <!--
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/1908.04520" target="_blank">SDM-NET (SIGGRAPH Asia 2019)</a></span><br>
    -->
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/2011.00844" target="_blank">GAN2Shape (ICLR 2021)</a></span><br>
    <b>Presenter: Hangil Park</b><br>
    <span style="background-color:#FFC107">Project Midterm Check-In Due Date</span>
  </td>
  </tr>

  <!-- Week 12 -->
  <tr><td>12</td>
  <td>May 18</td><td>
    <span style="color:#C62828;font-weight:bold">Detection/Semantic Segmentation in Scenes</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1904.09664" target="_blank">Deep Hough Voting (ICCV 2019)</a></span><br>
    <b>Presenter: Jeonghyun Kim</b><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/1904.08755" target="_blank">MinkowskiNet (ICCV 2019)</a></span><br>
    <b>Presenter: Seungwoo Yoo</b><br>
  </td>
  <td>May 20</td><td>
    <span style="color:#C62828;font-weight:bold">Instance Segmentation in Scenes</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1812.07003" target="_blank">3D-SIS (CVPR 2019)</a></span><br>
    <b>Presenter: Chungsu Jang</b><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/2004.01658" target="_blank">PointGroup (CVPR 2020)</a></span><br>
    <b>Presenter: Junho Lee</b><br>
    <a href="https://arxiv.org/abs/2003.06537" target="_blank">OccuSeg (CVPR 2020)</a><br>
  </td>
  </tr>

  <!-- Week 13 -->
  <tr><td>13</td>
  <td>May 25</td><td>
    <span style="color:#C62828;font-weight:bold">3D Generative Models</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1707.02392" target="_blank">Point Cloud GAN (ICML 2018)</a></span><br>
    <b>Presenter: Yunpyo An</b><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/1709.04307" target="_blank">MeshVAE (CVPR 2018)</a></span><br>
    <b>Presenter: Hojun Cho</b><br>
    <a href="http://www.geometrylearning.com/ausdt/" target="_blank">Automatic Unpaired Shape Deformation Transfer (SIGGRAPH Asia 2018)</a><br>
  </td>
  <td>May 27</td><td>
    <span style="color:#C62828;font-weight:bold">Neural Rendering</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1812.01024" target="_blank">DeepVoxels (CVPR 2019)</a></span><br>
    <b>Presenter: Soomin Park</b><br>
    <a href="https://arxiv.org/abs/2004.03805" target="_blank">State of the Art on Neural Rendering (EG 2020)</a><br>
    <a href="https://www.neuralrender.com/" target="_blank">Tutorial (CVPR 2020)</a><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/2003.08934" target="_blank">NeRF (ECCV 2020)</a></span><br>
    <b>Presenter: In-young Cho</b><br>
    <a href="https://arxiv.org/abs/2012.03918" target="_blank">NeRD (arXiv)</a>
  </td>
  </tr>

  <!-- Week 14 -->
  <tr><td>14</td>
  <td>Jun 01</td><td>
    <span style="color:#C62828;font-weight:bold">3D Shape Flow</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/1806.07366" target="_blank">NeuralODE (NeurIPS 2019)</a></span><br>
    <b>Presenter: Hyunsoo Kim</b><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/1906.12320" target="_blank">PointFlow (ICCV 2019)</a></span><br>
    <b>Presenter: Mustafa Berk Yaldiz</b><br>
    <a href="https://arxiv.org/abs/2007.10973" target="_blank">Neural Mesh Flow (NeurIPS 2020)</a><br>
    <a href="https://arxiv.org/abs/2006.07982" target="_blank">ShapeFlow (NeurIPS 2020)</a><br>
  </td>
  <td>Jun 03</td><td>
    <span style="color:#C62828;font-weight:bold">3D Transformers</span><br>
    <span style="background-color:#BCCCDC">Paper 1: <a href="https://arxiv.org/abs/2012.09688" target="_blank">PCT: Point Cloud Transformer (arXiv)</a></span><br>
    <b>Presenter: Seongjoo Moon</b><br>
    <span style="background-color:#BCCCDC">Paper 2: <a href="https://arxiv.org/abs/2012.09164" target="_blank">Point Transformer (arXiv)</a></span><br>
    <b>Presenter: Shyngys Aitkazinov</b><br>
  </td>
  </tr>

  <!-- Week 15 -->
  <tr><td>15</td>
  <td>Jun 08</td><td>
    <span style="color:#C62828;font-weight:bold">Project Presentations 1</span><br>
    <span style="background-color:#FFC107">Project Report/Poster/Code Due Jun 06 (Sun) </span>
  </td>
  <td>Jun 10</td><td>
    <span style="color:#C62828;font-weight:bold">Project Presentations 2</span><br>
    <span style="background-color:#FFC107">Project Review Due Jun 13 (Sun) </span>
  </td>
  </tr>

  <!-- Week 16 -->
  <tr><td>16</td>
  <td>Jun 15</td><td>
    Final Week (No Class)
  </td>
  <td>Jun 17</td><td>
    Final Week (No Class)
  </td>
  </tr>
</table>
</details>


### Useful Links
This webpage kindly provides a comprehensive summary of resources regarding 3D machine learning:<br>
<a href="https://github.com/timzhang642/3D-Machine-Learning" target="_blank">https://github.com/timzhang642/3D-Machine-Learning</a>
<br />


### Acknowledgements
Most of the lectures will be based on the materials in the following courses:<br>
<a href="http://graphics.stanford.edu/courses/cs468-17-spring/">Stanford CS468: Machine Learning for 3D Data (Spring 2017)</a><br>
<a href="https://cse291-i.github.io/WI18/index.html">UCSD CSE291-I00: Machine Learning for 3D Data (Winter 2018)</a><br>
<a href="http://3ddl.stanford.edu/">A Tutorial on 3D Deep Learning (CVPR 2017)</a>
<br />

<br />
