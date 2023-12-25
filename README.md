# arabic-alpha-cnn-project
This Python script is a deep learning project for classifying Arabic alphabet characters using a Convolutional Neural Network (CNN). 

<body>
    <h1>Arabic Letters Classification Project</h1>

 <h2>Overview</h2>
    <p>The "Arabic Letters Classification Project" involves the classification of Arabic letters using machine learning
        techniques. The project utilizes Convolutional Neural Networks (CNN) to analyze and classify images of Arabic
        letters into distinct categories.</p>

<h2>Contents</h2>
    <ol>
        <li><strong>Libraries Used</strong>
            <pre>
                <code>
                    import numpy as np
                    import pandas as pd
                    import matplotlib.pyplot as plt
                    import seaborn as sns
                    import tensorflow as tf
                    from keras.models import Sequential
                    from keras.layers import Conv2D, MaxPooling2D, Flatten, Dense, Activation, Dropout, BatchNormalization
                    from sklearn.model_selection import train_test_split
                    from sklearn.metrics import accuracy_score, precision_score, recall_score, confusion_matrix, roc_curve, roc_auc_score
                    from keras.preprocessing.image import ImageDataGenerator
                    import cv2
                    import os
                    from tqdm import tqdm
                </code>
            </pre>
        </li>
        <li><strong>Machine Learning Model</strong>
            <p>The project employs a Convolutional Neural Network (CNN) for the classification task. The CNN is built using
                the Keras library with TensorFlow as the backend.</p>
            <pre>
                <code>
                    model = Sequential()
                    model.add(Conv2D(filters=32, kernel_size=(5, 5), padding='Same', activation='relu', input_shape=(64, 64, 3)))
                    model.add(MaxPooling2D(pool_size=(2, 2)))
                    <!-- Add more layers as needed -->
                    model.add(Dense(65, activation="softmax"))
                </code>
            </pre>
        </li>
      
            
 <h2>Model Performance</h2>
    <p>The trained model demonstrated excellent performance, achieving an accuracy of 88.9% for both the validation and test
        images. This high accuracy indicates the model's effectiveness in accurately classifying Arabic letters.</p>




