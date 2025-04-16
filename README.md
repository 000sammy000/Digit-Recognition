# NYCU Computer Vision 2025 Spring HW2
StudentID:110550142  
Name:黃芷柔  

## Introduction
In the Digit Recognition task, the primary goal is to identify and classify digits from images, a crucial application in fields such as automatic number plate recognition, postal sorting, and form processing. The challenge lies in handling varying image sizes, differing proportions of digits within images, and accurately detecting small objects in noisy environments.  
To address these challenges, we employ the Faster R-CNN framework, which is widely used for object detection tasks. Faster R-CNN consists of three key components: the backbone, the Region Proposal Network (RPN), and the head. The backbone extracts features from input images, while the RPN generates candidate regions for potential objects, and the head is responsible for classification and bounding box regression.  
For this task, we utilize the fasterrcnn_mobilenet_v3_large_fpn model, which incorporates MobileNetV3 as the backbone and Feature Pyramid Network (FPN) as the neck. MobileNetV3 is a lightweight and efficient model, making it ideal for applications that require real-time processing. FPN enhances the model's ability to detect objects at multiple scales, which is particularly useful in recognizing small digits that occupy a minor portion of the image. By modifying different parts of the Faster R-CNN architecture, such as the anchor sizes and the sample ratio in the RPN, we aim to optimize the performance for digit recognition.


## How to install
You can run this project directly in your browser using Google Colab. No local setup is needed.


Steps:
Click the badge above to open the notebook in Google Colab.

Run all cells in the notebook to install dependencies, train, and evaluate the model.

📦 All required packages will be installed automatically in the notebook. Example setup:

python
複製
編輯
!pip install torch torchvision
!pip install -r requirements.txt
⚠️ Make sure you are using a GPU runtime by going to
Runtime > Change runtime type > Hardware accelerator > GPU.


## Performance snapshot
