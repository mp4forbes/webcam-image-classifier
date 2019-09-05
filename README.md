# webcam-image-classifier
This Project is the first homeork assignment for implementing an image classifier.
1) The Index.html outlines a basic window that contains the video screen and 4 buttons one for each image you wish to train for. 
2) The index.js is the Java Script that makes calls to the tensor flow libraries that classifies the images from the webcam built into your computer.  Here is a brief description of the functions in the index.js file:
2.1) the setupWebcam() function used to configur
2.2) App() function which you added before, you can remove the prediction 
   through the image and instead create an infinite loop which makes predictions 
   through the webcam element.

If you experience a problem accessing your Webcam from a MacOS do the following:
   Type chrome://flags/ in the URL bar to various experimental features
   Then enable the following options (use the search feature to identify):
     Override software rendering list
     WebGL Draft Extensions
     WebGL 2.0

Training your App:
1) load the app into your web-browser, you will be projpted to allow the webcam
2) Hold up an image (in my case an orange)  before the web cam and hit buton A.
2.1) rotate the image and hit button A again until the probability stays at 1.
2.2) Repeate this at different angles until the prdiction (A) has a probability of 1.
3) Hold up another image (in my case grapes) before the webcam and hit Button B
3.2) rotate the same image and notice the prediction (B) flickers, keep repeating this until the prediction (B)
     has a probability of 1 regrdless of the angle or distance from the camera.
4) Repeat steps 2 and 3 for another object (in my case a Lomon).
5) Now that you have an image associated with prediction A, B and C create a state D as your neutral state.
6) Keep hitting D.. in this case Prediction D was just me in the camera and none of the objects A, B or C were visible.
No while the Prediction D (neutral state) with probability 1 was present, introduce the Orange and watch the prediction switch to A with probability 1.  Repeat this for the grapes and leamon.

This is totally awesome to watch the system change predictive state to match each of the objects on which it was trained.

Totally awesome!!!


