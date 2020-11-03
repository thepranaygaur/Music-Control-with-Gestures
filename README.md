# Music-Control-using-Gestures
## Description
This repository contains the Python code to develop your own hand gesture recognition system. 

## Packages Used
- OpenCV 
- Keras
- PyGame
- NumPy

## Files
Here's a list of files in the directory:
- `src/demo.py`: Contains all the functions to start and run the app
- `src/music`: Contains the song that will be played during 'gesture mode'
- `Presentation (Gesture Jester)`: Contains the slide deck for my project presentation

## Usage
In order to start the application, do the following:
1) Clone the repo
2) Navigate into the folder, set up a virtual environment and activate it
3) Once you've activated the virtual environment, install the requirements
```
pip install -r requirements.txt
```
4) Download `my_model_weights.h5` from [this Kaggle link](https://www.kaggle.com/dylanmendonca/training-hand-gesture-model) and store the file in the src folder. The model was trained on data 
that I collected through the 'data collection mode' of the app. If you find that my trained model doesn't work well for you or you feel like you need more gestures,
you can train the model using images of your own hand. Please refer to the Kaggle link for more information on building or training the model.
5) Navigate into the src folder and run the following command:
```
python demo.py
```
6) Some of the features have been included in the snippets in the Application Interface section

## Gesture Recognition Model
The model was built to recognize 7 different hand gestures and the absence of a hand. The encoding of the gestures is included in the demo file under the variable `GESTURE_ENCODINGS`. 
List of gestures recognized (in the order of the encodings):
1. `Fist`</br>
![Fist](imagesandgifs/fist.png)
2. `Five`</br>
![Five](imagesandgifs/five.png)
3. `None`</br>
![None](imagesandgifs/none.png)
4. `Okay`</br>
![Okay](imagesandgifs/okay.png)
5. `Peace`</br>
![Peace](imagesandgifs/peace.png)
6. `Rad`</br>
![Rad](imagesandgifs/rad.png)
7. `Straight`</br>
![Straight](imagesandgifs/straight.png)
8. `Thumbs`</br>
![Thumbs](imagesandgifs/thumbs.png)

## Music Player Model (Gesture Mode)
Currently the system is set up to recognize 6 gestures:
1. `Rad`: Loads the song (I Saw Her Standing There)
2. `Fist`: Plays/unpauses the song
3. `Five`: Pauses the song
4. `Okay`: Increases the volume. Hold the pose to continue increasing the volume
5. `Peace`: Decreases the volume. Hold the pose to continue decreasing the volume
6. `Straight`: Stops the song
7. `None`: Does nothing


