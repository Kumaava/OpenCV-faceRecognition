# OpenCV-faceRecognition

To make a face recognition program, first we need to train the recognizer with dataset of previously captured faces along with its ID, for example we have two person then first person will have ID 1 and 2nd person will have ID 2,  so that all the images of person one in the dataset will have ID 1 and all the images of the 2nd person in the dataset will have ID 2, then we will use those dataset images to train the recognizer to predict the 1 of an newly presented face from the live video frame
So lets break the program into 3 major part:

### Dataset Creator
Lets create the dataset generator script, open your python IDLE and create a new file and save it in your project folder and make sure you also have the haarcascade_frontalface_default.xml file in the same folderJust like in the previous post we will need to do the following first:
cv2 library (opencv library),
create a video capture object,
cascadeClassifier object.

### Add a dataSet Folder that will take the images from the Webcam
<img width="931" alt="dataset_file added" src="https://cloud.githubusercontent.com/assets/11708565/26136915/7466e1a2-3adc-11e7-8e71-4281b6b829af.png">

### dataSet folder after the images are added
<img width="1280" alt="dataset" src="https://cloud.githubusercontent.com/assets/11708565/26136752/6d0d8e3e-3adb-11e7-846c-3f9c5893d554.png">

### Trainer
we define a function getImages&Labels
So now inside this function we are going to do the following

Load the training images from dataset folder
capture the faces and Id from the training images
Put them In a List of Ids and FaceSamples  and return it
<img width="1098" alt="yml file" src="https://cloud.githubusercontent.com/assets/11708565/26137061/4c3dcf1e-3add-11e7-91f8-acd6cfec26b8.png">

### Detector
Loading Recognizer
Lets start the main loop and do the following basic steps
Starts capturing frames from the camera object
Convert it to Gray Scale
Detect and extract faces from the images
Use the recognizer to recognize the Id of the user
Put predicted Id/Name and Rectangle on detected face
<img width="1280" alt="final_detector" src="https://cloud.githubusercontent.com/assets/11708565/26137163/0745d8a6-3ade-11e7-8cc7-a5fc45072d42.png">


# @subpart of a project

