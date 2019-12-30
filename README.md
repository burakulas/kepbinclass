KEPBINCLASS is a Python script that is written for prediction of the morphological class of the Kepler binary star systems by recognizing their light curve images. Mainly, the Kepler binary star database [1] was used, however, the code can be used to classify the morphology of the binary stars from any other datasets based on light curve images.  

The model contains deep learning image recognition algorithm using neural networks to apply the multi-class classification to the light curve image data of the binary stars. The script predicts the classes and also plots the variation of “Accuracy” and “Loss Function” with the “Epoch” number. That is, the user can easily observe the quality of the model in terms of those quantities. 

 

Dependencies: 

Keras API [2] 

matplotlib library [3] 

numpy package [4] 

os module [5] 

tensorflow platform [6] 


 
Notes on Usage: 

. Change the variables “train_data_dir”, “validation_data_dir” and “pred_data_dir” based on your directory path scheme. 

. When predicting a single image alternate the prediction lines of the code according to the path and name of your test image to let the model outputs a prediction. 

. The default output will be in “class” format, however, the user may want to change it to “predict” or “proba” to observe the probabilities of different classes. 

. The output contain filename and the value of 0, 1 and 2 which correspond to contact, detached and semi-detached morphological classes respectively.  

. Different datasets probably need different trials of hyperparameters. Therefore, it is recommended to modify the parameters based on your light curve image dataset. 

. The script saves the model (mod_binclass.h5) on the working directory. 

. The script works on Python 3.x. Some modifications are needed to get the code runs in Python 2.x. It also uses TensorFlow 1.x. Some modifications are needed to get it run in TensorFlow 2.x 

. The deprecated warnings were disabled in the script. It is recommended to enable them when the code is used for development purposes. 


When used the script, you may want to give reference to its GitHub address: https://github.com/burakulas/kepbinclass

For comments and further questions: bulash@gmail.com
 

References: 

[1] www.keplerebs.villanova.edu/   

[2] www.keras.io 

[3] www.matplotlib.org 

[4] www.numpy.org 

[5] www.github.com/python/cpython/blob/3.8/Lib/os.py 

[6] www.tensorflow.org 