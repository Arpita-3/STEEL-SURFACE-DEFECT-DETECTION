# Steel Surface Defect Detection

This project uses deep learning to automate the detection and classification of surface defects in steel sheets. Built using a Faster R-CNN model with a ResNet-50 backbone, the system accurately detects and localizes five types of common defects in steel manufacturing images.

## 🔍 Project Overview

Manual inspection of steel sheets is time-consuming and prone to errors. Our solution uses a deep learning-based object detection model to identify:
- **Crazing**
- **Inclusion**
- **Patches**
- **Pitted Surface**
- **Scratches**



## 🧠 Technologies Used

- **Python**
- **PyTorch** – model development and training
- **Torchvision** – pre-trained Faster R-CNN with ResNet-50
- **OpenCV** – image handling and output visualization
- **Pandas, NumPy, Pillow**
- **XML Parsing** – for PASCAL VOC annotations



## 📁 Dataset
FROM kaggle :- NEU-surface-defect-database(you can download)
The dataset contains 1417 labeled images distributed across five folders (one per defect type), with XML files following the VOC annotation format.

| Defect Type     | Images |
|-----------------|--------|
| Crazing         | 283    |
| Inclusion       | 283    |
| Patches         | 284    |
| Pitted Surface  | 283    |
| Scratches       | 284    |
| **Total**       | **1417** |

Each image is annotated with bounding boxes marking the defect locations.


## 📈 Output

The model produces images with:
- Bounding boxes around defects
- Labels with confidence scores
- Visual distinction using different colors for each defect type

Example output:
- Green boxes for Inclusion
- Orange for Patches
- Blue for Crazing
- etc.


 
