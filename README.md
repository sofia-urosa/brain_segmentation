# Brain Segmentation    

This is a deep learning based project to segmentate brains of fetuses of MRI.

## Requirements</b>
- Python3
- pip

## Installation</b>

For an easy use of the project is highly recommended to create a virtual environment and install the dependencies found in the requirements.txt file.

- ### Setting a virtual environment

<br>Access to your terminal and type the following:</br>
<br><code>$ pip install virtualenv virtualenvwrapper</code></br>
<br>Then create a directory for the virtual environments:</br>
<br><code>$ mkdir ~/python-envs </code>  
<br>Now you'll add to your .bashrc file these two lines:</br>
<br><code>$ export WORKON_HOME=~python-envs</code></br>
<br><code>$ source /usr/share/virtualenvwrapper/virtualenvwrapper.sh</code></br>
<i><br>(If this path to virtualenvwrapper.sh doesn't work, try with:)</br></i>
<br><code>$ /usr/share/virtualenvwrapper/virtualenvwrapper.sh</code></br>
<br>Now you're ready to source your .bashrc and create a Python3 environment:</br>
<br><code>$ source .bashrc</code></br>
<br><code>$ mkvirtualenv --python=python3 python_env</code></br>
<br><code>$ workon python_env</code></br>
<br><i>(Note that "python_env" is a suggested name, you can replace it with any desired name for your environment)</i></br>
<br>And finally when you're done working you can deactivate the environment with:</br>
<br><code>$ deactivate</code></br>

- ### Running the project

Once you're in your own environment access to the desired location and type the following commands:
<br><code>$ git clone https://github.com/chrisorozco1097/brain_segmentation.git</code></br>
<br><code>$ cd brain_segmentation</code></br>
<br>Now install the requirements</br>
<br><code>$ pip install -r requirements.txt</code></br>
<br>Before running the project you will have to access the "data" folder and add the images and masks in the "test" and "train" folders. It's recommended to divide the total amount of images in 80% train, 20% test.</br>
<br>Finally you're ready to execute the project:</br>
<br><code>$ python train.py --exp name_of_the_training</code></br>
<br>If you don't chose a name_of_the_training or you pick an existing one the tool will show an error message</br>
<br>You will have to activate the environment every time you want to run the tool.</br>
