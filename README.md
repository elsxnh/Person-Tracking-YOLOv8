# Person-Tracking-YOLOv8

📁 Created by: Elsa Nurul Hidayah, 2023

This repository is created to fulfill the bootcamp Computer Vision project requirement from Indonesia AI.

🔬 This project of person tracking is developed using existing models of YOLOv8l with settings of 25 and 50 epochs, due to the constraint in time and resources. Ths usage is simple: to create an artificial intelligence model to track people for the needs of a futuristic smart city. This system will then automatically detect and track people within a specific point to maintain safety and security within the city. 

## RESULTS

The dataset used is from COCO Dataset, downloaded from the fifty one zoo library (dataset preparation is already included in the notebook given) and the class used is only 'person'. The components of the dataset are explained below:

 - ± 3000 images as training
- ± 1000 images as validation
- ± 500 images as test
  
After the model is trained from the image dataset, the corresponding results are shown below:

|                      	| **YOLOv8l 25 epochs** 	| **YOLOv8l 50 epochs** 	|
|----------------------	|:---------------------:	|:---------------------:	|
|    **_Precision_**   	|         0.726         	|          0.75         	|
|     **_Recall_**     	|          0.65         	|         0.656         	|
|     **_mAP@50_**     	|          0.71         	|         0.722         	|
|   **_mAP(@50-95)_**  	|         0.465         	|         0.482         	|
| **_Inference Time_** 	|          12.4         	|          12.4         	|

The graphical results are shown below: 

- YOLOv8l 25 Epochs
![results](https://github.com/elsxnh/Person-Tracking-YOLOv8/assets/77186233/09dc6404-2fcb-480b-8374-5520a0e2b2d6)

- YOLOv8l 50 Epochs
![results](https://github.com/elsxnh/Person-Tracking-YOLOv8/assets/77186233/e8a76ebc-9163-4976-b3c3-7c8c2fe339f0)

The result using the weights on a video can be seen in the link below:

https://drive.google.com/file/d/1-XcaZFrSpQ686q2-hLRr1AZr1Z0aEsV7/view?usp=sharing 

## Getting Started

To run this project on your local machine using Google Colab connected to Google Drive, follow these systematic steps:

### Prerequisites

Before you begin, make sure you have the following prerequisites:

1. Google Colab account
2. Access to Google Drive
3. Dependencies (in the section below)

### Procedure

1. Open Google Colab and navigate to the notebook located in the project's directory.

2. Mount Google Drive within the Colab notebook by executing the following cell:

    ```python
    from google.colab import drive
    drive.mount('/content/drive')
    ```
3. Clone the repository to your google colab (recommended):

    ```bash
    git clone https://github.com/elsxnh/Person-Tracking-YOLOv8.git
    ```

4. Install any necessary dependencies by following the instructions in the notebook.

5. Run the notebook cells sequentially to train and test your model.

By following these steps, you should be able to successfully run the project and understand the implemented features.

