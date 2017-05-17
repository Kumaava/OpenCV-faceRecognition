## OpenCV-faceRecognition

To make a face recognition program, first we need to train the recognizer with dataset of previously captured faces along with its ID, for example we have two person then first person will have ID 1 and 2nd person will have ID 2,  so that all the images of person one in the dataset will have ID 1 and all the images of the 2nd person in the dataset will have ID 2, then we will use those dataset images to train the recognizer to predict the 1 of an newly presented face from the live video frame
So lets break the program into 3 major part:
### Dataset Creator
### Trainer
### Detector
