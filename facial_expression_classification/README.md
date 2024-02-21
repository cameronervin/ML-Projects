# Convolutional Network Architecture - Facial Expression Classification

## About this Project

The goal of this project is to use Deep Learning and Artificial Intelligence techniques to create a computer vision model that can accurately detect facial emotions. The model should be able to perform multi-class classification on images of facial expressions, to classify the expressions according to the associated emotion.

## Dataset & Dependencies

Our dataset is from MIT's Applied Data Science Program. 

We use the following Python/JupyterNotebook libraries in our work: 
• TensorFlow and Keras to create our model architecture.  
• Scikit-learn for model evaluation and data processing.
• Seaborn and Matplotlib for data visualization.
• Other essential libraries include NumPy, Pandas, and TensorFlow.

## Technical Approach

First, we perform exploratory data analysis (EDA) by checking the distributions of our classes. After understanding the breakdown of our data, we then build our base model using a standard multi-layer perceptron in TensorFlow. Then, we experiment with building seven custom convolutional neural networks in TensorFlow, and we compare the performance of all of our models using our validation data. Next, we also compare the performance of our custom models with models using transfer learning. We create further models using VGG16, ResNet, and EfficientNet. Again, we compare the performance of our transfer learning models with our previous models. Finally, we create a more robust CNN model and analyze the performance of all of our models.

## Highlights

• EDA
• Convolutional Neural Networks
• Multi-Layer Perceptron
• Transfer Learning
• Model Analysis

## Conclusion

• We are going ahead with our final model, i.e, model3. The earlier models have a very less number of trainable parameters.
• We also tried out a few Transfer Learning architectures. But we realized that we couldn't use 'grayscale' color mode with those architectures. And as per our analysis, 'rgb' color mode was giving really poor results when we used 3 input channel images with our Deep Learning Architectures.
• Thus we had to come up with our complex CNN architecture that has a comparable number of trainable parameters to our Transfer Learning Architectures and works with single channel (or 'grayscale') inputs. This final model had 5 Convolutional blocks, with each Conv2D layer having a significantly higher number of filters than all its predecessors.
• As expected, our final model gives us higher accuracies over validation and test data than all the other models.
• The model has consistent values over training, testing, and validation accuracies, suggesting that there is no overfitting.

