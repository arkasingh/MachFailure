# Machine Failure Detection
This is a comparative analysis of Machine Learning and Deep Learning approach on working with data with high class imbalance.  The domain chosen here is to predict "Machine Failure" leading to successful Predictive Preventive Maintenance

The Dataset is taken from [UCI-Machine Learning Depository](https://archive.ics.uci.edu/ml/datasets/AI4I+2020+Predictive+Maintenance+Dataset#)

The original credit : Stephan Matzka, School of Engineering - Technology and Life, Hochschule fÃ¼r Technik und Wirtschaft Berlin, 12459 Berlin, Germany, stephan.matzka'@'htw-berlin.de

The dataset [*ai4i2020.csv*](https://github.com/arkasingh/MachFailure/blob/main/ai4i2020.csv) consists of 10,000 data points stored as rows with 14 features in columns.

### Methods Deployed to handle the Class Imbalance

1. Under Sampling
2. Over Sampling
3. Machine Learning - Synthetic Minority Oversampling Technique (SMOTE)
4. Deep Learning - Generative Adversarial Network (GAN)

### Methods Deployed to solve Predictive Preventive Maintenance

1. Machine Learning - Linear Support Vector Machine (SVM)
2. Deep Learning - Multi Layer Perceptron (MLP)

### Model Weights

The GAN architecture consists of 2 networks - Generator and Discriminator. The training weights for the same are given in the files [*gan_discriminator_model.h5*](https://github.com/arkasingh/MachFailure/blob/main/gan_discriminator_model.h5) & [*gan_generator_model.h5*](https://github.com/arkasingh/MachFailure/blob/main/gan_generator_model.h5). The fineal GAN model weights are [*gan_final_model.h5*](https://github.com/arkasingh/MachFailure/blob/main/gan_final_model.h5).

The MLP network weights trained with the GAN samples can be found in the file [*mlp_gan_model.h5*](https://github.com/arkasingh/MachFailure/blob/main/mlp_gan_model.h5)

### Results and Conclusions
*Classification Results with Support Vector Machine*

<img src="https://user-images.githubusercontent.com/110922376/210347487-2c64a7c0-71bb-4a1b-81d5-398b4e06c65d.png" width="343" height="201">

*Classification Results with Multi layer Perceptron*

<img src="https://user-images.githubusercontent.com/110922376/210347565-0230e68f-2d0a-47ad-be2f-3889afb7b4d8.png" width="343" height="201">


*MLP classified better than SVM*

*MLP performed best when trained with unsampled imbalanced data*

*Considering all the metrics (recall, precision , f1-score), GAN proved to be the best sampling method*
