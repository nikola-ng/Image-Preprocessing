# Image-Processing

1. Get the image to work with. This process usually involves some functions so that you can read the image from different sources (camera, video stream, disk, online resources)

2. Process the image by applying image-processing techniques to achieve the required functionality (for example, detecting a cat in an image).
Step 2 can be broken down into 3 processing levels:
- Low-level process:
Usually takes an image as the input and then outputs another image. 
Example procedures that can be applied in this step include the following:
    + Resize
    + Noise removal
    + Image sharpening
    + Illumination normalization
    + Perspective correction
In connection with the face-detection example, the output image can be an illumination normalization image to deal with changes caused by sun reflection.
  
- Mid-level process:
Takes the preprocessed image to output some kind of representation of image. 
  Consider this as a collection of numbers (for example, a vector containing 100 numbers), which summaries the main information. In connection with the face-detection example, the output could be a rectangle defined by a point (x,y), the width and the height containing the detected face.
  
- High-level process:
Takes this vector of numbers (usually called attributes) and outputs the final result. For example, the input could be the detected face and the output could be the following:
    + Face recognition
    + Emotion recognition
    + Drowsiness and distraction detection
    + Remote heart rate measurement from the face
    
3. Show the result of the processing step (for example, drawing a bounding box in the image and saving it to disk)
