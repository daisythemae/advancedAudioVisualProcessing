# advancedAudioVisualProcessing
 - Theremin Camera
 - My Theremin camera takes pixel data from a camera/webcam source and uses it to generates frequencies for synthesis whilst drawing pixel data as well. The program has two outputs for the visuals; the first is the webcam output. The second performs analysis on the pixel information for the camera and creates a new output. In a for loop it checks for the colour of the pixel, as well as values for the lightness and saturation. It draws a white pixel if it fufills certain criteria, and a black if not. The criteria is set by the user in a gui control interface, using the ofxGui library. The colour can be selected to track red, green or blue pixels. The threshold for the lightness and saturation can also be adjusted, meaning the app can be calibrated live for different lightings. This output is then analysised to check for brightness of the pixels; if the pixel is white within a certain area of the screen, the y value is changed. This value then determines the frequency for the audio output. The sound is created using frequency modulation synthesis to recreate the sound of the theremin. This is combined with an ADSR envelope to give the sound it's shape. The interface can show either of the pixel outputs, both or neither. By showing both, a comparison can be made between the image taken by the camera and the analysised and redrawn pixel data.
 - Video demonstration : https://youtu.be/640dNJkDrAo
 

- Guide for compiling.
- These examples use the following libraries: ofxGui and ofxMaxim
- For the fftVideo example, the audio must be downloaded from the Github repository and placed in the data folder, as the .wav file is too large to upload with the project.
