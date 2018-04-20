# Face-Recognition-using-Principal Component Analysis

# Goals
Familiarizing with AT&T face database
Face Recognition using Principal Component Analysis (PCA)

# AT and T Face Database
1. The AT&T database is freely downloadable and contains a set of 400 face images (http://www.cl.cam.ac.uk/research/dtg/attarchive/facedatabase.html)

2. There are ten different images of each of 40 distinct subjects 

3. For some subjects, the images were taken at different times, varying the lighting, facial expressions (open / closed eyes, smiling / not smiling) and facial details (glasses / no glasses)

# Face Recognition Procedure
1. Prepared a training set of face images.
2. Each image is treated as one vector, simply by concatenating the rows of pixels in the original images.
3. All the images of the training set are stored in a single matrix where each column of the matrix is an image.
4. Subtracted the mean and computed the covariance matrix. 
5. Calculated the eigenvectors and eigenvalues of the covariance matrix.
6. Chose the principal components (Sort the eigenvalues in descending order and arrange eigenvectors accordingly). 
7. Used Euclidean distance as distance metrics.

# Modes
Mode 1: For each subject, use the first five images (1.pgm to 5.pgm) for training the subspace. Use the files 6.pgm to 10.pgm for the performance evaluation. 

Mode 2: Use the first twenty five subjects (1.pgm to 10.pgm) for training the subspace. Use the rest 15 subjects for the performance evaluation. 

# Performance Evaluation
False Rejection Rate (FRR) is the proportion of images belonging to the same subjects that are classified as impostors. 
False Accept Rate (FAR) is the proportion of images belonging to different subjects that are classified as genuine. 



