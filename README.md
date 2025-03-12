# Automatic Alignment of Point Clouds in Rectilinear Construction Projects

# Introduction
This study focused on the automatic alignment and detection of points belonging to rectilinear objects on construction projects. Rectilinear building construction represents the most common type of floor plan due to the dimensioning flexibility offered by rectangular packing. Developing a generic solution for the automatic processing of point clouds in rectilinear construction projects, hence, provides considerable opportunities to enhance efficiency by acquiring frequent as-built analytics for decision-support in many construction projects. As a part of this study, two new algorithms were developed to solve two classes of complexities in point cloud processing, namely, level I complexity with negligible construction errors; and level I complexity with only assembly errors, but negligible dimensioning errors (e.g., quality-controlled elements). The boundary of problems covered by the three difference classes of complexity are further explained in the following Stacey complexity matrix.

![Picture 1](https://github.com/user-attachments/assets/88e72b29-4d5e-4b63-b6c5-1f6035e840e0)

# Algorithm 1: Alignment of Point Cloud to Digital Model in Rectilinear Construction
First, the principal axes were detected using the solution to a newly formulated quadratic unconstraint binary optimization (QUBO) problem. Once the rotation was recovered, the translation parameters in the direction of each of the principal axes was estimated by finding the solution to a non-linear max-min problem, solved through available global artificial intelligence (AI)-based optimization methods. This algorithm was developed as a part of a stand-alone MATLAB App with various opportunities for the user to change differen parameters, such as initial transformation, point measurement error, method for predicting normal vector of neighborhood of each point and AI-based optimization method used to recover the translation. The following ~1.5-minute video provides a demonstration of the App.

https://github.com/user-attachments/assets/e7f934d5-5a18-492d-bbab-500640ecc36f

# Algorithm 2: Iterative Plane-Correspondence Registration
for the cases with reliable planar segmentation, the plane correspondence matching was performed by finding the solution to a linear assignment problem, which can be solved using integer linear programming, or the Hungarian method (e.g., the Munkres method). This algorithm was developed as a part of a stand-alone MATLAB App with various opportunities for the user to change differen parameters, such as point measurement error, point cloud density, thresholds for coverage, plane distance, normal angle, and registration convergence, and BIM element ID. The final outcome of the algorithm provides the user to toggle between colour-coded visual descriptive analytics, including detected elements, coverage ratios, accuracy of final registration, and construction error. The following ~1.2-minute video provides a demonstration of the App.

https://github.com/user-attachments/assets/4256e23c-1359-48f0-860c-cb3074fb2e88

# Implementation and Dependencies
The code was implemented in MATLAB. As such, in order to utilize the code, the user must install an up-to-date Matlab software with the following Toolboxes:

1- Parallel Computing Toolbox

2- Optimization Toolbox

3- MATLAB Support Package for Quantum Computing

4- Curve Fitting Toolbox

5- Statistics and Machine Learning Toolbox

# Explanation on Code and Provided Files
As part of this Repository, two folders are provided:

1- Algorithm 1 for Level I Complexity Stand-alone MATLAB App.

2- Algorithm 2 for Level II Complexity Stand-alone MATLAB App.

# Citation
The study is under review at the journal of Remote Sensing, where the mathematical formulations are explained in more detail. You may cite the study using the following information:

Maalek, R. 2025. MATLAB App for the Automatic Alignment of Point Clouds and Digital Models in Rectilinear Building Construction, Remote Sensing, under review.

# Acknowledgements
The author wishes to acknowledge the generous endowment provided by GOLDBECK GmbH to the Karlsruhe Institute of Technology (KIT) for the establishment of the Professorship in Digital Engineering and Construction at the Institute of Technology and Management in Construction (TMB).
