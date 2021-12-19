# CS_74020_final_project

This repository contains the code for the final project for Graduate Center CS 74020 Fall 2021 Final Project


Authors:
- Weicong Feng
- Tugce Ozdemir
- Gulya Radjapova
- Nancy Sea

Instructions: 1. Clone the repository
2. Copy the contents of the _final_project_ to Google Drive (to utilize the Google Collab environment) to the root folder of the Google Drive. All of the project documents should exist in _final_project_ folder in the root of your drive.
3. Open MatterportTrainMammals_final.ipynb in Google Collab
4. Follow instructions in the notebook and run each portion.
5. In the Load MaskRCNN and dependencies section, ensure that the ROOT_DIR variable set tp '/content/drive/MyDrive/final_project/' represents the location where you copied the repository.
6. Continue running the notebook.
7. In the Training section, ensure that the location of the original initialization via COCO is '/content/drive/MyDrive/final_project/mask_rcnn_coco.h5'  in your drive.
8. model.train() function allows you to train the model based on the configurations of interest. The resulting experiment results will be saved in the temp_log folder. Note that training on large amount of epochs and large size of training dataset will take quite a bit of time to train. To test that training is working, set epochs in model.train() to a small number.
9. Copy the contents of the temp_log folder to the experiment folde in Google driver. For example:
 * !cp /content/temp_log/mammal20211219T1808/mask_rcnn_mammal_0010.h5 "/content/drive/MyDrive/final_project/Experimentation/12192021/" 
* !cp /content/temp_log/mammal20211219T1808/events.out.tfevents.1639937351.999d6dda7416 "/content/drive/MyDrive/final_project/Experimentation/12192021/"
The timestamps associated with the model training will be different when you run this. Change mammal20211219T1808 to relevant folder.
10. To replicate the loss analysis in the Visualizing & Understanding Losses section, ensure that the location of the experimentation folder is in /content/drive/MyDrive/final_project/Experimentation/. This folder will contain all the results of experiments we have conducted. We use tensor board to visualize losses.
