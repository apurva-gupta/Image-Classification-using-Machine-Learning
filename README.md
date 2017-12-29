# Image-Classification-using-Machine-Learning
Predicting orientation of images using 3 machine Learning Algorithms: K Neighbours algorithm, Adaboost algorithm and Neural Networks.

DATA
Dataset of images from Flickr photo sharing website.

Features
Rescaled each image to 8 * 8  pixels. This resulted in 8 * 8 * 3 = 192 dimensional feature vector. 3 is for three colors : red,green,blue.

Description of Files
1. train-data.txt : It has various images. Each is in the form of- photo_id correct_orientation r11 g11 b11 r12 g12 b12 ...
   ->photo-id is the photo ID for image
   ->correct_orientation is 0,90,180 or 270.
   ->r11 is red pixel value at 1,1 and so on.
2. test-data.txt :It has various images. Each is in the form of- photo_id correct_orientation r11 g11 b11 r12 g12 b12 ...
   ->photo-id is the photo ID for image 
   ->correct_orientation is 0,90,180 or 270.
   ->r11 is red pixel value at 1,1 and so on.
3. orient.py : It contain code written in python
4. Report.pdf : Contains project report
5. adaboost_model,nnet_model,nearest_model,best_model : It contains the model files for all algorithms

To Run Program:

For Training
./orient.py train train_file.txt model_file.txt [model]

For Testing
./orient.py test test_file.txt model_file.txt [model]

model can take in 4 options:
1. nearest : K nearest algorithm
2. adaboost : Adaboost algorithm
3. nnet : Neural Networks
4. best : Neural Networks(gives best accuracy)
