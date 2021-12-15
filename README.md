# Galaxy_Prediction
#  Introduction
Galaxies come in different shapes, sizes, and ages: from beautiful spirals (like our Milky Way) to huge ellipticals. To understand how these morphologies of galaxies relate to their underlying physics, galaxies morphologies classification is a crucial step. However, it is unlikely to manually classify millions of galaxies observed by modern sky surveys. Hence, our goal is to help astronomers automatically classify galaxies by building a machine learning model from analyzing manually classified galaxy images.
#  Dataset
The original data is from Galaxy zoo data.
The total number of pictures is up to 60,000  RGB images with an original size of 424x424.
The galaxies are classified into 37 different categories
The values of labels in each class represent the probability from human classification.
#  DatasetMethodology and Results
## Data Pre-processing
To make the training more efficient and avoid the possible confusion from irrelevant edged objects, we decide to crop the image. The images are cropped from 424x424 pixels to central 130x130 pixels, and resized to 64x64 pixels for training.
## Model Performance
We use Root-Mean-Square Error as loss function to show model’s performance. We achieve almost 81% accuracy by using the ResNet 152 Model, which is including 515 layers, for 10 epochs with 0.0001 learning rate. The plot below show the RMSE loss of different neural network architectures.
