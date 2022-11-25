# Classic ML vs CNN vs Transfer Learning
**Notebook&amp;Report** of a **face recognition classification task** of a similar charateristics data set comparing performace three ways of achieving it:

* A *classic machine learning classificator*
* A *convolitional neural network* builted from scratch 
* A *transfer learning* aproach replacing *dense layers* of a pre-trained CNN

## Dataset
Used a modified olivetti dataset. It is a set of face images taken between April 1992 and April 1994 at AT&amp;T Laboratories Cambridge. The particularity of this dataset is that images **were closeup photos with similar lighting and pose**. 

## Results

Because of the similarity of the images, the Classic ML has outstandig results, proven that classic ML is still a good option for this kind of tasks, deppending on the dataset.

Type | Model | Accuracy | F-score 
---|---|---|---
Classic ML | SVM with PCA | 0.9625 | 0.96
Deep Learning | custom CNN | 0.95 | 0.9475
Transfer Learning | VGG16 + new layers | 0.9625 | 0.96

Despite being an image classification job with few data, classic machine learning turned out to be a fast and light alternative, especially due to the reduction of the dimensionality from 4096 to 471. The CNN model was also a good alternative, but it was more complex and time consuming to train, and it was not as accurate as the classic ML model. The transfer learning model was accurate as the classic ML model, but it was more complex and time consuming to train.

