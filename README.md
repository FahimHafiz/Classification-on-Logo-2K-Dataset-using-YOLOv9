# Classification-on-Logo-2K-Dataset-using-YOLOv9
"Logo-2K+" is a large-scale logo dataset with a diverse range of logo classes from real-world logo images containing 167,140 images with 10 root categories and 2,341 categories. In this work, we apply the newly released YOLOv9 for logo classification purposes in the "Logo-2K+" dataset.

# Custom Model Architecture for YOLOv9 for classification purposes
YOLOv9 do not have the classification module yet. In this work, we modified the object detection module of YOLOv9 for classfication purpose. The modifed model is the 'yolov9c-cls.yaml' file which needs to be imported in the model while training.

# Dataset Organisations
The datasets are organised according to subclasses as follows:

![image](https://github.com/FahimHafiz/Classification-on-Logo-2K-Dataset-using-YOLOv9/assets/39213309/e98ceed0-aae1-481a-9693-377fb0266bae)

# Dataset Preprocessing
Augmentations such as flipping, rotating and grayscaling & high pass filters were used. Also, each subclasses have 400 images after preprocessing and augmentation.

# Run "logo_classification_without_preprocessing_yolov9.ipynb":
This colab file trains the dataset without applying any augmentations, filtering. You can simply set their directories according to your own and import the custom yaml file given in the repository. Then, you can simply run all the sections to train the YOLO model and classify the datasets!

The results generated from this codes are:
confusion matrix:
![confusion_matrix_wo_pr](https://github.com/FahimHafiz/Classification-on-Logo-2K-Dataset-using-YOLOv9/assets/39213309/f5172b93-c18d-442c-aca7-070778358787)
Results:
![results_wo_pr](https://github.com/FahimHafiz/Classification-on-Logo-2K-Dataset-using-YOLOv9/assets/39213309/fdbfcd18-8351-4af5-ab25-b08fbe31c0de)
Prediction Sample:
![val_batch0_pred_wo_pr](https://github.com/FahimHafiz/Classification-on-Logo-2K-Dataset-using-YOLOv9/assets/39213309/6314e0e9-a21c-4edd-b5bc-9fbf4473e4d3)



