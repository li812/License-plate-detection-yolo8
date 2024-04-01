# License-plate-detection-yolo8

The code provided in the notebook named final consist of two functions: one for detecting license plates in a video, and another for extracting registration numbers from images containing license plates. The first function saves frames with detected license plates to a folder called "LP_frames", and the second function extracts registration numbers from images in a specified folder and saves them to a folder called "mined_RP_numbers".

To use these functions, you need to provide a video file path to the `detect_license_plate` function and specify the input folder containing images with detected license plates to the `extract_register_numbers_from_folder` function.

Here's how you can use these functions:

```python
# Call detect_license_plate function with your video file path
video_path = "path/to/your/video.mp4"
detect_license_plate(video_path)

# Once the frames with detected license plates are saved in "LP_frames" folder, 
# call extract_register_numbers_from_folder function with the folder path
input_folder = "LP_frames"
extract_register_numbers_from_folder(input_folder)
```

Make sure you have the necessary dependencies installed, such as OpenCV (`cv2`), `ultralytics`, `easyocr`, and their dependencies. Additionally, ensure that the YOLO model file "L_Plate.pt" is available in your working directory or specify the correct path to it.