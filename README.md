# Small Animal and Ex Vivo Diffusion
Code, software, and datasets for small animal and ex vivo diffusion MRI

Here, we compile  a list of existing and freely shared [small-animal datasets](#small-animal-datasets) or [ex vivo diffusion datasets](#ex-vivo-datasets), a list  of available software dedicated to [image acquisition](#data-acquisition), a list of software  available for [data pre-processing](#pre-processing), and a list of software available for [model fitting](#model-fitting). 

This project is associated with two works on preclinical diffusion MRI:

(1) Recommendations and guidelines from the ISMRM Diffusion Study Group for preclinical diffusion MRI: 
Part 1 — In vivo small-animal imaging

(2) Recommendations and guidelines from the ISMRM Diffusion Study Group for preclinical diffusion MRI: 
Part 2 — Ex vivo imaging


## Small Animal Datasets

| URL  | Species | Diffusion Scheme | Other features | Institution |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| https://doi.org/10.14264/de9aa47  | Mouse brain  | DTI | Model of Concussion | University of Queensland
| http://cmrm.med.jhmi.edu/ (M. Aggarwal et al. 2009)  | Mouse brain  | Atlas | Johns Hopkins
| https://mouse.brain-map.org/static/atlas  | Mouse | Allen Mouse brain atlas (not diffusion MRI, but histology dataset) | full-color, high-resolution anatomic reference atlas accompanied by a systematic, hierarchically organized taxonomy of mouse brain structures | Allen Institute |
| https://scalablebrainatlas.incf.org/macaque/MERetal14_on_F99  | Macaque | F99 macaque (not diffusion, histology tracer based dataset) | 91 cortical regions atlas, registered to F99 space | Stem cell and Brain Research Institute, Université de Lyon, University of Yale |
| https://openneuro.org/datasets/ds004441 (see https://doi.org/10.1016/j.neuroimage.2020.117498 & http://doi.org/10.1002/mrm.29495) | Rat brain | Multi-shell | Model of sporadic Alzheimer's disease, longitudinal datasets | EPFL |

## Ex Vivo Datasets

| URL  | Species | Diffusion Scheme | Other features | Institution |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| http://www.drcmr.dk/map-datasets  | Mouse brain  | micro-FA, Multi-shell, multi-resolution, Tractography, Axon diameter, Exchange rate, Axon relaxation | Validation: 3D synchrotron imaging of axons, cell bodies, vacoules and vessels, in vivo tracers | Danish Research Center for MR
| https://www.nature.com/articles/sdata201672 | Rat brain, rat spinal cord, human brain | DKI |  | Aarhus University |
| https://doi.org/10.1016/j.dib.2016.08.020 | Rat, pig and human spinal cords | DTI | Ultra-high resolution (MR microscopy) | U of Florida |
| https://doi.org/10.1016/j.dib.2016.06.061 | Rat brain | Multi-shell, high b-value | Mild chronic stress model | Aarhus University |
| https://github.com/sepehrband/AxonDiameter | Mouse brain | Multi-shell  | Augmented with EM data and manually segmented axon diameter | U of Queensland |
| http://cmrm.med.jhmi.edu/ (M. Aggarwal et al. 2009) | Adult and postnatal developing mouse brains |  | Atlas | Johns Hopkins |
| https://doi.org/10.1016/j.neuroscience.2005.07.014  | Mouse brain |  | Atlas | Several |
| http://doc.pmod.com/pneuro/pneuro.html?mousebrainatlasma-benveniste-mirrione4996.html | Cynomolgus, rhesus monkey and pig  |  | Atlas  | PMOD |
| https://osf.io/yp4qg/ (Cohen-Adad et al. 2019)  | White matter axons |  | Microscopy data (non-MR) | Several |
| https://doi.org/10.1016/j.dib.2015.05.019 |Cynomolgus macaque corpus callosum  |  | Microscopy data (non-MR) | Several |
| http://www.duhs.duke.edu/mouseconnectome | Mouse Connectome in Waxholm Space | HARDI @ 43 um, 120 angle, b-value @ 4000 s/mm2 | Segmented Atlas compared to retroviral tracers WHS Labels | Duke CIVM |
| https://civmvoxport.vm.duke.edu/voxbase/login.php?return_url=%2Fvoxbase%2Fstudyhome.php%3Fstudyid%3D754 | Rat Connectome | MGRE @ 25 um HARDI @ 50 um 60 Angles Single specimen Average (n=6)b=3000 s/mm2 |Segmented Atlas includes downloadable application for display | Duke CIVM |
| http://www.civm.duhs.duke.edu/rhesusatlas |Rhesus | MGRE@75um DTI@150 um 12 angles; b value =1500 s/mm2  | Average N=10 241 labels  | Duke CIVM |
| https://civmvoxport.vm.duke.edu/voxbase/login.php?return_url=%2Fvoxbase%2F | Mouse NODDI @ 50 um | 8 shells B value 1000-8000 s/mm2 384 angles |With comparative histology | Duke CIVM |
| Histology: https://www.nitrc.org/projects/smatlas/ Atlas: https://www.nitrc.org/projects/validate29/ | Squirrel monkey atlas + histology | Multi-shell HARDI acquisition | Atlas + histology | Vanderbilt |
| https://civmvoxport.vm.duke.edu/voxbase/login.php?return_url=%2Fvoxbase%2F https://www.sciencedirect.com/science/article/pii/S1053811920303621  | Mouse brain | 25um and 67um isotropic at b=4000 s/mm2 | diffusion + QSM data | Duke University |
| https://www.nitrc.org/projects/rat_dmri_atlas https://www.sciencedirect.com/science/article/pii/S1053811921007436 | Rat Brain | 61 DWIs, b=3000s/mm2 | Three sets of data: a single specimen at 25 um and 50um; an average specimen at 50um; WHS3.0 data in affine alignment to Paxinos Watson(7th edition) orientation | Duke University |
| [Digital Brain Bank](https://open.win.ox.ac.uk/DigitalBrainBank/#/) Paper:https://elifesciences.org/articles/73153 | Human, Macaque | HARDI & Multi-shell | Human datasets for neuroanatomy and neuropathology investigations (including whole brain diffusion MRI) + nonhuman species covering multiple taxonomic ranks | Oxford University |


## Data acquisition

| Name  | URL | Institution | Features | Dependencies |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Pulse Sequences | https://osf.io/ngu4a/   | University of Wisconsin  Madison | Custom diffusion sequences (for Bruker Consoles) | ParaVision version
| REMMI | https://remmi-toolbox.github.io/  | Vanderbilt University | Sequences for small animal quantitative MRI including diffusion | Paravision or VNMRJversion
| double PFG directions | [https://cfin.au.dk/cfin-labs-research-groups/neurophysics/software](https://cfin.au.dk/cfinmindlab-labs-research-groups/neurophysics/software/)  | Aarhus University | Output pairs of diffusion directions for dPFG | Matlab
| q-space sampling resources  | [https://github.com/ecaruyer/qspace](https://github.com/ecaruyer/qspace) http://www.emmanuelcaruyer.com/q-space-sampling.php | Univ Rennes, Inria, CNRS, IRISA | Tools for sampling and reconstruction in q-space diffusion MRI | N/A |

## Pre-processing

| Name  | URL | Institution | Features | Dependencies |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| DICOMIFIER  | https://github.com/lamyj/dicomifier  | University of Strasbourg | Conversion Bruker to DCM and NIFTI format (incl. Diffusion information) | Python
| atlasBREX  | https://github.com/jlohmeier/atlasBREX  | Charité Berlin | Non-human brain extraction | FSL, AFNI, ANTs, ABSORB
| PreQual  | https://github.com/MASILab/PreQual  | Vanderbilt | All pre-processing steps | Python
| SCT  | https://spinalcordtoolbox.com/   | Polytechnique Montreal | Spinal cord MRI | Python
| MChepato  | https://github.com/fragrussu/MChepato | Vall d’Hebron Institute of Oncology | Tools for mouse liver dMRI-histology imaging used in (Grussu et al. 2022) | Python, FSL, QuPath, MRItools, DiPy, NiftyReg, and others
| Tractoflow  | https://doi.org/10.1016/j.neuroimage.2020.116889 | Sherbrooke University | End to end tractography (not small animal specific) | 
| dwigradcheck  | https://mrtrix.readthedocs.io/en/latest/reference/commands/dwigradcheck.html | MRtrix3 software | Check the orientation of the diffusion gradient table; Jeurissen et al., MIA, 2014 | MRtrix3 |
| dwi2mask  | https://mrtrix.readthedocs.io/en/dev/reference/commands/dwi2mask.html | MRtrix3 software | Generate a binary mask from DWI data using a variety of algorithms | MRtrix3 |
| scil_validate_and_correct_bvec  | https://github.com/scilus/scilpy/blob/master/scripts/scil_validate_and_correct_bvecs.py | SCILPY (Shrebrooke) | Detect sign flips and/or axes swaps in the gradients table from a fiber coherence index (Schilling et al, MRI, 2019) | scilpy |
| dwidenoise  | https://mrtrix.readthedocs.io/en/latest/reference/commands/dwidenoise.html | MRtrix3 software | dMRI noise level estimation and denoising using Marchenko-Pastur PCA (Veraart et al., NI, 2016) | MRtrix3 |
| Koay's Inversion Method for Rician Bias correction  | https://github.com/jan-martin-mri/koays-inversion | National Institutes of Health | This GitHub repository contains MATLAB code for correcting noisy MRI data for Rician bias according to Koay's inversion method | Koay's inversion method to correct data for Rician bias requires a corresponding noise map |
| DESIGNER (Diffusion parameter EStImation with Gibbs and NoisE Removal)  | (https://github.com/NYU-DiffusionMRI/DESIGNER) | NYU | mage-processing pipeline for (diffusion) MRI data that has been developed to identify and correct various specific artifacts and confounding factors for an improved accuracy, precision, and robustness in diffusion MRI analysis | Python, but requires the installation of Matlab, MRtrix, and FSL |
| Signal Drift correction for dMRI data (Vos method)  | https://www.mathworks.com/matlabcentral/fileexchange/55008-signal-drift-correction-for-diffusion-mri-data | UCL | Function to correct for signal drift in diffusion-weighted MRI data as described in Vos et al., MRM 2016; also available in ExploreDTI (www.exploredti.com) | N/A |

## Model Fitting
| Name  | URL | Models | Features | Dependencies |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| qMRINet  | https://github.com/fragrussu/qMRINet  | qMRI models | model fitting using fully-connected deep neural networks | NumPy/Nibabel/SciPy/PyTorch
| Fast Kurtosis  | https://cfin.au.dk/cfinmindlab-labs-research-groups/neurophysics/software/  | Kurtosis metrics | kurtosis metrics from reduced diffusion kurtosis imaging data sets | Matlab
| WMTI-Watson  | https://github.com/Mic-map/WMTI-Watson_DL | White Matter Standard Model | Estimated directly from DKI parameters, based on DL | python |

