# Parking-Space-Detector

# Install
cvzone

numpy

opencv-python

pip

# Marking Parking Spaces on an Image
The code allows users to define parking spots on an image:

Loading Existing Parking Spots: It tries to load a file that contains positions of parking spots (if it exists).

Displaying the Image: It opens an image (carParkImg.png) and displays it using OpenCV.

Mouse Interaction: It lets the user click on the image:

Left-click to mark a new parking spot.

Right-click to remove an existing parking spot.

Saving Parking Spot Positions: It saves the positions of these parking spots in a file (CarParkPos) using the pickle library.

# Analyzing Parking Spaces in a Video
The code reads a video and identifies occupied and free parking spaces:

Video Processing Loop: It continuously processes frames from a video file (carPark.mp4) using OpenCV.

Image Processing Techniques: It converts each video frame to grayscale and applies techniques like blurring and thresholding to enhance the image.

Parking Space Detection: It checks each pre-defined parking space in the video frame by cropping that particular region.

It counts the number of non-zero pixels in that region to determine occupancy.

If there are fewer non-zero pixels, it assumes the space is free; otherwise, it's considered occupied.

Drawing Results: It draws rectangles around these parking spaces and labels them as free or occupied based on the pixel count.
