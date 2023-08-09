# Brain Segmentation    

This repository contains a deep learning based project made to train several architectures for MRI fetal brain masking performance.

It's updated so it works with TensorFlow2.

Some of the tested architectures are:

- **Unet**
- Unet + Grid Attention Gate
- Unet + Filter Attention Gate
- UNet + Regularization
- Unet + Grid Attention Gate + Regularization
- Mask RCNN
- FCN vgg19 backbone

In our tests, U-Net showed the best overall performance. Thus, it was used to train our model. You can find the GitHub repo for it [here](https://github.com/sofia-urosa/brain-masking.git).

## Requirements</b>
- tqdm
- opencv
- nibabel
- MedPy
- Keras
- TensorFlow
- Scikit-image

### Download the tool

Clone the source code, cd into your desired location

```python
(env_name)$ git clone GIT
(env_name)$ cd brain_segmentation
(env_name)$ git checkout tf2
```

Install requirements from requirements.txt

```python
(env_name)$ pip install -r requirements.txt
```

### Running the project

<br>Before running the project you will have to access the "data" folder and add the images and masks in "test" and "train" folders. A discussion about splitting methods is outside of the scope of this README, but you can try whatever you think is best. There are no strict rules on how to do this, but a good starting point can be using the 80/20 rule.

You can find files to help you with the splitting inside of ``data/split``. </br>

<br>Finally you're ready to train:</br>

```python
python train.py --exp name_of_the_training
```

or using k-fold cross-validation:

```python
python kfold.py --exp name_of_the_training
```

<br>If you don't chose a name_of_the_training or you pick an existing one the tool will show an error message.</br>
<br>You will have to activate the environment every time you want to run the tool.</br>

## Setup

You can create a new virtual environment using the `venv` command:

```python
python -m venv /path/env_name
```
    
This will create a virtual environment called `env_name` in the directory `/path`.
To activate it, run:

```python
source /path/env_name/bin/activate
```

The environments name should appear at the beginnig of the shell surrounded by parentheses, like this:

```python
(env_name)$
```
    
For further information on how virtual envirionments work, check the [python documentation](https://docs.python.org/3/library/venv.html).
    

