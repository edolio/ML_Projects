# ML_Projects
This is a repo containing various projects developed for educational purposes on various AI/ML topics

## LogisticRegression
Project that uses multinomial logistic regression to classify satellitary images (5631 images 64x64 taken from https://github.com/RealGoldenGeneral/mini-project-5) of 4 classes (cloudy, desert, green, water). Validation is performed with Stratified K-fold with 3 splits. Regularization hyperparameter is calibrated using a grid validation. <br>Conlusions:
- Model suffers a bit of poor generalization capabilites for specific classes: cloudy and desert class are easily distinguishable while green and water gets often confused one for the other of the times. Specific image preprocessing for those classes could be required.
- Poor test accuracy is due to lost info from image patterns and colors features (Logistic regression only consists in a fully connected layer). Results with CNN would surely be better another faster solution could be PCA.
