# Spot-check

Melanoma Detection with Image Recognition

This is a model that uses image recognition to identify melanoma in 8 different categories. The model is trained on images that are resized to 256x256 pixels. It uses a MobileNetV2 pre-trained model with the last few layers modified to include a dense layer with 8 neurons to output the classification results.

Data Augmentation

To reduce overfitting and improve model generalization, we used data augmentation techniques on the training dataset. The following transformations were applied to each image in the dataset:

Random horizontal and vertical flips
Random rotation of up to 30 degrees
Preprocessing

The images were preprocessed using the MobileNetV2 preprocessor, which applies the necessary transformations to the input data so that it is suitable for the pre-trained model. This includes mean subtraction and scaling the pixel values.

Base Model

The MobileNetV2 model was chosen as the base model for this project. It is a lightweight and efficient model that performs well on mobile devices. The model was pre-trained on the ImageNet dataset and we modified the last few layers to include a dense layer with 8 neurons to output the classification results.

Training

The model was trained on a dataset of melanoma images that were labeled with 8 different categories. The training data was split into training and validation sets, and the model was trained for 128 epochs using the Adam optimizer with a learning rate of 0.00001. The loss function used for this multi-class classification problem was categorical cross-entropy, and the model was evaluated based on accuracy.

Results

The model achieved an accuracy of around 70% on the validation set. This is a good result considering the limited number of training images available and the complexity of the task. With more training data and a more complex model architecture, it is possible to achieve higher accuracy levels.

Usage

The trained model can be used to predict the probability of an input image belonging to each of the 8 categories. The predicted category with the highest probability can then be used to classify the image.

Conclusion

This project demonstrates the potential of using image recognition techniques for the early detection of melanoma. By analyzing skin lesions, it is possible to identify potential cancerous growths at an early stage, increasing the chances of successful treatment. The model can be further improved with additional training data and a more complex architecture, and can be deployed on mobile devices for easy and convenient use by healthcare professionals.

![Image 3-30-23 at 11 29 PM](https://user-images.githubusercontent.com/113937079/229015711-de7497b0-b739-4f68-81f7-3afbef661ccc.jpg)

