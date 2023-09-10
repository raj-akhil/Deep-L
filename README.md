# Deep-L
There are mainly 3 projects submitted along with this file.
1. text prediction using LSTM
2. classification of 200 birds using inception v3 model
3.cyclegan model for generating fake combined images of human, cats, and dogs

location of files are given below.

.\210409183_cycleGan\210409183_cyclegan_model.h5    -cyclegan trained model
.\210409183_Birds_classification\210409183_birds_classification_model.h5  -trained model for birds classification
.\210409183_textclassification\210409183_textprediction_model.h5           - trained model for text prediction

.\210409183_cycleGan\210409183_cyclegan_notebook.ipynb                    - python code for cycleGAN model
.\210409183_Birds_classification\210409183_birds_classificaton_notebook.ipynb - python code for birds classification model
.\210409183_textclassification\210409183_text_prediction_notebook.ipynb        -python code for text prediction model

.\210409183_cycleGan\Generated_images                                     - folder containing generated images of cycleGAN model.



Instructions.
---------------
Text prediction
--------------
Before running the script pass the location of the .txt file to source_text parameter.
Run the code and finally in the testing area, input the sentence for which the model predicts the output.

cycleGAN model.
----------------
Image Translation using cycleGAN
----------------------------------
In this project, image translation is implemented using cycleGAN model. 
The location of the files can be found in this directories.

Before running the code the upload the zipped files cat_and_dog.zip and face_img.zip in google drive if colab is the selected platform. Assign the variables as follows:
zipped_cat_dog_dir ='Address of the cat and dog image file(zipped)'
zipped_human_dir='Address of the human images zipped file'
Then execute the script sequencely for getting the proper outputs.
script startING with ! should be run in terminal. The code first re arrange input file structure to the below form 
------data
-------cat_dog
----------test
----------train
-------human
----------test
----------train
The output folders are
-----saved_models(where the models are saved agfter each epochs)
-----generated_images(images created during training)
-----test_results(contains generated test data)

Birds classification
----------------------
Before running the code place the zipped birds data downloaded from the given link in the google drive.
pass the location of the file to data_source parameter.
model_output should be assigned with dircetory name where the checkpoint model has to be saved.
After running the first few script. new folder named data will be created with the following structure.
-----data
----------CUB_200_2011
-------------images_sorted
----------------test
------------------test images will be presnt in this folder under different sub directories
----------------train
------------------train images will be presnt in this folder under different sub directories


Additional information
-----------------------

1. cycleGAN model performance can be improved by running the model for some more epochs . the model given here is chosen subjectively from differents model produced after each epochs.
   The model generated in third epochs is camparitievly produced better results and as the epochs increases there is chance of overfitting that is the model generated images that is more      related to one class only.

2. Text prediction model and birds class can also be improved by increasing the epochs.
 
