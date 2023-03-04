# Mood based Music Recommender System

# ABSTRACT :

1. Song recommendation existed for a long time, in the majority of the scenarios the recommendation is determined after learning the user preferences over a period of time, like looking at the past history of the song preferences.

2. "Songs on Mood" - an innovative app/website which uses the power of AI and machine learning algorithms to suggest songs based on your mood. With Moodify, we can discover new music that matches your current emotional state, whether we are feeling happy, sad, relaxed, or energized. The app's intuitive interface allows us to simply select our current mood, and Moodify will generate a custom playlist of songs tailored to our preferences.

3. But Moodify doesn't stop there - it also responds to voice commands, allowing us  to change songs, skip tracks, or pause playback without ever having to touch your device. With Moodify, you can enjoy your favorite music hands-free, and let the app do the work of finding the perfect song for our current mood.
With its advanced AI algorithms and vast music library, Moodify is the perfect tool for music lovers everywhere. Whether we are  looking to discover new music or just need a little help finding the right song for our current mood, Moodify has got us covered.

4. We are using  user input app which takes input from the user following that we have  used   Spotify Api  . For training purpose we are taking the spotify dataset from Kaggle ,and with the spotify Api the demand that user has made for specified singer is stored, later on we will use  the playlist of that singer  that is provided from the bot ,which later work upon the recognition of  mood dependent on the voice of the person and points to the playlist for the situation like what type of mood they have at that time. 

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



