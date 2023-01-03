# MachFailure
This is a comparative analysis of Machine Learning and Deep Learning approach on working with data with high class imbalance.  The domain chosen here is to predict "Machine Failure" leading to successful Predictive Preventive Maintenance

The Dataset is taken from UCI-Machine Learning Depository
https://archive.ics.uci.edu/ml/datasets/AI4I+2020+Predictive+Maintenance+Dataset#

The original credit : Stephan Matzka, School of Engineering - Technology and Life, Hochschule fÃ¼r Technik und Wirtschaft Berlin, 12459 Berlin, Germany, stephan.matzka'@'htw-berlin.de

The dataset *ai4i2020.csv* consists of 10,000 data points stored as rows with 14 features in columns.

Methods Deployed to handle Class Imbalance:

1. Under Sampling
2. Over Sampling
3. Synthetic Minority Oversampling Technique (SMOTE)
4. Generative Adversarial Network (GAN)

Methods Deployed to solve Predictive Preventive Maintenance:

1. Machine Learning (Linear SVM)
2. Deep Learning (Multi Layer Perceptron - MLP)

The GAN architecture consists of 2 networks - Generator and Discriminator. The training weights for the same are given in the files *gan_discriminator_model.h5* & [*gan_generator_model.h5*](https://github.com/arkasingh/MachFailure/blob/main/gan_generator_model.h5)
