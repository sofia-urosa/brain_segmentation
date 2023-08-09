# Brain Segmentation    

This repository contains a deep learning based project made to train several architectures for MRI fetal brain masking performance.

It's updated so it works with TensorFlow2.

Some of the tested architectures are:

Unet


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

<br>Before running the project you will have to access the "data" folder and add the images and masks in the "test" and "train" folders. It's recommended to divide the total amount of images in 80% train, 20% test.</br>
<br>Finally you're ready to execute the project:</br>

```python
python train.py --exp name_of_the_training
```
<br>If you don't chose a name_of_the_training or you pick an existing one the tool will show an error message</br>
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
    

