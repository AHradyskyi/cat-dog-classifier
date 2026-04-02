# Cat-dog classifier
This small program checks whether the provided image is a Cat or a Dog.

The project consists of two parts: training the model and using the results for the GUI program.

## Training the model

The learning dataset was taken from this [Kaggle page](https://www.kaggle.com/datasets/bhavikjikadara/dog-and-cat-classification-dataset). The original data contains 12.5k images in both categories. Due to a lack of resources, it was reduced to 1.2k images.

We now have two classes, each with 1,000 training images and 200 validation images. After that, the VGG19 pretrained model was used.
The result of training could be seen in this table:
|| accuracy | loss | val_accuracy | val_loss | learning_rate |
| --- | --- | -------- | --- | -------- | -------- |
| 55  | 1.0 | 0.000165 | 1.0 |	0.000680 |	1.000000e-06 |
| 56  | 1.0 | 0.000514 | 1.0 | 0.000041 | 1.000000e-06 |
| 57  | 1.0 | 0.000558 | 1.0 | 0.000100 | 1.000000e-06 |
| 58  | 1.0 | 0.000126 | 1.0 | 0.0000040 | 1.000000e-06 |
| 59  | 1.0 | 0.000309 | 1.0 | 0.0000150 | 1.000000e-06 |

 The graphs show the accuracy and learning rate for this model
 ![text](https://github.com/AHradyskyi/cat-dog-classifier/blob/main/graphs.png?raw=true)

 ## GUI
The Graphical User Interface is a small window that asks the user to load the image. The result shows how precisely the model detects whether it is a cat or a dog.
