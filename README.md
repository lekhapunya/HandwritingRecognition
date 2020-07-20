# HandwritingRecognition

## Project Description
###### Purpose: I want to use this model to be able to transcribe a full page of student notes on paper into a computer document. 
###### The model is able to take in an image of a word in my own personal handwriting, and output the model's prediction of the word. 
###### I followed the implementation specified in this article: https://towardsdatascience.com/build-a-handwritten-text-recognition-system-using-tensorflow-2326a3487cd5
###### Currently, the model is able to take in an image of one word with no outside spaces. The contrast, word line width, and size of the picture is formatted within Model.py to match the training set.
###### The model is trained on the IAM dataset.

## Software 
###### Mac OS - Version: 10.15.2
###### Python - Version: 3.7.6
###### Anaconda with Python 3.7 - Version: 4.8.3
###### TensorFlow - Version: 1.13.1 *** I received problems while using the latest version of tensorflow 2+. I found that this version worked well with the code implementation ***
###### OpenCV - Version: 4.3.0

## FAQ (Errors I Encountered)
###### 1. If you are using Homebrew to download OpenCV or TensorFlow and are running into many problems during the process, I recommend using Anaconda to install these two packages instead. It was a much simpler process and was successful for me. 
###### 2. If the command:
###### /tconda activate (env)
###### is not working for you when you are trying to install tensorflow in a separate environment, you can use pip to install tensorflow in the base environment and the implementation will still work
###### 3. If you get a ModuleNotFoundError or ImportError such as:
###### /tModuleNotFoundError: No module named 'keras_preprocessing'
###### it is likely that the package is not installed. Use conda or pip commands to install the package.
###### 4. If you encounter the error:
###### /tAttributeError: module 'tensorflow.python.pywrap_tensorflow' has no attribute 'TFE_DEVICE_PLACEMENT_EXPLICIT'
###### you may have missing dependencies. I fixed this error by installing the missing dependencies that the Spyder application pointed out for me. Whenever I opened the application, a pop-up appeared that highlighted the dependencies I needed. 
###### 5. If you encounter the error:
###### /tImportError: cannot import name 'descriptor' from 'google.protobuf' (unknown location)
###### your tensorflow and protobuf versions may not be compatible. You should uninstall both tensorflow and protobuf from anaconda. Then, reinstall tensorflow version 1.13-1.15. Next, reinstall protobuf. 
