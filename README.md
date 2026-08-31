# MATHEMATICAL-FOUNDATION-FOR-MACHINE-LEARNING---ASSIGNMENT
This is a Repository for all assignemnts of MFML 3RD SEM
# B.Tech Class Projects (Module 1)

**Student Details:**
Name: Rajdeep Sarkar
Registration Number: 202500412
Roll Number: 16
Branch: B.Tech
Department: CSE (DS), Dept of AI&DS

This document outlines the execution steps, concepts, and requirements for the Python implementations based on the assignment details provided in the Class_Projects.docx file.

## Project 1: Gaussian Elimination Algorithm

**Objective:**
Implementation of the Gaussian Elimination Algorithm for solving linear systems. The requirement is to write a generalized Python program to solve systems of linear equations without hardcoding for specific matrix dimensions.

**Files Used:**
- `gaussian_elimination.py`: The Python source code containing the elimination and back substitution functions.

**Mathematical Concepts:**
The function accepts a coefficient matrix and a right-hand-side vector to form an augmented matrix. It converts the augmented matrix into upper triangular form using elementary row operations. Partial pivoting is implemented to handle zero or small pivot elements. A separate function is used for back substitution to compute the final variable values.

**Steps to Execute:**
1. Install the required numerical dependency: `pip install numpy`
2. Run the program from the command line: `python gaussian_elimination.py`

**Expected Output:**
Upon execution, the terminal displays the input coefficient matrix, RHS vector, and the initial augmented matrix. It prints the matrix after forward elimination and the final solution obtained using back substitution. The program verifies the obtained solution by substituting it into the original equations and includes error handling for singular matrices, zero pivots, and invalid matrix dimensions.

---

## Project 2: Data Augmentation using Affine Transformation

**Objective:**
Implementation of Data Augmentation using Affine Transformation on images.

**Files Used:**
- `affine_augmentation.py`: The Python source code containing functions for geometric image manipulation.

**Mathematical Concepts:**
The program represents image coordinates using homogeneous coordinates. It constructs specific affine transformation matrices for translation, rotation, scaling, and shearing. Applying these transformations improves the diversity of training data for machine learning and computer vision applications by generating new geometric variations of the original data.

**Steps to Execute:**
1. Install the required libraries for matrix operations, computer vision, and plotting: `pip install numpy opencv-python matplotlib`
2. Run the program from the command line: `python affine_augmentation.py`

**Expected Output:**
The script allows the user to specify transformation parameters such as translation directions, rotation angles, and scaling/shearing factors. It displays the original image along with the translated, rotated, scaled, and sheared images for comparison. The generated augmented images are saved as separate image files, and the output includes the affine transformation matrix used for each respective transformation.

## Conclusion
Both source code files are generalized and modular rather than written only for a given example. The testing phases confirmed that the mathematical implementations handle the required edge cases.
