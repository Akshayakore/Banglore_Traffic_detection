# Data Annotation GUI

Welcome to the comprehensive documentation for the Data Annotation project! This intuitive platform offers a powerful graphical user interface (GUI) designed to streamline the process of annotating images, performing object detection through a YOLO model, and enhancing your data labeling tasks using the LabelImg tool.

In the following sections, we'll guide you through the installation, setup, and optimal utilization of the Data Annotation platform. Whether you're an AI researcher, developer, or enthusiast, this documentation will equip you to leverage the project's capabilities effectively.

Let's embark on this journey of transforming raw data into a refined and annotated dataset, laying the foundation for robust machine learning models.
### Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Flowchart](#flowchart)
- [Inference Phase-1](#inference-phase-1)
- [Training Dataset](#training-dataset)
- [Training](#training)
- [Inference Phase-2](#inference-phase-2)
- [Getting Started](#getting-started)
  - [Uploading Video](#uploading-video)
  - [Uploading Images](#uploading-images)
  - [Running YOLO Model](#running-yolo-model)
  - [Downloading Labels](#downloading-labels)
  - [Using LabelImg](#using-labelimg)
  - [Modify Classes](#modify-classes)
- [Conclusion](#conclusion)
- [Contributions](#contributions)
- [References](#references)

### Introduction

Data annotation plays a pivotal role in training and refining machine learning models, especially in the realm of computer vision. The Data Annotation project emerges as a solution that bridges the gap between accuracy and user-friendliness. By combining the capabilities of image uploading, YOLO-based object detection, label downloading, and the LabelImg annotation tool, this project empowers users to efficiently prepare and enrich their datasets for various applications.

### Features
- **Video Upload:** Seamlessly upload videos and convert the videos into frames.
- **Image Upload:** Seamlessly upload images for annotation and processing.
- **YOLO Model Integration:** Employ advanced YOLO-based object detection for accurate labeling.
- **LabelImg:** Utilize the powerful LabelImg tool for precision annotation refinement.
- **Modify classes:** This allows the filteration of selected classes.

### Flowchart
<div style="text-align:center;">
    <img src="https://github.com/TiHAN-Hyderabad/UGV-Object-Detection-21-Class-Model-Training/assets/83684051/6cfd23c9-e6a2-4fb2-acc5-2f123ad1df0c" alt="image" width="50%" height="50%">
</div>

In the project lifecycle, Inference Phase-1 involves preparing the data and setting up the model, followed by the training phase where the model learns from the data, and finally, the Inference phase-2 stage where the trained model makes predictions or classifications based on new input.

### Inference Phase-1
This initial phase focuses on preparing the necessary data and setting up the machine learning model for training. Data preparation involves tasks such as cleaning, formatting, and organizing the data to make it suitable for the model. Using the training GUI labels are generated for the dataset.

### Training Dataset
The annotated dataset with images and labels is [here](https://github.com/TiHAN-Hyderabad/TTL-USECASE-1/tree/main/Datasets/final_data).

### Training 
The generated labels from the Inference Phase-1 is the input to the training phase. In this phase, the prepared model is exposed to the training data to learn patterns and relationships. The model iteratively adjusts its parameters to minimize the difference between its predictions and the actual outcomes in the training data. The training phase continues until the model reaches a satisfactory level of performance.

### Inference Phase-2
The output of training phase is the Inference result.
After the model has been trained, it moves to the inference phase, where it is applied to new, unseen data. In this phase, the trained model makes predictions or classifications based on input it hasn't encountered before. The model uses the knowledge gained during training to generalize and provide meaningful outputs for new data.


### Getting Started <a id="getting-started"></a>

### Uploading Video <a id="uploading-video"></a>

1. On the main page, click Browse beside the "Upload Video" button.
2. Select the video you want to upload from your local machine.
3. Click the "Upload Video" button to initiate the video upload process.
4. Frames are generated during the upload process.
5. Click the "Download Images" button to download the frames.
6. Click "Run Video" button and click "Download Labels" button to download video with object detection. 

### Uploading Images <a id="uploading-images"></a>

1. On the main page, click Browse beside the "Upload Images" button.
2. Select the images you want to upload from your local machine.
3. Click the "Upload Images" button to initiate the image upload process.
4. The uploaded images will be displayed on the page.

### Running YOLO Model <a id="running-yolo-model"></a>

1. Click the "Run" button.
2. The YOLO model will process the selected image and highlight detected objects.

### Downloading Labels <a id="downloading-labels"></a>

1. After running the YOLO model, click the "Download Labels" button.
2. The generated labels for the processed image will be downloaded in a ZIP archive format.
3. Extract the ZIP archive to access the labels and associated text files.

### Using LabelImg <a id="using-labelimg"></a>

1. Click the "Run LabelImg" button to launch the LabelImg tool.
2. Open the extracted folder in LabelImg to further annotate the images and improve labeling accuracy.
3. Follow the tutorial from [here](https://github.com/HumanSignal/labelImg).
4. Save the annotations and exit LabelImg.


### Modify classes<a id="using-labelimg"></a>

1. Folder with images, text files and classes.txt file can be uploaded into "Uplaod Folder".
2. Select the classes from dropdown and click "Submit".
3. Click "Run Modify Classes" button. This removes the label values of other classes and the labels for selected classes remain in the txt files.
4. Click "Download Folder" button.
5. Folder with images, txt files and classes.txt gets downloaded.

### Conclusion

Congratulations! You've now familiarized yourself with the core features of the Data Annotation project. From seamless image uploading to robust object detection and annotation using YOLO, this platform offers a unified solution for enhancing your dataset's quality and utility.

We encourage you to explore the different sections of this documentation to harness the full potential of the Data Annotation project. Whether you're a machine learning practitioner, a developer, or an enthusiast, this GUI-driven tool can significantly accelerate your data annotation and model training workflows.

If you have any questions, feedback, or suggestions, please don't hesitate to contribute to the project. We welcome your engagement and look forward to seeing the creative ways you leverage this tool for your image annotation needs.

Happy annotating and detecting!

### Contributions <a id="contributions"></a>

Contributions to this project are welcome! Feel free to submit bug reports, feature requests, and pull requests. Please adhere to the project's coding standards and guidelines.

### References
1. Indian Dataset: https://idd.insaan.iiit.ac.in/
2. International Dataset: https://www.nuscenes.org/
3. YOLOv5: https://github.com/ultralytics/yolov5
4. LabelImg: https://github.com/HumanSignal/labelImg
