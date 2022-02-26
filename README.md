# MCA PROJECT :- Traffic-Signs-Recognition
MCA Project of Driver Drowsiness Detection By RollNo 134- Zaid Sayyed and 02 - Aaquibe Shaikh


You must have heard about the self-driving cars in which the passenger can fully depend on the car for traveling. But to achieve level 5 autonomous, it is necessary for vehicles to understand and follow all traffic rules.

Traffic Signs Recognition – About the Python Project
In this Python project example, we will build a deep neural network model that can classify traffic signs present in the image into different categories. With this model, we are able to read and understand traffic signs which are a very important task for all autonomous vehicles.

# Prerequisites
This project requires prior knowledge of Keras, Matplotlib, Scikit-learn, Pandas, PIL and image classification.
To install the necessary packages used for this Python data science project, enter the below command in your terminal:
pip install tensorflow keras sklearn matplotlib pandas pil

# Steps to Build the Python Project
The dataset contains more than 50,000 images of different traffic signs. It is further classified into 43 different classes. The dataset is quite varying, some of the classes have many images while some classes have few images. The size of the dataset is around 300 MB. The dataset has a train folder which contains images inside each class and a test folder which we will use for testing our model.

Our ‘train’ folder contains 43 folders each representing a different class. The range of the folder is from 0 to 42. With the help of the OS module, we iterate over all the classes and append images and their respective labels in the data and labels list.

Our approach to building this traffic sign classification model is discussed in four steps:
Explore the dataset
Build a CNN model
Train and validate the model
Test the model with test datase

Step 1: Explore the dataset
Step 2: Build a CNN model
Steps 3: Train and validate the model
Step 4: Test our model with test dataset

# Traffic Signs Classifier GUI
Now we are going to build a graphical user interface for our traffic signs classifier with Tkinter. Tkinter is a GUI toolkit in the standard python library. Make a new file in the project folder and copy the below code. Save it as gui.py and you can run the code by typing python gui.py in the command line.

In this file, we have first loaded the trained model ‘traffic_classifier.h5’ using Keras. And then we build the GUI for uploading the image and a button is used to classify which calls the classify() function. The classify() function is converting the image into the dimension of shape (1, 30, 30, 3). This is because to predict the traffic sign we have to provide the same dimension we have used when building the model. Then we predict the class, the model.predict_classes(image) returns us a number between (0-42) which represents the class it belongs to. We use the dictionary to get the information about the class.

# Input output screen
input screen
![image](https://user-images.githubusercontent.com/79075376/155858519-7a8be523-ebd5-44c4-855a-ff1cb9b73390.png)
output screen
![image](https://user-images.githubusercontent.com/79075376/155858576-1517b964-005b-4395-9933-75858fa93482.png)
input screen
![image](https://user-images.githubusercontent.com/79075376/155858619-3cee25f4-f938-4804-b661-ab8ba895a017.png)
outputscreen
![image](https://user-images.githubusercontent.com/79075376/155858627-34bb25be-9c6e-445b-ab1a-fe891eaf49e4.png)
input screen
![image](https://user-images.githubusercontent.com/79075376/155858646-f495c7a7-5119-4ebb-953f-85410aa05600.png)
output screen
![image](https://user-images.githubusercontent.com/79075376/155858653-3013c117-053d-47c6-b25e-f80203031727.png)

# Summary
we have successfully classified the traffic signs classifier with 95% accuracy and also visualized how our accuracy and loss changes with time, which is pretty good from a simple CNN model.
