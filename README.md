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
Implementation of Gaussian Elimination Algorithm for Solving Linear Systems[span_0](start_span)[span_0](end_span). The requirement is to write a generalized Python program to solve systems of linear equations without hardcoding for specific matrix dimensions[span_1](start_span)[span_1](end_span).

**Files Used:**
- `gaussian_elimination.py`: The Python source code containing the elimination and back substitution functions.

**Mathematical Concepts:**
The function accepts a coefficient matrix and a right-hand-side vector to form an augmented matrix[span_2](start_span)[span_2](end_span). It converts the augmented matrix into upper triangular form using elementary row operations[span_3](start_span)[span_3](end_span). Partial pivoting is implemented to handle zero or small pivot elements[span_4](start_span)[span_4](end_span). A separate function is used for back substitution to compute the final variable values[span_5](start_span)[span_5](end_span). 

**Steps to Execute:**
1. Install the required numerical dependency: `pip install numpy`
2. Run the program from the command line: `python gaussian_elimination.py`

**Expected Output:**
Upon execution, the terminal displays the input coefficient matrix, RHS vector, and the initial augmented matrix[span_6](start_span)[span_6](end_span). It prints the matrix after forward elimination and the final solution obtained using back substitution[span_7](start_span)[span_7](end_span). The program verifies the obtained solution by substituting it into the original equations and includes error handling for singular matrices, zero pivots, and invalid matrix dimensions[span_8](start_span)[span_8](end_span).

---

## Project 2: Data Augmentation using Affine Transformation

**Objective:**
Implementation of Data Augmentation using Affine Transformation on images[span_9](start_span)[span_9](end_span).

**Files Used:**
- `affine_augmentation.py`: The Python source code containing functions for geometric image manipulation.

**Mathematical Concepts:**
The program represents image coordinates using homogeneous coordinates[span_10](start_span)[span_10](end_span). It constructs specific affine transformation matrices for translation, rotation, scaling, and shearing[span_11](start_span)[span_11](end_span). Applying these transformations improves the diversity of training data for machine learning and computer vision applications by generating new geometric variations of the original data[span_12](start_span)[span_12](end_span).

**Steps to Execute:**
1. Install the required libraries for matrix operations, computer vision, and plotting: `pip install numpy opencv-python matplotlib`
2. Run the program from the command line: `python affine_augmentation.py`

**Expected Output:**
The script allows the user to specify transformation parameters such as translation directions, rotation angles, and scaling/shearing factors[span_13](start_span)[span_13](end_span). It displays the original image along with the translated, rotated, scaled, and sheared images for comparison[span_14](start_span)[span_14](end_span). The generated augmented images are saved as separate image files, and the output includes the affine transformation matrix used for each respective transformation[span_15](start_span)[span_15](end_span).

## Conclusion
Both source code files are generalized and modular rather than written only for a given example[span_16](start_span)[span_16](end_span). The testing phases confirmed that the mathematical implementations handle the required edge cases (like singular matrices in linear systems and coordinate mapping in image processing).
