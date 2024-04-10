Video-Summarization
Steps to Run Frame Difference Video Processing Program:

•	Python and Library Installation:
Ensure Python is installed (Version 3.6 or above) on your system. Install necessary libraries by running the following commands in your terminal:
•	OpenCV: pip install opencv-python
•	NumPy: pip install numpy
•	Jupyter Notebook (Optional):
•	Ensure that you have Jupyter installed if you prefer to run the code within a Jupyter Notebook environment.

Execute the Project:

•	Open the Project:
•	Open the project link or navigate to the project directory on your local system.
•	Clone the Repository:
•	Click on the "Code" button next to the "Add file" button.
•	Select HTTPS and copy the URL.
•	Open the terminal in the desired project folder.
•	Type git clone [paste URL] and press enter.

Run the Code:

Open the "Frame-Difference-Video-Processing" folder in your terminal.
Type the command jupyter notebook and press enter.
Select and open the "frame_difference.ipynb" Jupyter file.

Steps to Execute the Program:

•	OpenCV Video Capture:
The code captures frames from the video file specified in video = cv2.VideoCapture('first_video.mp4').

•	Frame Difference Processing:
It calculates the absolute frame difference between consecutive frames using NumPy operations.
Frames with a significant difference (thresholded) are written to the output video file "final.mp4" using OpenCV's VideoWriter.

•	Display and Termination:
Displays frames in real-time using OpenCV's cv2.imshow() function.
Press 'q' key to terminate the program and close the OpenCV windows.

•	Output and Statistics:
The program calculates and prints statistics about the frames processed:
Total frames read (c).
Unique frames written to output (a).
Common frames skipped due to low difference (b).

•	Resource Cleanup:
After program execution, it releases video capture and writing resources using video.release() and writer.release().
Close all OpenCV windows using cv2.destroyAllWindows().
