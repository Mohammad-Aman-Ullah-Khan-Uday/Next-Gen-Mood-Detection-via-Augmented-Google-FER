**Project title**: [Next Gen Mood Detection via Augmented Google-FER](https://github.com/Mohammad-Aman-Ullah-Khan-Uday/Next-Gen-Mood-Detection-via-Augmented-Google-FER)

There has been extensive work in mood detection using machine learning, focusing on physical and neuro-physical data, along with emotion recognition through eye tracking. My goal is to demonstrate that a person’s mood can be detected solely through images of their eyes, as I believe mood is reflected in one’s eyes. To achieve this, I chose Convolutional Neural Networks (CNNs) for this task because they allow the model to automatically learn and extract features, eliminating the need for manual feature extraction. 

In this project, I used the [FER-2013](https://www.kaggle.com/datasets/msambare/fer2013/data) dataset, which has 28,709 training and 3,589 testing images for seven emotions. Since "Disgust" had too few samples, I excluded it and focused on six emotions: **Angry**, **Fear**, **Happy**, **Neutral**, **Sad**, and **Surprise**. I created a custom dataset of 2,230 training and 351 testing eye images, cropped in a 16:9 aspect ratio. Before training, these images were grayscale and resized to 48x48 pixels, similar to the FER-2013 preprocessing.

The dataset was organized into classes, with images stored in separate folders based on emotions, focusing solely on eye images from various expressions. While FER-2013 has thousands of images for each emotion, the dataset only contains a few hundred images per emotion, highlighting its limitations in quantity and diversity.

Using the Custom FER-2013 dataset, I developed CNN models by focusing exclusively on the eye regions for six emotions: happy, fear, sad, angry, neutral, and surprise. I trained and tested the models on the Custom FER-2013 dataset. The lower accuracy observed with my dataset is likely due to the limitations caused by the insufficient number of training and testing images. I believe the model’s accuracy could be significantly improved with a larger and more diverse dataset for training.

Training and Validation Accuracy

* Final **Train** Accuracy: 77.67%  
* **Validation** Accuracy: 76.92%

It’s not a bug, it’s an undocumented feature. Happy coding\!

