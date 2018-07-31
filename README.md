# Personal-Data-Identification
CNN to segregate credit card data from non personal image. The New Model contains jupyter notebook file of the trained model using the dataset uploaded in the box. Predict contains the prediction code for inference.

1. Installation and prerequisite : Anaconda with Python 3.6, Tensorflow 1.9, Keras (Deep learning library). You might need to install matplotlib and numpy separately using anaconda. You will need jupyter notebook to run the training program which comes as a part of anaconda.

2.   Instruction on how to run your training program : 
Refer to New Model.ipynb
1) Make a folder structure as follows:
Split the available data in 80 - training 20 - validation ratio and place in the below folders
a)   dataset/train/non personal/Put_All_Training_Non_Personal_Images.jpg
b) dataset/train/personal/Put_All_Training_Personal_Images.jpg
c) dataset/validation/non personal/Put_All_Non_Validation_Personal_Images.jpg
d) dataset/validation/personal/Put_All_Personal_Validation_Images.jpg

2) Replace the paths in cell 22 of my github notebook with the above created folder paths
3) Please follow the comments in the notebook for rest of the configurations and run the cells 22 to 26 as it is in case there is no tuning in model required.
4) The new_weight.h5 in cell 26 and model.json in cell 14 represent the path where you want to save the model  and the weight. If not changed these will get saved in the folder where anaconda is installed.

3)   Instruction on how to run the inference : 
Refer to  Predict.ipynb 

1) Convert cell 115 to a python program. 
2) Replace model.json with the path where you model is saved from the previous steps.
3)  Replace new_weight.h5 with the path where your weights are saved from the previous steps.
4) Replace C:/Users/IBM_ADMIN/Downloads/samplecard/ssn_images/only_cards_images with your mixed data folder path. This lists all the images in that folder.
5) Replace C:/Users/IBM_ADMIN/Downloads/samplecard/ssn_images/images/ with your mixed data folder path. This iteratively runs through every image listed in the previous step. 
6)   Replace C:/Users/IBM_ADMIN/Desktop/credit card/ with the folder where you want to place personal data
7)  Replace C:/Users/IBM_ADMIN/Desktop/non pi/ with the folder where you want to place non personal data
8) Run the python script/program
