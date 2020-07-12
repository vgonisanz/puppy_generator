# space_invaders_generator

This is a concept art to generate pixel puppies automatically using Tensorflow.

## Developing

Invoke `make develop`, now you can execute any script.

## Datasets

In order to train models, we have created a dataset called `cherry`. This dataset contain folders. 

Each folder have the info about a sample of a space invader puppy:

* `${IMAGE_ID}.png`: The puppy png, it can have any width and height.
* `metadata.yaml`: The metadata that describe how the puppy is. This will be the input to generate new puppies.

### Metadata

The metadata is the input of the IA. It have the following elements:

* ...