"""
Sickle Cell Classification with CNN
-----------------------------------

This project is focused on classifying sickle cell blood images using deep learning. I used a convolutional neural network (CNN) to detect whether sickle cells were present in microscopic images. The dataset came from the Teso region in Uganda, and it includes labeled sickle cell images, unlabeled positive images, and clear negative images. I chose not to use the unclear images to keep the model training on higher quality data.

The CNN was built using several Conv2D and MaxPooling2D layers followed by Dense layers for the final classification. I used ImageDataGenerator for rescaling and organizing the input images. The model was trained over 30 epochs. The training accuracy kept going up, reaching 1.00, but after a certain point the validation accuracy started dropping a bit. That told me the model might be overfitting a little.

Final results:
- Training Accuracy: 1.00
- Validation Accuracy: 0.96

Given the size of the dataset, I’m actually okay with those numbers. If I had more balanced or expanded data, it might generalize better. Later on, I plan to try dropout, early stopping, and more data augmentation to help reduce the overfitting.

This is just the start of applying ML to real-world medical problems, and I’m looking forward to building on this project.
"""
