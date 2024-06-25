# MRI_denoising
Deep learning pipeline to denoise T1-weighted low-field MRI acquisitions.
This repo contains the pipeline used to generate the results supporting the conclusions in our manuscript titled __________________________ DOI:

Overview of repo pipeline:
![image](https://github.com/erz-7/MRI_denoising/assets/74198413/27505be6-1ab8-4c2f-b114-327ae47467c3)


### Data availability
In this article, we used three publicly available MRI datasets:

1. IXI dataset - 1.5T/3T cerebellar MR acquisitions (UK): http://brain-development.org/ixi-dataset/

2. FastMRI dataset (T1w images only) - 1.5T/3T cerebellar + genicular acquisitions (USA): https://fastmri.med.nyu.edu/

3. M4Raw dataset (T1w images only) - 0.3T cerebellar acquisitions (CN): https://zenodo.org/records/8056074

Access to these datasets may need to be requested from the initial authors via e-mail correspondence.

### Preprocessing
To preprocess the data, we provide an automated pipeline that does the following:

1. Determines the file format of the input data (DICOM/h5/NIFTI formats currently supported)

2. Z-score normalizes each patient image to itself to uniformize the dataset

3. Re-organizes the dataset as to create a single contiguous 3D array containing each slice within the dataset, which is then saved as a .pt tensor file for model import.

### Analysis
The file ____ contains our model and training loop for generating our results at the click of a button:

1. 

2.

3.
