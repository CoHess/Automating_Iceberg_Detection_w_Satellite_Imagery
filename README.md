# Automating_Iceberg_Detection_w_Satellite_Imagery
The project was for a Kaggle competition sponsored by C-Core and Statoil. The aim of the project was to classify satellite SAR images as either ships or icebergs. The identification by satellite is necessary for the protection of offshore instillations in areas like Iceberg Alley off of Newfoundland, Canada.

For the project I trained convolution neural networks with a semi supervised learning technique to improve results. Here is a summary of the Jupyter Notebooks:
1. Data Preprocessing and EDA – Processing SAR dataset into an RGB composite image that can be input to a CNN
2. VGG16 First Pass – VGG16 model training, including dropout and data augmentation
3. Pseudo Labeling – Semi supervised pseudo labeling technique is used to expand the size of the training set by labeling the current test set with highest confidence labels
4. Model predict pseudo labeled – retrained VGG16 architecture using larger Pseudo labeled dataset. Resulted in a 15% uplift in model performance in Kaggle competition

Powerpoint explaining project and methodology is also attached.
