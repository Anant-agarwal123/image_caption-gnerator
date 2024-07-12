# Image Caption Generator

### Objective:
To develop an image caption generator that can automatically generate descriptive captions for a diverse set of images using a CNN-encoder and LSTM-decoder architecture.

### Background:
The project was initiated to explore the intersection of computer vision and natural language processing, aiming to create a model that can understand and describe the content of an image. This capability can be applied in various domains such as accessibility, content creation, object detection, image indexing and many more.

### Technologies Used:
**Languages:** Python
**Frameworks and Libraries:** 
+ **TensorFlow and Keras:** For data preprocessing and model creation.
+ **OpenCV:** For image preprocessing

**CNN Architecture:** MobileNet for feature extraction

**RNN Architecture:** Long Short-Term Memory (LSTM) for sequence generation

### Process:
+ Data Collection: Utilized a dataset of over 8000 diverse images.
+ Image Preprocessing: Applied various image preprocessing techniques such as resizing and normalization to prepare the images for feature extraction.
+ Feature Extraction: Used MobileNet, a lightweight and efficient convolutional neural network, to extract high-level features from the images.
+ Text Preprocessing: Processed the image captions by removig numerals and special symbols, tokenizing and creating a vocabulary dictionary. Converted the text data into sequences that the LSTM model could understand.
+ Model Design: Designed a CNN-encoder and LSTM-decoder architecture. The encoder (MobileNet) extracted features from images, while the decoder (LSTM) generated captions based on these features.
+ Training: Fed the processed image features and text data into the model. Trained the LSTM model through multiple iterations, experimenting with various model architectures and hyperparameters.
+ Evaluation: Evaluated the model using the BLEU (Bilingual Evaluation Understudy) score, achieving a score of 0.6 after several iterations and optimizations.

### Challenges:
+ Handling the diversity and complexity of the dataset.
+ Handling multiple captions for same image.
+ Balancing the model's performance and computational efficiency.
+ Reducing validation loss faster and efficiently.
+ Achieving a satisfactory BLEU score through model tuning and experimentation.


### Outcome:
Successfully developed an image caption generator model with a BLEU score of 0.6. The model can generate coherent and relevant captions for a wide range of images, demonstrating the effective integration of computer vision and natural language processing techniques.

### Future Plans:
+ Improving the BLEU Score of model.
+ Deploying the model as a web application.
+ To add a voice generator mechanism which audibly calls out the generated caption.


### Learnings:
+ Gained in-depth knowledge of CNNs and RNNs, particularly LSTM networks.
+ Learned the importance of preprocessing in handling diverse datasets.
+ Improved skills in model evaluation and performance tuning.
