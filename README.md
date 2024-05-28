# Catch-a-Glimpse



### To run this project 

### Step 1
Open the Catch a Glimpse.ipynb on Google collab

### Step2
Run all the cells in the  0. Setup Paths.

In 1. Download TF Models Pretrained Models from Tensorflow Model Zoo and Install TFOD sections

run all cells till the cell with the following code:
   ```sh
   !pip uninstall protobuf matplotlib -y
   !pip install protobuf==3.20.3 matplotlib==3.7.1
   
   ```
after running the above given piece of code COLLAB will prompt you to restart the session
so restart the session

### Step3
After restarting the session you have to run all the cells from start again till this cell
   ```sh
   !pip uninstall protobuf matplotlib -y
   !pip install protobuf==3.20.3 matplotlib==3.7.1
   
   ```

Note: you don't have to run this cell this time

### Step4:
Before running verification scripts cell go to: 
   ```sh
  Tensorflow/models/research/object_detection/packages/tf2/setup.py
   
   ```

Comment out keras and limit the versions of tf-models-official to 

```sh
'tf-models-official >= 2.5.1, <2.16.0',
```
this procedure solves the error of  "AttributeError: module 'keras._tf_keras.keras.layers' has no attribute 'experimental'".

### Step5

1.Go to:
   ```sh
  Tensorflow/workspace
   ```
create a folder "Detection_Images"


2.Go to:
   ```sh
  Tensorflow/workspace/images
   ```
create a folder "test" inside images and upload all the contents of "test images" given on the Catch a Glimpse repository.

3.Go to:
   ```sh
  Tensorflow/workspace/models/my_ssd_mobnet
   ```
Upload all the contents of the "checkpoints and config files" folder given on the Catch a Glimpse repository.

### Step5:
Now run the verification scripts cell and you can go ahead and run all other cells.

Note: If you ever stuck anywhere just restart the session and you are good to go.
 
