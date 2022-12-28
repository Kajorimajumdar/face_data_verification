# Facial recognition System using simple KNN algorithm.

## Dataset used
face_data_collect.py file is used to capture face data which acts as the dataset for this project.

## Flow of the program is as follows:

For face_data_collect.py 
- Data collection through video capturing using opencv and frontal_face_haarcascade.xml
- Storing the data with name of the person in disk.

For face_recognition.py

- Read a video stream using opencv
- extract faces out of it using haarcascade
- load the training data(numpy arrays of all the persons)
#### x - values are stored in numpy array
#### y - values we need to assign to each person
- Use knn to find the prediction of face(int)
- Map the predicted id to name of the user
- Display the prediction on the screen - bounding box and name