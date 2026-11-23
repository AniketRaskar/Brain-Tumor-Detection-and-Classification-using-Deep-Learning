# Brain-Tumor-Detection-and-Classification-using-Deep-Learning
My project is **Brain Tumor Detection and Classification using Deep Learning**, which is an extension of a published research paper.

The original research paper used ResNet152 and InceptionV3 for binary classification of brain MRI images, achieving a maximum test accuracy of 97.22%.

I extended this work to **four-class classification: glioma, meningioma, pituitary tumor, and no tumor**.

I used a brain MRI dataset containing 5,712 training images and 1,311 evaluation images. All images were resized to 224 × 224 pixels and normalized.

For classification, I implemented two pretrained CNN architectures, **ResNet50 and InceptionV3**, using TensorFlow and Keras.

I followed a two-stage transfer-learning approach. Initially, I froze the pretrained CNN backbone and trained only the newly added classifier layers. Then I selectively unfroze deeper convolutional layers and fine-tuned the models using a small learning rate of 1e-5.

Fine-tuning improved ResNet50 accuracy from 74.6% to 88.8%, while InceptionV3 improved from approximately 93% to 97%.

I evaluated the models using accuracy, precision, recall, F1-score, and confusion matrices. InceptionV3 achieved the best reported results, with approximately 97% accuracy and 0.96 macro F1-score.

The main contribution of my project was extending binary tumor detection to multiclass classification and investigating how selective fine-tuning improves pretrained CNN performance.
