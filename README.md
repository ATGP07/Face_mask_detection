# Face_Mask_Detection

This project is implemented in Python using Keras, Tensorflow and OpenCV.<br>
[Here](https://drive.google.com/drive/u/1/folders/1NnPrkV6WzrvxHMCxUAJYkJVtDCPyPeLI) is the drive link of the project 

## About the Data

The dataset used to train the face-mask detection model taken from [here](https://github.com/prajnasb/observations/tree/master/experiements/data)

This dataset contains 1376 images belonging to the 2 classes.
The classes are:
- With mask(690)
- Without mask(686)<br>
You can have a glimpse look of data in Dataset folder.

## Workflow
### Data Preprocessing
For every image following process is applied.
  1. Resizing all images into a common size to fir to neural network.
  2. Applying normalization.
  3. Appending images pixels to X(feauture vector) and giving them labels(y).
  4. Shuffling X and Y.

### Transfer Learning
 **InceptionV3**<br>
     This model was applied with same weights as learned from imagenet dataset and in the last trainable layers were inserted.<br>
     
   **Training of model** <br>
   ![name-of-you-image](https://github.com/ATGP07/Face_mask_detection/blob/main/incep_accu.png?raw=true)
   ![name-of-you-image](https://github.com/ATGP07/Face_mask_detection/blob/main/incep_loss.png)
 Test Accuracy = 0.9320388436317444<br>
 Test Loss = 0.1794693022966385<br>
  
 ## Trying own model
 
   **Training of model** <br>
   ![name-of-you-image](https://github.com/ATGP07/Face_mask_detection/blob/main/model_accu.png?raw=true)
   ![name-of-you-image](https://github.com/ATGP07/Face_mask_detection/blob/main/model_loss.png)
 Test Accuracy = 0.9708737730979919<br>
 Test Loss = 0.07088583707809448<br>

# Notes
   1. Notebooks in the repository are made in google colab.<br>
   2.All the models with increasing validation accuracy are available in the folder.
