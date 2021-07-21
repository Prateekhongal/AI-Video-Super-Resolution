# AI-Video-Super-Resolution-Using-Dynamic-Upsampling-Filters-Without-Explicit-Motion-Compensation
Video super-resolution (VSR) has become even more important recently to provide high resolution (HR) contents for ultra high definition displays. While many deep learning based VSR methods have been proposed, most of them rely heavily on the accuracy of motion estimation and compensation.  This is a novel end-to-end deep neural network that generates dynamic upsampling filters and a residual image, which are computed depending on the local spatio-temporal neighborhood of each pixel to avoid explicit motion compensation. 

# Environments
TensorFlow:1.8.0

Pillow:5.3.0

Numpy:1.15.4

# Data folder
Low-resolution:

./data/x_train_data4x/: The scaled frames by 4x which will be used in train stage

./data/x_valid_data4x/: The scaled frames by 4x which will be used in valid stage

./data/x_test_data4x/: The scaled frames by 4x which will be used in test stage

Original-resolution:

./data/y_train_data/: The HR frames which will be used in train stage coresponde to ./data/x_train_data4x/

./data/y_valid_data/: The HR frames which will be used in valid stage coresponde to ./data/x_valid_data4x/

Another folders

Results of output:

./result_test/: The output frames after VSR-DUF processing

./checkpoint/: save ckpt

./model/: save pb model

./logs/: save graph and variables

# Run
Before run train and test, your should prepare your datasets and check your environments if you want to run it successfully.

Training: train.py

Testing: test.py

