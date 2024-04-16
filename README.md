# Multi-Face-Detection-System
Multi Face Detection System

![image](https://github.com/Praveen1034/Multi-Face-Detection-System/assets/145018906/e22d5d68-0c90-4f40-9ef3-ee71ff84a370)

1. **Cascade Classifier Loading**:
   - We load a pre-trained cascade classifier for frontal face detection using the `CascadeClassifier` function from the OpenCV library.

2. **Image Loading**:
   - We load an image file from the specified file path using the `imread` function from OpenCV.

3. **Grayscale Conversion**:
   - To perform face detection, we convert the loaded image from color (BGR) to grayscale using the `cvtColor` function. The face detection algorithm typically works on grayscale images.

4. **Face Detection**:
   - We apply the `detectMultiScale` method on the grayscale image along with specific parameters (scale factor and minimum neighbors) to detect faces. This method returns a list of rectangles representing the detected faces.

5. **Drawing Rectangles Around Faces**:
   - For each detected face, we draw a rectangle around it on the original color image using the `rectangle` function. This visually marks the detected faces.

6. **Image Resizing**:
   - To display the image with detected faces, we resize the original image to a smaller size using the `resize` function. This is done to fit the image within the display window.

7. **Displaying the Image**:
   - Finally, we display the resized image with the detected faces using the `imshow` function. The image remains displayed until any key is pressed, after which all display windows are closed using `destroyAllWindows`.

