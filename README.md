# SMART_WEED_DETECTION_AND_REMOVAL_SYSTEM_Final_YOLOv8
Smart Weed Detection using YOLOv8 for crop and weed classification. Includes dataset preprocessing, augmentation, and model training on a balanced dataset with performance evaluation metrics such as precision, recall, and mAP.
# Smart Weed Detection System using YOLOv8

This project focuses on detecting weeds and crops in agricultural fields using deep learning. The system is designed to help farmers identify unwanted weeds and improve crop management using computer vision techniques.

The project currently implements the YOLOv8 model for object detection. The model is trained on a custom dataset containing crop and weed images with bounding box annotations.

# Dataset Description

The dataset consists of three parts:

Training set with 1579 images
Validation set with 451 images
Test set with 226 images

Each image contains annotations for two classes:

0 represents  # crop(Banana Plant)
1 represents weed

The dataset is prepared in YOLO format with corresponding label files for each image.

Model Training

The YOLOv8 model was trained using Google Colab with GPU support. Training was performed for multiple epochs to observe improvement in performance metrics.

The following results were obtained during training:

At 10 epochs
Precision was 0.597
Recall was 0.362
mAP at 0.50 was 0.407
mAP at 0.50 to 0.95 was 0.215

At 20 epochs
Precision was 0.612
Recall was 0.441
mAP at 0.50 was 0.482
mAP at 0.50 to 0.95 was 0.256

At 30 epochs
Precision was 0.690
Recall was 0.575
mAP at 0.50 was 0.634
mAP at 0.50 to 0.95 was 0.372

At 40 epochs
Precision was 0.734
Recall was 0.636
mAP at 0.50 was 0.699
mAP at 0.50 to 0.95 was 0.440

At 50 epochs
Precision was 0.801
Recall was 0.664
mAP at 0.50 was 0.745
mAP at 0.50 to 0.95 was 0.506

These results show consistent improvement in detection performance as the number of epochs increased.

Visualization

Performance graphs were generated for Precision, Recall, mAP at 0.50, and mAP at 0.50 to 0.95 across different epochs. These graphs help in understanding how the model improves during training and how accuracy stabilizes over time.

Model Output

The final trained model was saved as YOLOv8_best.pt after completing training. This model can be used for detecting crops and weeds in new images.

Models Used

YOLOv8 is used for fast and real-time detection. It processes the entire image in a single pass and is suitable for applications requiring speed.
