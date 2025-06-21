# Computer_Vision
## *This was a Computer Vision project for TripleTen. 👩🏽‍💻*
This project was developed for Good Seed, a supermarket chain seeking to enhance compliance with alcohol sales laws by using computer vision to estimate customer age at the point of sale. The goal was to build a model that can automatically flag customers who may be underage, prompting a manual ID check while avoiding unnecessary interruptions for clearly eligible customers.

To accomplish this, the project applies convolutional neural networks (CNNs) to a dataset of facial images labeled with individuals’ real ages. A regression model was developed using the ResNet50 architecture and the Adam optimizer, outputting a single nonnegative value representing the predicted age of each subject.

After training for 17 epochs, the model achieved its best performance with a mean absolute error (MAE) of 6.642 and loss of 3.221 on the validation set. While training metrics continued to improve, validation performance plateaued—indicating overfitting, and suggesting that early stopping would yield the most reliable predictions.

Although the model is not accurate enough to fully automate age verification, it meets Good Seed’s accuracy threshold of ±8 years, making it well-suited as a screening tool. For example, it could flag customers whose predicted age falls within ±7 years of the legal threshold for alcohol or tobacco, prompting staff to request ID only when appropriate.

🔍 Potential Future Enhancements:

* Expanding the training dataset—particularly with more samples from individuals aged 10–30—could improve accuracy and generalizability.
* Restricting the dataset to likely consumers (e.g., 10+ years) could reduce bias and improve efficiency.
* Repurposing the model for non-regulatory use cases like age-based marketing segmentation or restricted product recommendations.<br>

This project demonstrates the potential of applied computer vision to streamline retail operations and enhance compliance.
## Skills Highlighted
👀 Computer Vision
📸 Image Classification in Python
🔗 Fully Connected & Convolutional Neural Networks
🍰 Multilayer Network Training
🥅 LeNet & ResNet Architecture
👨🏽 Adam Algorithm
➕ Augmentations
📚 Keras Library
## Installation & Usage
* This project uses pandas, tensorflow, matplotlib.pyplot, and numpy.  It requires python 3.11.7.
