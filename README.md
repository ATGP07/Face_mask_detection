# Face_mask_detection

This project is implemented in Python using Keras, Tensorflow and OpenCV.

## About the Data

The dataset used to train the face-mask detection model taken from [here](https://github.com/prajnasb/observations/tree/master/experiements/data)

This dataset contains 853 images belonging to the 2 classes. The classes are:
The classes are:
- With mask
- Without mask

## Workflow
### Data Preprocessing
For every image following process is applied.
  1. Resizing all images into a common size to fir to neural network.
  2. Applying normalization.
  3. Appending images pixels to X(feauture vector) and giving them labels(y).
  4. Shuffling X and Y.

### Transfer Learning
 **InceptionV3**<br>
     This model was applied with same wieghts as learned from imagenet dataset. Last 3 layers of inceptionV3 were removed and trainable  layers were inserted.<br>
     
   **Training of model** <br>
 Test Accuracy = 0.9320388436317444<br>
 Test Loss = 0.1794693022966385<br>
  
 ## Trying own model
 
   **Training of model** <br>
 Test Accuracy = 0.9708737730979919<br>
 Test Loss = 0.07088583707809448<br>
