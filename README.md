# Object-Detection-with-YOLO
Implementing YOLO for object detection from scratch

Virtual environment Creation with Mamba:
1. Install Mmaba from here
https://github.com/conda-forge/miniforge#mambaforge

2. mamba create --name yolo_venv python=3.6
create a virtual environment "yolo_venv" with python version 3.6

3. mamba activate yolo_venv
activate the environment

4. pip install -r requirements.txt
for installing dependencies

5. mamba env export > requirements.yaml
for exporting dependencies

4. mamba env create -f requirements.yaml
for using the requirement file in cross platform (from another pc)

5. mamba deactivate yolo_venv
deactivate the environment


**Creating Model**
Information about architecture config:
Tuple is structured by (kernel_size, filters, stride, padding) 
"M" is simply maxpooling with stride 2x2 and kernel 2x2
List is structured by tuples and lastly int with number of repeats