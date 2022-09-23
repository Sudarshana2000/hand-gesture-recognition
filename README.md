# hand-gesture-recognition

Recognises basic hand gestures i.e counting fingers, with finger tracking using OpenCV and Python.


## Usage

Firstly, it requires a stable plain background which is used to differentiate our ROI (i.e hand) in image frames with the same background. This helps in better detection of hands. 

For images: provide a background image along with the image of hand. Make sure both images are of same shape.
```
hand_gesture.check_gesture(backgroundImagePath, handImagePath)
```

For videos: keep the background clear and stable for a few seconds, then insert hand in the ROI frame.
```
hand_gesture.real_time_feed()
```

In the output frame, hand-gesture is recognized by counting fingers and tracking fingertips. Threshold image of hand is also displayed alongside to let users adjust the hand in ROI properly.

Please refer the code for better understanding of the procedure.


## Results

<img src="https://github.com/Sudarshana2000/hand-gesture-recognition/blob/master/output.png" />
<br />