## OpenCV-faceRecognition

To make a face recognition program, first we need to train the recognizer with dataset of previously captured faces along with its ID, for example we have two person then first person will have ID 1 and 2nd person will have ID 2,  so that all the images of person one in the dataset will have ID 1 and all the images of the 2nd person in the dataset will have ID 2, then we will use those dataset images to train the recognizer to predict the 1 of an newly presented face from the live video frame
So lets break the program into 3 major part:

### Dataset Creator
Lets create the dataset generator script, open your python IDLE and create a new file and save it in your project folder and make sure you also have the haarcascade_frontalface_default.xml file in the same folderJust like in the previous post we will need to do the following first:
cv2 library (opencv library)
create a video capture object
cascadeClassifier object
<img width="1280" alt="dataset" src="https://cloud.githubusercontent.com/assets/11708565/26136752/6d0d8e3e-3adb-11e7-846c-3f9c5893d554.png">

### Trainer
### Detector
