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

| Attribute          | type | values                                     |
|--------------------|------|--------------------------------------------|
| width              | int  | Number of pixels in the png width          |
| height             |      | Number of pixels the png height            |
| number_of_legs     | int  | 0 in example                               |
| number_of_arms     | int  | 0 in example                               |
| number_of_eyes     | int  | 0 in example                               |
| number_of_antennas | int  | 0 in example                               |
| number_of_horns    | int  | 0  in example                              |
| has_head           | bool | True in example                            |
| has_tail           | bool | True in example                            |
| is_symetric        | bool | True in example                            |
| side               | enum | It shall be front, left or right           |
| expression         | enum | It shall be happy, angry, zigzag or normal |