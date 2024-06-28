# MRI_denoising

This repo contains a Deep learning pipeline to denoise T1-weighted low-field MRI acquisitions. The pipeline used to generate the results supporting the conclusions in our manuscript titled "DenoiseNET: a generalizable approach to denoising low-field cerebellar MR acquisitions". This project can be reproduced by downloading the public data as described below and running our code with a single "run all" command.
(DOI: coming soon!) 

Requirements:
- Python 3.11.7
- Pip install requirements.txt
- Cuda
- Windows (Unix coming soon, or you can just edit lines with directory paths)

### Overview of repo pipeline:
![Screenshot 2024-06-28 102622](https://github.com/erz-7/MRI_denoising/assets/74198413/17194216-360c-4dfe-8599-fa68fffaffaf)

### Data availability
In this article, we used three publicly available MRI datasets:

1. IXI dataset - 1.5T/3T cerebellar MR acquisitions (UK): http://brain-development.org/ixi-dataset/

2. FastMRI dataset (T1w images only) - 1.5T/3T cerebellar + genicular acquisitions (USA): https://fastmri.med.nyu.edu/

3. M4Raw dataset (T1w images only) - 0.3T cerebellar acquisitions (CN): https://zenodo.org/records/8056074

Access to these datasets may need to be requested from the initial authors via e-mail correspondence.
To re-produce our results, downlaod these three datasets and store them in separate folders.
project_folder/
├── IXI/
├── FastMRI/
└── M4Raw/


### Preprocessing
To preprocess the data, we provide an automated pipeline that does the following:

1. Determines the file format of the input data (DICOM/h5/NIFTI formats currently supported)

2. Z-score normalizes each 2D slide to homogenize the dataset

3. Re-organizes the dataset as to create a single contiguous 3D array containing each slice within the dataset, which is then saved as a .pt tensor file for model import.


### Analysis
The file ____ contains our model and training loop for generating our results at the click of a button:

1. 

2.

3.

### Network architecture

![Picture1](https://github.com/erz-7/MRI_denoising/assets/74198413/fe8ad133-8c51-4d90-99b9-b978c901d646)
