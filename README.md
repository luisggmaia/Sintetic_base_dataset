# Sintetic base dataset

Implementation, for Convolutional Neural Network training, of computer vision transformations to produce labels corresponding to target bases in a synthetic images dataset - created from Blender.

### Files

Arena.blender: Arena modeled in Blender. For the wallpapers to be added, the .png files must be in the same directory as the .blender files. The arena had been updated to a more complete version.

Blender_v1.py: contains classes (and methods) useful for creating the dataset, in particular defined for the reference systems within which the transformations take place (camera and image).

Blender_v2.py: an update of Blender_v1.py. It takes into account the camera distortion furthest from the center of the camera in y-axis. This was done by considering the Kannala-Brandt model, in particular for $\delta$ f = f.

Dataset.py: effectively implements the creation of the dataset from Blender. It has also been updated to generate a most compatible output.

### Results

Some results are shown below. The first images correspond to the first version of the files. The rest, to the second.
Note the interesting distortion of the bounding boxes in the first version compared to the second.

![train_1](https://github.com/user-attachments/assets/0eb29701-cd28-4fdd-bbac-780ad6f08f01)

![train_2](https://github.com/user-attachments/assets/b2bc2309-126a-4ba3-aeff-d4dd3a832c9b)

![train_5](https://github.com/user-attachments/assets/fd9c7f7e-761d-4d66-883d-16bf05c5bc64)

![train_8](https://github.com/user-attachments/assets/43552b49-095d-421d-b027-60ebe3c90246)

![train_9](https://github.com/user-attachments/assets/59161948-21da-45bb-8f08-361818339f88)
