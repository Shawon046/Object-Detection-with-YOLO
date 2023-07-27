# Object-Detection-with-YOLO
Implementing YOLO for object detection from scratch

Virtual environment Creation with Mamba: <br>
1. Install Mmaba from here <br>
https://github.com/conda-forge/miniforge#mambaforge

2. mamba create --name yolo_venv python=3.6 <br>
create a virtual environment "yolo_venv" with python version 3.6

3. mamba activate yolo_venv <br>
activate the environment

4. pip install -r requirements.txt <br>
for installing dependencies

5. mamba env export > requirements.yaml <br>
for exporting dependencies

4. mamba env create -f requirements.yaml <br>
for using the requirement file in cross platform (from another pc)

5. mamba deactivate yolo_venv <br>
deactivate the environment


**Creating Model** <br>
Information about architecture config: <br>
Tuple is structured by (kernel_size, filters, stride, padding) <br>
"M" is simply maxpooling with stride 2x2 and kernel 2x2 <br>
List is structured by tuples and lastly int with number of repeats <br>

**Loss Function** <br>
Regression loss for center, dimension, and class probability <br>

**VOC Dataset Loader** <br>
Custom Dataset loader for VOC <br>
The implementation restrict to ONE object per cell 