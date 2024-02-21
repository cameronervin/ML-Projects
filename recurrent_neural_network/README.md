# Recurrent Neural Networks - Book Review Classification
 
## About this Project

The goal of this project is to use Deep Learning and Artificial Intelligence techniques to create a multi-class classification model using varied recurrent neural network architectures that can accurately predict the genre of a book based off corpus text pulled from book reviews. 
 
## Dataset & Dependencies

Our dataset comes from the following CSV files: 'mental_health_bad_user_reviews.csv', 'mental_health_good_user_reviews.csv', 'specialized_diets_bad_user_reviews.csv', 'specialized_diets_good_user_reviews.csv', 'sports_and_outdoors_bad_user_reviews.csv', 'sports_and_outdoors_good_user_reviews.csv', 'christianity_bad_user_reviews.csv', 'christianity_good_user_reviews.csv'. 

We use the following Python/JupyterNotebook libraries in our work: 
* TensorFlow and Keras to create our model architecture.
* Scikit-learn for model evaluation and data processing.
* Seaborn and Matplotlib for data visualization.
* Other essential libraries include NumPy, Pandas, and TensorFlow.

 
## Technical Approach

First, we engineer our features by combining and cleaning up our dataset for our analysis. Next, we run exploratory data analysis to better understand our data before modeling. Then, we load in GloVe as our pretrained embedding. From here, we create different RNN architectures using LSTM and GRU layers, and we compare the performance of our models on our validation data. Our GRU model performs the best, so we then added a second chain to our best performing GRU model. We also explore the use of a hybrid GRU and LSTM model. Again, we analyze the performance of our models and plot this comparison graphically. Finally, we compare the performance of our GloVe pre-trained embedding to a ConceptNet Numberbatch pre-trained embedding.
 
## Highlights

* EDA
* Feature Engineering
* Recurrent Neural Networks
* Pre-trained embedding
* GloVe, ConceptNet Numberbatch
 
## Conclusion

One interesting result from the Conceptnet Numberbatch evaluation metrics is how it does not overfit the data like most of our other models do. Actually, at times Conceptnet Numberbatch can underfit the training data. As for the comparison with our GloVe pre-trained embedding layer, the two perform about the same. It is hard to say which performs the best since their validation f2 metric scores are so similar.


We found that, surprisingly, our hybrid CNN-RNN model had the best performance with a validation F2 score of   0.7809. As we previously mentioned, hybrid CNN-RNN models capture sequential and local patterns. This makes hybrid models a reasonable and common approach for text classification.

