Acoustical Command Recognition (FFT Approach)
Author: Syed Murtuza Quadri
Project: Sensor Signal Processing (SSP SS25)

Project Overview
This project implements a complete pipeline for an acoustical command recognition system. The system is designed to recognize spoken voice commands ('up', 'down', 'left', 'right', 'stop') and use them to control an interactive application. The core of this submission is a single Jupyter Notebook that demonstrates the entire workflow for the FFT-based approach (Task 1.a).

System Requirements
Python Version: 3.13.0

Operating System: Tested on Windows 11 and Linux (Ubuntu/Debian).

File Structure
Acoustical Command Recognition SSP SS25 (1.a FFT).ipynb: The main Jupyter Notebook containing all code for data processing, model training, evaluation, and the live demo.

requirements.txt: A list of all necessary Python libraries.

README.md: This setup and instruction file.

/recordings/: The development dataset (350 .wav files).

/TEST/: The hidden test dataset (250 .wav files).

Setup Instructions (for Linux)
1. Create & Activate Virtual Environment

Navigate to the project directory and run the following commands in your terminal:

python3 -m venv env
source env/bin/activate

2. Install Dependencies

Install all required libraries using pip.

pip install -r requirements.txt

Note on PyAudio: If the command above fails, PyAudio may require system dependencies. On Debian/Ubuntu, they can be installed with:

sudo apt-get update
sudo apt-get install portaudio19-dev python3-pyaudio

After installation, please run pip install -r requirements.txt again if necessary.

Setup Instructions (for Windows)
1. Create & Activate Virtual Environment

Open Command Prompt or PowerShell, navigate to the project directory, and run the following commands:

py -m venv env
.\env\Scripts\activate

2. Install Dependencies

Install all required Python libraries using the provided requirements.txt file.

pip install -r requirements.txt

IMPORTANT NOTE for PyAudio: PyAudio can be difficult to install on Windows with pip. If the command above fails with an error related to PyAudio or portaudio.h, the most reliable solution is to install it from a pre-compiled wheel file:

Go to the Unofficial Windows Binaries for Python Extension Packages page.

Download the PyAudio wheel (.whl) file that matches your Python version (e.g., PyAudio‑0.2.14‑cp313‑cp313‑win_amd64.whl for Python 3.13 on 64-bit Windows).

Open a terminal in the folder where you downloaded the file and install it directly with pip:

pip install PyAudio-0.2.14-cp313-cp313-win_amd64.whl

After PyAudio is successfully installed, run pip install -r requirements.txt again to install the remaining packages.

How to Run
1. Launch Jupyter Notebook

With your virtual environment still active ((env) should be in your prompt), start Jupyter Notebook:

jupyter notebook

2. Run the Notebook

In the browser, open the Acoustical Command Recognition SSP SS25 (1.a FFT).ipynb file. The cells are designed to be run sequentially from top to bottom.