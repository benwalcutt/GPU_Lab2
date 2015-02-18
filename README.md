# GPU_Lab2
Matrix multiplication with CUDA

University of Arkansas
Department of Computer Scie
nce and Computer Engineering
CSCE4643 – GPU Programming
Lab 2: Basic Matrix Multiplication
Due Date: February 12 (Thursday) 12:00PM
1. Objective
The purpose of this lab is to implement a basic dense matrix multiplication routine.
2. Procedure
Step 1:
Download the lab 2 materials from moodle to
your local folder at any machine in JBHT 237.
Unzip it.
unzip lab2-sgemm.zip
Step 2:
Edit the file
lab2/main.cu
to implement the following where indicated:
a)
Allocate device memory
b)
Copy host memory to device
c)
Copy results from device to host
d)
Free device memory
Step 3:
Edit the file
lab2/kernel.cu
to initialize the thread block
and kernel grid dimensions and
invoke the CUDA kernel, and to implement the matrix multiplication kernel code.
Step 4:
Compile and test your code.
cd lab2
make
./sgemm # Uses the default matrix sizes
./sgemm <m> # Uses square m x m matrices
./sgemm <m> <k> <n> # Uses (m x k) and (k x n) input matrices
It is a good idea to test and de
bug initially with small input dime
nsions. Your code is expected
to work for varying input dimensions – which
may or may not be divi
sible by your block size –
so don’t forget to pay attention to boundary conditions. 
