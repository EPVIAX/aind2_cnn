aind2-cnn
Instructions

Clone the repository and navigate to the downloaded folder.

	git clone https://github.com/udacity/aind2-cnn.git
cd aind2-cnn

(Optional) If you plan to install TensorFlow with GPU support on your local machine, follow the guide to install the necessary NVIDIA software on your system. If you are using an EC2 GPU instance, you can skip this step.

(Optional) If you are running the project on your local machine (and not using AWS), create (and activate) a new environment.

    Linux (to install with GPU support, change requirements/dog-linux.yml to requirements/dog-linux-gpu.yml):

conda env create -f requirements/dog-linux.yml
source activate dog-project

    Mac (to install with GPU support, change requirements/dog-mac.yml to requirements/dog-mac-gpu.yml):

conda env create -f requirements/dog-mac.yml
source activate dog-project

    Windows (to install with GPU support, change requirements/dog-windows.yml to requirements/dog-windows-gpu.yml):

conda env create -f requirements/dog-windows.yml
activate dog-project

(Optional) If you are running the project on your local machine (and not using AWS) and Step 6 throws errors, try this alternative step to create your environment.

    Linux or Mac (to install with GPU support, change requirements/requirements.txt to requirements/requirements-gpu.txt):

conda create --name dog-project python=3.5
source activate dog-project
pip install -r requirements/requirements.txt

    Windows (to install with GPU support, change requirements/requirements.txt to requirements/requirements-gpu.txt):

conda create --name dog-project python=3.5
activate dog-project
pip install -r requirements/requirements.txt

    (Optional) If you are using AWS, install Tensorflow.

sudo python3 -m pip install -r requirements/requirements-gpu.txt

Switch Keras backend to TensorFlow.

    Linux or Mac:

     KERAS_BACKEND=tensorflow python -c "from keras import backend"

Windows:

 set KERAS_BACKEND=tensorflow
 python -c "from keras import backend"

    (Optional) If you are running the project on your local machine (and not using AWS), create an IPython kernel for the dog-project environment.

python -m ipykernel install --user --name dog-project --display-name "dog-project"

    Launch Jupyter notebook.

jupyter notebook

    (Optional) If you are running the project on your local machine (and not using AWS), before running code, change the kernel to match the dog-project environment by using the drop-down menu (Kernel > Change kernel > dog-project).

