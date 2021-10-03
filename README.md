# URL_classifier

As part of a personnal project, i worked on a URL classifier to detect malicious and non malicious URL with different type of methods algorithms.

The dataset used is composed of 549 346 values divided into 2 features, "URL" which represent the text of the URL and "Label" which define the type of the URL (good or bad).

This project is divided in 3 python notebooks where we developped 3 differents methods :

- Machine Learning with Scikit-learn :
  - Cleaning : Balance label to have equal bad and good URLs and reduce our dataset to 40 000 values
  - Pre-Processing : Remove non alphabetical character -> tokenize each word or sequence of character -> stem each token -> find importance in each token with BoW methods.
  - Training : Use of Logistic Regression and Multinomial Naïves Bayes algorithms for training.

- Deep Learning (Neural Network) with TensorFlow :
  - Cleaning : Balance label to have equal bad and good URLs and reduce our dataset to 40 000 values.
  - Pre-processing : Two parralel processing 
    - Dividing each URL into domain, subdomain, domain suffix.
    - Giving for each character an ID that will create for each urls a sequence of number representing each character of the url
  - Training : Use of a parralel CNN structure with the two differents dataset given by the two preprocessing methods.

- Machine Learning with Spark :
  - The cleaning, pre-processing and training methods are the same as the Machine Learning with Scikit-learn version.


RESULTS :

- Machine Learning with Scikit-learn : 
  -> Logistic Regression :
  -> Multinomial Naïve Bayes :
  
- Deep Learning with Tensorflow :
  -> CNN : 
  
- Machine Learning with Spark :
  -> Cleaning and pre-processing efficient but i didn't managed to pass the training step yet.
  


