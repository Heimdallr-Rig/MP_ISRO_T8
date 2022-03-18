#  Project Heimdall
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Contents
- [Overview](#overview)
- [Installation](#installation)
- [Local Setup](#local-setup)
- [Demo](#demo)


## Overview
**Project Heimdall** is a stand-alone web-based application using <a href="https://streamlit.io/">Streamlit.io</a> to identify and categorize X-ray bursts. 

Submission for the Inter-IIT Tech Meet's Mid Prep event: ISRO'S Web-Based Automatic Identifiaction Of Solar Bursts In X-Ray Light Curves 

Team: **MP_ISRO_T8**

Visit ### Visit our deployed webapp <a href="https://project-isro-heimdall.herokuapp.com/">here</a> <br/>


## Installation
### Prerequistes
An active internet connection is required to run the application, unless you build the application from source. In order to build application from source, click [here](#local-setup)
### Windows
1. Download and unzip the zip file from [here](https://drive.google.com/drive/folders/1v8izoqzm3gI1KHPVqUfHHnEvnoVlucB-?usp=sharing)
2. Once unzipped, click on ```Heimdall.exe``` to launch the application

### MacOS
1. Download and unzip the zip file from [here](https://drive.google.com/drive/folders/1VRQUN0qGjYclX9AZX_Rz_RxKy6Ln_iyK?usp=sharing)
2. Once unzipped, click on ```Heimdall.app``` to launch the application

### Linux and it's various distributions
1. Download and unzip the zip file from [here](https://drive.google.com/drive/folders/1VRQUN0qGjYclX9AZX_Rz_RxKy6Ln_iyK?usp=sharing)
2. Once unzipped, run the following command to cd into the dirctory using the terminal 
```bash
cd Heimdall-linux-x64
```
3. Then run the following command to run the binary 
```bash
./Heimdall
```

## Local Setup
### Prerequistes
1. Python3

### Setup
1. Clone the repository using
```bash
git clone https://github.com/Heimdallr-Rig/MP_ISRO_T8.git

```

2. Create a virtual environment, using:
```bash
virtualenv venv
```
3. Activate the virtual environment using:
```bash
source venv/bin/activate
```
4. Install dependecies using the following command
```bash
pip install -r requirements.txt
```
5. Run the app using
```bash
streamlit run app.py
```
6. On successfull deployment you should get the following output. Click on the Local URL to open the application in your browser
```
  You can now view your Streamlit app in your browser.

  Local URL: http://localhost:8501
  Network URL: http://xx.xx.xx.xx:8501
```

## Demo 

Once the app is up and running , you'll be welcomed with a very simple welcome screen with an upload option. 
We support the following file extensions:
``` lc, csv, ascii, txt, xls, xlsv, xlsm, xlsb, odf, odt ```

The files are then extracted for data using a pretty neat library called <a href="https://www.astropy.org/">Astropy</a>. This data is then further processed using various methods and processed. A brief in

![image](https://user-images.githubusercontent.com/59011370/159001786-a3c85b1b-b82e-4317-ae21-148c4ece3fe4.png)

Once done, we get the following output.

In order to get the following input we used the ```ch2_xsm_20211111_v1_level2.lc``` file under the ```data``` directory [here](https://github.com/Heimdallr-Rig/MP_ISRO_T8/tree/main/data)

### Section 1: Raw Data Input
Here we visualize the data with a graph to plot the raw data before any proccessing
![raw_data_input](https://user-images.githubusercontent.com/59011370/158999454-13fde19d-3b5b-4be6-8877-76d1abff66cd.png)

### Section 2: Data After Noise Reduction
We then
![noise_red](https://user-images.githubusercontent.com/59011370/158999452-a927a40c-22ad-4e4e-9872-ee4201182e23.png)
![peaks](https://user-images.githubusercontent.com/59011370/158999453-2d0488c5-ab69-4e1d-81a4-25b22c6cb0c8.png)
![analysis](https://user-images.githubusercontent.com/59011370/158999445-1166537e-afde-4dc5-9ce4-ede61d576e1b.png)

## Why use our app?

Our web app has some beautiful dynamic graphs that are interactive, means draggable and scrollable. It also display coordinates on hovering, making the analysis very easy. <br/>
![gif](https://user-images.githubusercontent.com/59011370/159001213-2f3d8976-0ce8-4bea-abb7-5f154fbe6bdd.gif)
<br/>

