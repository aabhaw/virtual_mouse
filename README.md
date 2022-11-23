# virtual_mouse

Project name: Hand Gesture Recognition Based VIrtual Mouse


Hand detection-
  The web camera is accessed using VideoCapture() of OpenCV.
  It is detected using mediapipe.
  
Pre-processing of the picture of hand-
  The image captured is edited as follows.
    Horizontal flip method of OpenCV is used.
    Color schema is changed using cvtcolor method os OpenCV.
    Background removal is done using fill method of numpy.
 
Getting the co-ordinates-
  Landmark Algorithm is used to extract the co-ordinates.
  Mediapipe library is used. 
  The co-ordinates extracted are plotted on the white background.

Classification of gesture using CNN Model-
  The image is then sent to CNN (Convolutional Neural Network).
  CNN then recognizes the gesture and gives the result accordingly.

Controlling mouse-
  The result from the CNN is used to determine the mouse operation to be done.
  The mouse operations supported are-
    1. Navigation
    2. Left click
    3. Right click
    4. Scroll down
    5. Scorll up
    6. Screenshot.
  All the gestures are done using the PyAutoGUI.
  
  
CNN model-
  The dataset consists of 9000 images.
  The model is trained using 7200 images.
  The training set for each gesture consist of 1500 images.
  The testing set for each gesture consist of 300 images.
  Training accuracy of 98.87% achieved.
  Testing accuracy of 87.5% is achieved.
  

Contrary to the existing virtual mouse, it doesnt require any additional hardware thus making it more effective and easy to use. Also all the gestures are natural gestures as opposed to the number gestures proposed in earlier papers.
  
