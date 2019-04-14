# Plant Seedling Identification

### Training Data

Training set and Test set contains thousands of images of plant seedlings at various stages of grown. Each image has a filename that is its unique id. The dataset comprises 12 plant species. The goal is to create a classifier capable of determining a plant's species from a photo. The list of species is as follows:

* Black-grass
* Charlock
* Cleavers
* Common Chickweed
* Common wheat
* Fat Hen
* Loose Silky-bent
* Maize
* Scentless Mayweed
* Shepherds Purse
* Small-flowered Cranesbill
* Sugar beet

### Approach

My Solution to the problem is to use transfer learning on [VGG16](https://arxiv.org/abs/1409.1556) architecture by replacing the classifier module of standard VGG16 to generate 12 class probabilities and finetuning the pretrained weights to learn patterns required to classify plant seedlings. In order to make model robust in identifying plant seedling data augmentation techniques like blur, rotate, flip were also used.

### Evaluation Metric

[MeanFScore](https://en.wikipedia.org/wiki/F1_score)


### Results

Solution has an accuracy of 91.813%.