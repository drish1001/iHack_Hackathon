# iHack Hackathon

## Overview
This project demonstrates **object detection** using the YOLO (You Only Look Once) algorithm implemented with OpenCV. The repository provides a pipeline to detect objects in images by leveraging pre-trained YOLO weights and configuration files. The output highlights detected objects with bounding boxes and their respective class labels.

The project was developed as part of a hackathon to showcase the power of deep learning-based object detection models in real-world applications.

## Features
- **Object Detection with YOLO:** Detects multiple objects in an image with high accuracy.
- **Pre-trained Model Usage:** Utilizes YOLOv3 pre-trained weights for object detection.
- **Customizable Inputs:** Allows users to test the model on their own images.
- **Output Visualization:** Displays output images with bounding boxes and class labels for detected objects.

## Technologies Used
- **Programming Language:** Python 3.6
- **Libraries:**
  - OpenCV (cv2)
  - NumPy
- **YOLO Framework:**
  - YOLOv3 weights (`yolo.weights`)
  - YOLOv3 configuration file (`yolov3.cfg`)
  - Class labels (`yolov3.txt`)

## Installation

Follow these steps to set up and run the project:

1. Clone this repository:
   ```bash
   git clone https://github.com/drish1001/iHack_Hackathon.git
   ```

2. Navigate to the project directory:
   ```bash
   cd iHack_Hackathon
   ```

3. Download the YOLOv3 weights file:
   - Download the `yolo.weights` file from [pjreddie.com](http://pjreddie.com/media/files/yolov3.weights).
   - Place the downloaded `yolo.weights` file in the root directory of the project.

4. Install required Python libraries:
   ```bash
   pip install numpy opencv-python
   ```

5. Prepare input images:
   - Place training images in the `input_images/` folder.
   - Place test images (named `test0.jpg`, `test1.jpg`, etc.) directly in the root directory.

## Steps to Run the Project

1. Run the `output.py` script from the terminal:
   ```bash
   python output.py
   ```

2. The script will process the test images and display output images with bounding boxes and class labels for detected objects.

3. The processed output image will also be saved as `object-detection.jpg` in the root directory.

## Project Structure

```
iHack_Hackathon/
├── input.py                # Script for processing training images
├── output.py               # Main script for object detection on test images
├── yolo_opencv.py          # Additional script for object detection using arguments
├── yolov3.cfg              # YOLOv3 configuration file
├── yolov3.txt              # Class labels for YOLOv3 model
├── input_images/           # Folder containing training images
│   ├── image1.jpg          # Example training image
│   ├── image2.jpg          # Example training image
│   └── ...
├── test0.jpg               # Example test image 0
├── test1.jpg               # Example test image 1
├── object-detection.jpg    # Output image with bounding boxes (generated after running)
└── LICENSE                 # License file (MIT License)
```

## Example Output

After running the project, you will see an output image like this:

- Objects detected in the image are highlighted with bounding boxes.
- Each bounding box is labeled with its corresponding class name (e.g., "person," "car," etc.).

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This implementation is based on work by Arun Ponnusamy (http://www.arunponnusamy.com).
- Special thanks to [pjreddie.com](http://pjreddie.com) for providing pre-trained YOLO weights and configuration files.

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/33876548/66dd1b9d-c571-4568-8980-3d78be5fe5e4/paste.txt
