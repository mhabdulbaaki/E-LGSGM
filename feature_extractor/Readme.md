# Visual Feature Extraction

This directory contains code to extract visual features from the flickr30k dataset.

Create a virtual environment and install the packages using in the requirements.txt file

To extract the features, download the flickr30k dataset from here.

Place the images in an appropriate location and the change the location path in the extract_visual_features.py file.

Our data is original given by the SGM paper where some basic cleaning process were performed to remove duplicated data and lowering text. The preprocessed data can be found in the Data folder. Download it [here](https://drive.google.com/file/d/1e9ko0xnKEDl-OQ36So5Wq11zSPlimK_2/view?usp=sharing)

The model also need the visual features which are the embedded vector of objects in images. In this research, we used ConvNext (tiny) to extract the features. You can extract by running extract_visual_features.py script. The extracted features will be in the folders VisualObjectFeatures_b5 and VisualPredFeatures_b5 directories in the data folder.

After extracting the visual features, kindly move the data folder into the LGSGM directory where it can be used for training.

If you only want to evaluate our pretrained model, you only need to download the preprocessed data from the same link above. no need to extract visual features from the flickr dataset.