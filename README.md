# Project Setup Guide 

This guide provides a structured approach to setting up your project environment on Windows, covering the installation of essential dependencies like FFmpeg and PortAudio. Additionally, it walks through the creation of a Python virtual environment using various methods such as Pipenv, pip, and Conda.

## Table of Contents

1. [Installing FFmpeg and PortAudio](#installing-ffmpeg-and-portaudio)
2. [Setting Up a Python Virtual Environment](#setting-up-a-python-virtual-environment)
   - [Using Pipenv](#using-pipenv)
   - [Using pip and venv](#using-pip-and-venv)
   - [Using Conda](#using-conda)
3. [Running the Application](#running-the-application)

---

## Installing FFmpeg and PortAudio

### Installing FFmpeg
1. Download the latest static build from [FFmpeg’s official website](https://ffmpeg.org/download.html).
2. Extract the ZIP file to a directory, e.g., `C:\ffmpeg`.
3. Add `C:\ffmpeg\bin` to the system PATH via the Environment Variables settings.

### Installing PortAudio
1. Download PortAudio binaries from [PortAudio’s website](http://www.portaudio.com/download.html).
2. Follow the installation instructions provided on the site.

---

## Setting Up a Python Virtual Environment

### Using Pipenv

1. **Install Pipenv:**
   ```bash
   pip install pipenv
   ```
2. **Install Dependencies:**
   ```bash
   pipenv install
   ```
3. **Activate the Environment:**
   ```bash
   pipenv shell
   ```

---

### Using pip and venv

1. **Create a Virtual Environment:**
   ```bash
   python -m venv venv
   ```
2. **Activate the Environment:**
   ```bash
   venv\Scripts\activate
   ```
3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

---

### Using Conda

1. **Create a New Conda Environment:**
   ```bash
   conda create --name myenv python=3.11
   ```
2. **Activate the Environment:**
   ```bash
   conda activate myenv
   ```
3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

---

## Running the Application

### Phase 1: Initialize the Core Logic
```bash
python brain_of_the_doctor.py
```

### Phase 2: Process Patient's Voice Input
```bash
python voice_of_the_patient.py
```

### Phase 3: Generate Doctor's Response
```bash
python voice_of_the_doctor.py
```

### Phase 4: Launch the User Interface with Gradio
```bash
python gradio_app.py
```

