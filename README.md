# Small Animal and Ex Vivo Diffusion
Code, software, and datasets for small animal and ex vivo diffusion MRI

Here, we compile  a list of existing and freely shared small-animl or ex vivo diffusion datasets (**Table 1 and Table 2**), a list  of available software dedicated to image acquisition (**Table 3**), a list of software  available for data pre-processing (**Table 4**), and a list of software available for model fitting (**Table 5**). 

Citation of paper goes here


## Small Animal Datasets

| URL  | Species | Diffusion Scheme | Other features | Institution |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| https://doi.org/10.14264/de9aa47  | Mouse brain  | DTI | Model of Concussion | University of Queensland
| http://cmrm.med.jhmi.edu/ (M. Aggarwal et al. 2009)  | Mouse brain  | Atlas | Johns Hopkins

## Ex Vivo Datasets

| URL  | Species | Diffusion Scheme | Other features | Institution |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| https://doi.org/10.14264/de9aa47  | Mouse brain  | DTI | Model of Concussion | University of Queensland
| http://cmrm.med.jhmi.edu/ (M. Aggarwal et al. 2009)  | Content Cell  |

## Data acquisition

| Name  | URL | Institution | Features | Dependencies |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Pulse Sequences | https://osf.io/ngu4a/   | University of Wisconsin  Madison | Custom diffusion sequences (for Bruker Consoles) | ParaVision version

## Pre-processing

| Name  | URL | Institution | Features | Dependencies |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| DICOMIFIER  | https://github.com/lamyj/dicomifier  | University of Strasbourg | Conversion Bruker to DCM and NIFTI format (incl. Diffusion information) | Python

## Model Fitting
| Name  | URL | Models | Features | Dependencies |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| sMRINet  | https://github.com/fragrussu/qMRINet  | qMRI models | model fitting using fully-connected deep neural networks | NumPy/Nibabel/SciPy/PyTorch

