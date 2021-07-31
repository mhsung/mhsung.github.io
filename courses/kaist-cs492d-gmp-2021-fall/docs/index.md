# CS492(D): Geometry Modeling and Processing

## Description
3D content creation is a crucial part of many industries such as graphics, AR/VR, CAD/CAM, and digital fabrication, which tasks typically include designing and creating virtual objects/scenes or reconstructing a real environment. Processing scanned 3D data is also an important problem in many applications as 3D scanning technology is being widely applied, for example, in autonomous driving, robot navigation, and 3D object replication.

In this course, we discuss fundamental mathematical methods for geometric 3D modeling and geometric data processing, which can be used (not only in graphics-related fields but) in many other areas in science and engineering. Topics to be covered include the followings:

- Homogeneous coordinates and geometric transformations
- Quaternions and their use in modeling 3-d rotations and rigid motions
- Parametric and implicit representations for curves
- Algebraic classification of the parametric polynomial curves of low degree
- Polar forms and the de Casteljau's subdivision algorithm
- The Bézier representation and the Bernstein basis
- Splines and continuity constraints
- B-Splines and the de Boor's algorithm
- Rational curves
- Parametric polynomial surfaces and NURBS
- Subdivision curves and surfaces
- Triangle meshes for surface representation and reconstruction
- The quad-edge data structure for manifold subdivision
- Volumetric representations and conversion algorithms
- Surface reconstruction from scattered points
- Scan alignment and shape matching
- Mesh simplification and fairing
- Mesh parametrization and other geometry processing algorithms


## Prerequisites
The following courses are not required but recommended:  
- [CS380: Introduction to Computer Graphics](http://vclab.kaist.ac.kr/cs380/index.html)  
- MAS109: Introduction to Linear Algebra  
Students are also expected to have good programming skills in C/C++.


## Time & Location
**Time**: Mon/Wed 10:30am - 11:45am (KST)  
**Location**: Zoom

## Course Staff
**Instructor**: [Minhyuk Sung](https://mhsung.github.io/)

- Email: [mhsung@kaist.ac.kr](mailto:mhsung@kaist.ac.kr)  
- Office hours: TBD.

## Links
Course Website: [https://mhsung.github.io/kaist-cs492d-gmp-2021-fall/](https://mhsung.github.io/kaist-cs492d-gmp-2021-fall/)  
Zoom Links, Submission, and Grading: KLMS  
Discussion and Q&A: Slack (An invitation will be sent to the registered students by email.)  

## Grading
- Homeworks (Including Programming Assignments): 50%
- Midterm Exam: 20%
- Final Exam: 20%
- Participation: 10%

## Schedule
(Subject to Change) 



| Week | Date  | Topic                                                                                                       | Note                           |
| ---- | ----- | ----------------------------------------------------------------------------------------------------------- | ------------------------------ | 
| 1    | 8/30  | Introduction                                                                                                |                                |
| 1    | 9/1   | Homogeneous Coordinates; The Projective Plane and 3-Space                                                   |                                |
| 2    | 9/6   | Oriented Projective Geometry; Euclidean, Affine and Projective Transformations; Matrix Representations      |                                |
| 2    | 9/8   | Rotations and Quaternions                                                                                   | Homework 1 out                 |
| 3    | 9/13  | Shape Modeling: Parametric and Implicit Representations; Classification of Parametric Cubics                |                                |
| 3    | 9/15  | Polar Forms of Polynomials                                                                                  |                                |
| 4    | 9/20  | (Chuseok Holidays)                                                                                          |                                |
| 4    | 9/22  | (Chuseok Holidays)                                                                                          |                                |
| 5    | 9/27  | Derivatives and Polar Forms; Continuity Constraints                                                         |                                |
| 5    | 9/29  | Splines and B-Splines                                                                                       | Homework 1 due, Homework 2 out |
| 6    | 10/4  | Rational Curves                                                                                             |                                |
| 6    | 10/6  | Subdivision Curves                                                                                          |                                |
| 7    | 10/11 | Tensor-Product and Total Degree Parametric Surfaces                                                         |                                |
| 7    | 10/13 | Midterm Summary                                                                                             | Homework 2 due, Homework 3 out |
| 8    | 10/18 | Midterm Exam                                                                                                |                                |
| 8    | 10/20 | Midterm Exam                                                                                                |                                |
| 9    | 10/25 | Triangle Meshes and their Representation; the Quad-Edge Data Structure                                      |                                |
| 9    | 10/27 | Introduction to Shape Acquisition and Geometry Processing                                                   |                                |
| 10   | 11/1  | Representations of 3D Geometry: Voxel-Grids, Point Clouds, Meshes and Other Boundary Models, Solid Models.  |                                |
| 10   | 11/3  | Scan Alignment and Registration; Surface Matching                                                           | Homework 3 due, Homework 4 out |
| 11   | 11/8  | Mesh Simplification                                                                                         |                                |
| 11   | 11/10 | Laplace-Beltrami and other operators on meshes.                                                             |                                |
| 12   | 11/15 | Break (CVPR)                                                                                                |                                |
| 12   | 11/17 | Break (CVPR)                                                                                                | Homework 4 due, Homework 5 out |
| 13   | 11/22 | Global and local shape descriptors; intrinsic descriptors, heat and wave kernel signatures.                 |                                |
| 13   | 11/24 | Functional spaces and functional maps, variations; map visualization.                                       |                                |
| 14   | 11/29 | Mesh Smoothing, Remeshing, Parametrization                                                                  |                                |
| 14   | 12/1  | Geodesic Distances                                                                                          |                                |
| 15   | 12/6  | Guest Lecture                                                                                               |                                |
| 15   | 12/8  | Course Summary                                                                                              |                                |
| 16   | 12/13 | Final Exam
| 16   | 12/15 | Final Exam


## Acknowledgements
Most of the lectures will be based on the materials in the following courses:  
[Stanford CS348A: Geometric Modeling / Processing](https://graphics.stanford.edu/courses/cs348a-21-winter/)  
[Stanford CS233: Geometric and Topological Data Analysis](http://graphics.stanford.edu/courses/cs233-20-spring/)
