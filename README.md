# Dlib compiled binary wheels for Python 3.7 - 3.12 on Windows and x64 CPUs

This repository contains the compiled binary (.whl) files for the [Dlib](http://dlib.net/) library to install on Python versions 3.7, 3.8, 3.9, 3.10, 3.11, and 3.12 on a Windows x64 OS. 

## 📢 New Update:
* May 08, 2024: Added compiled binary file (.whl) for Python 3.12!

## Steps to install Dlib:

* Install Python from [Python.org](https://www.python.org/downloads/) (download the 64-bit installer file)
  
   **OR**
* Create a virtual environment via [venv](https://docs.python.org/3/library/venv.html) or [Anaconda](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) i.e. `conda create -n env_name python = 3.8` 
 
* Download the wheel file for your specific Python version 

* Open a terminal and install Dlib via:

### Python 3.7
```
python -m pip install dlib-19.22.99-cp37-cp37m-win_amd64.whl 
```
### Python 3.8
```
python -m pip install dlib-19.22.99-cp38-cp38-win_amd64.whl
```
### Python 3.9
```
python -m pip install dlib-19.22.99-cp39-cp39-win_amd64.whl
```
### Python 3.10
```
python -m pip install dlib-19.22.99-cp310-cp310-win_amd64.whl
```
### Python 3.11
```
python -m pip install dlib-19.24.1-cp311-cp311-win_amd64.whl
```
### Python 3.12
```
python -m pip install dlib-19.24.99-cp312-cp312-win_amd64.whl
```
## Steps to build Dlib from source:
If you'd like to build it from source, follow these exact steps as per their [docs](https://github.com/davisking/dlib?tab=readme-ov-file#compiling-dlib-python-api):
* Install [Visual Studio 2022](https://visualstudio.microsoft.com/vs/community/) with the option **Desktop Development with C++**
* Create a virtual env with [`venv`](https://docs.python.org/3/library/venv.html) or [anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)
* Execute these commands:
```
git clone https://github.com/davisking/dlib.git
cd dlib
pip install build
python -m build --wheel # Upon successful run, a ".whl" binary will be created under "dlib/dist/" 
pip install dist/dlib-<version>.whl # replace <version> with the exact name of the ".whl" file
``` 
Cheers!
