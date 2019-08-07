# TensorFlow Data Validation & Pre-Processing w/ Apache Beam

[![Tensorflow](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT7b9ZDD7lMdkByT-f_RCAqSQYqnq_CpgD16IFrwfmUwWCmdt7H)](https://www.tensorflow.org/beta/guide/effective_tf2)

[![TensorFlow Extended](https://storage.googleapis.com/gweb-cloudblog-publish/images/tensorflow.max-2200x2200.png)]
(https://www.tensorflow.org/tfx/guide/tft)

[![Colab](https://camo.githubusercontent.com/52feade06f2fecbf006889a904d221e6a730c194/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/github/JohnAntonusMaximus/TensorFlow-Preprocessing-Apache-Beam/blob/master/Data_Validation_w_Tensorflow_Transform_%26_Pre_Processing_w_Apache_Beam_2_0.ipynb)

## Background

TensorFlow Data Validation (TFDV) helps developers understand, validate, and monitor their ML data at scale. TFDV is used to analyze and validate petabytes of data at Google every day, and has a proven track record in helping TFX users maintain the health of their ML pipelines.

When applying machine learning to real world datasets, a lot of effort is required to preprocess data into a suitable format. This includes converting between formats, tokenizing and stemming text and forming vocabularies, and performing a variety of numerical operations such as normalization. You can do it all with tf.Transform which utilizes Apache Beam for data pre-processing.

Detailed developer documentation on TensorFlow Extended:
https://www.tensorflow.org/tfx

						

## Approach

In this Python 2.0 notebook, we're using a CSV that has data about air quality in Belgrade. Using TensorFlow Data Validation, we can infer a schema that can be used for future new datasets to maintain the integrity of data being fed into the model. We also make a copy of the data and drop a column to show anomalies, as well as make two different environments (one for Training the other for Serving) which gives us flexibility with our schema for our Target (we're trying to predict "soot" in the air, given so2, no2, and pm10). 

Later on, we create metadata for our schema which can be used with Apache Beam to perform data pre-processing transformations via tf.Transform. 


# Links

* [KaizenTek](http://www.kaizentek.io) - IT Consulting & Cloud Professional Services 
