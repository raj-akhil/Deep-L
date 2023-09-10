Image Translation using cycleGAN
----------------------------------
In this project, image translation is implemented using cycleGAN model. 
The location of the files can be found in this directories.

210409183_cyclegan_notebook             : python notebook containing the code.
210409183_cyclegan_model.h5             : Saved model

Before running the code the upload the zipped files cat_and_dog.zip and face_img.zip in google drive if colab is the selected platform. Assign the variables as follows:
zipped_cat_dog_dir ='Address of the cat and dog image file(zipped)'
zipped_human_dir='Address of the human images zipped file'
Then execute the script sequencely for getting the proper outputs.
script startING with ! should be run in terminal. The code first re arrange input file structure to the below form ----data
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