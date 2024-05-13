# RUINS TO RECOVERY: Enhancing Building Detection in Disaster-Affected Areas Using Machine Learning

Welcome to the official repository for our cutting-edge machine learning project, aimed at enhancing the detection of buildings in disaster-affected areas. Utilizing state-of-the-art algorithms and high-resolution satellite imagery, this initiative marks a significant leap forward in disaster response technology.

## About the Project

In the aftermath of natural disasters, rapid and accurate damage assessment is critical for effective emergency response and resource allocation. Our project addresses this need by automating the detection of damaged buildings using advanced machine learning models, which analyze satellite imagery to provide timely and precise evaluations of affected areas.

### Objectives
- **Rapid Detection**: Significantly reduce the time required to assess damage by automating the detection process.
- **High Accuracy**: Improve the reliability of assessments to aid in better decision-making during crisis situations.
- **Scalable Solutions**: Develop a system that can be adapted to various disasters and geographical locations.

## Technical Overview

### Technologies and Frameworks
This project leverages the following technologies:
- **TensorFlow & Keras**: For building and training deep learning models.
- **Mask R-CNN, Res2 UNet, SegFormer**: Cutting-edge models for semantic segmentation and object detection tailored to our specific needs in disaster scenarios.
- **Rasterio & PIL**: For image processing tasks.
- **GeoPandas**: To handle geospatial data effectively.
- **NVIDIA A100 GPUs**: Utilized for their robust computational power, facilitating faster model training.

#### Model Mask RCNN - https://arxiv.org/abs/1703.06870
<img width="883" alt="image" src="https://github.com/Ruthik27/Building_Detection/assets/62241739/52215c07-498b-4865-af63-07d7d09d40cc">

https://github.com/matterport/Mask_RCNN

### Data Handling
- **High-Resolution Maxar Imagery**: Satellite images are processed into 1024x1024 pixel chunks, providing the necessary granularity for accurate building detection.
- **GIS-Compatible Dataset**: Integration with GIS tools allows for effective mapping and analysis of the data.

### Data Processing
#### Mask Creation
<img width="596" alt="image" src="https://github.com/Ruthik27/Building_Detection/assets/62241739/c92dcce9-6c75-4c78-ae8f-433a5b4176e3">

#### Contour Creation
<img width="627" alt="image" src="https://github.com/Ruthik27/Building_Detection/assets/62241739/f1f0a5f0-e922-43ab-b550-b6fb4ad6162a">

### Model Architecture
- **Customized Mask R-CNN**: Adapted to detect subtle variations in building structures post-disaster.
- **Res2 UNet & SegFormer**: Employed for their efficiency in handling complex image segmentation tasks at scale.

## Setup and Installation

Ensure you have Python 3.10 installed, then clone this repository and set up the environment:
```bash
git clone https://github.com/your-repository/building-detection.git
cd building-detection
pip install -r requirements.txt
```

### Usage Instructions
Execute the model training and evaluation by running:
```bash
python run_testing_detection.py
```

## Experiments and Insights

Our evaluation process leverages Neptune.ai for tracking experiments, allowing for meticulous analysis of model performance over various configurations. Key results include:
- **Precision and Recall**: Achieved high precision with varied recall across models, indicating robust detection capabilities.
- **IoU (Intersection over Union)**: This metric confirmed the accuracy of our segmentation, critical for precise damage assessments.

#### Test Results
<img width="405" alt="image" src="https://github.com/Ruthik27/Building_Detection/assets/62241739/6bc2d312-86eb-4127-a590-fa89eb3f0ecc">

<img width="406" alt="image" src="https://github.com/Ruthik27/Building_Detection/assets/62241739/bc40098e-8385-4880-9f7a-62f85abd22aa">

### Configurations Explored
- **Learning Rates**: Tuned to balance fast convergence with model stability.
- **Batch Sizes**: Optimized to maximize the efficiency and capability of our GPU resources.

## Future Directions

- **Real-Time Analysis**: Incorporate live satellite feeds to provide instant assessments.
- **Algorithmic Improvements**: Continuous improvement of model accuracy and efficiency.
- **Scalability and Adaptability**: Extend our models to operate across different disaster scenarios and geographical locations.

#### Post Processing
<img width="406" alt="image" src="https://github.com/Ruthik27/Building_Detection/assets/62241739/c2b7150c-0ba5-46a1-a7b9-d0968542e747">


## Contribute

We welcome contributions from the community. Please fork this repository, make your changes, and submit a pull request with your improvements.

## Licensing

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

<img width="392" alt="image" src="https://github.com/Ruthik27/Building_Detection/assets/62241739/f2be2c60-cc16-42bd-94fb-3ce3d14311f7">


<img width="409" alt="image" src="https://github.com/Ruthik27/Building_Detection/assets/62241739/cd357b20-f5f3-42cc-884d-75042cd12585">

<img width="409" alt="image" src="https://github.com/Ruthik27/Building_Detection/assets/62241739/4c4df0c3-be42-4023-bede-171b63e300fa">

---

https://www.cviog.uga.edu/information-technology/

https://gacrc.uga.edu/
