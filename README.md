# Mood based Music Recommender System

# DESCRIPTION :


1. We first process the image of the user taken as an input with the help of a python library for Computer Vision called 'OpenCV'. This captured image is then made available for the CNN in combination with DNN to make a prediction whether the current mood of the user is 'Happy' or 'Sad'.
2. The second part is the usage of Unsupervised Machine Learning techniques for clustering songs.The songs are clustered as either of the two classes-'VERY ENTERTAINING'(class 0) and 'RELAXED'(class 1) using the popular K-means algorithm. Then the recommendation is made in order of the current popularity of the respective songs.
3. We have an unique story in the way we recommend the songs for each mood, for example when other sites recommend sad songs when a person is sad or feeling bad, we recommend users with songs which will cheer them up('VERY ENTERTAINING') and 'RELAXING' songs when they are 'HAPPY'.
4. The code to train the neural network can be found in the 'Emotion_detector_version2' iPython notebook. If anyone wants to modify the network to suit their particular needs or feel it is necessary to tweak the network they can do so by making changes to the code present there. The model created is saved as 'final_model.h5'


# DATA :
 1. The file contains more than 160,000 songs collected from Spotify Web API, and also you can find data grouped by artist, year, or genre in the data section.
 2. It has features like acousticness, energy, loudness and danceability which make the clustering algorithm work more effectively.
 
 
# LIBRARIES USED :
  1. OpenCV.
  2. Tensorflow and Keras.
  3. Sklearn.
  4. LightGBM.
  5. Spotipy.
  5. Tkinter.
  6. Pillow.


# HOW TO USE :

   1. This application can be used by executing the run.py file which then opens up a GUI asking the user to enter the name of the artist.
   2. This will then collect required albums from the API and then will open up your WebCam .
   3.  Just click 'q' button on the keyboard to stop capturing the image and the GUI will lead you through. 
   4. Clicking on print button will make the recommendations ready for you. 



