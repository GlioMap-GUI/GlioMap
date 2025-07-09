
GlioMap
=======

GlioMap is an open-source MATLAB-based graphical user interface (GUI) designed for brain tumor segmentation and feature extraction from MRI images. It offers an integrated workflow combining image preprocessing, skull stripping, tumor segmentation (semi-automated and manual), and the calculation of radiomic and morphological features — all within a user-friendly GUI.

Key Features
------------

- 2D MRI Visualization with slice-by-slice navigation and contrast adjustment.
- Preprocessing Tools including normalization and bias field correction.
- Skull Stripping using a simplified BET (Brain Extraction Tool) method.
- Segmentation using fuzzy FMC (Fuzzy Membership Clustering) or manual tools (drawing, ROI).
- Feature Extraction:
  - Over 100 IBSI-compliant radiomic features.
  - 33 morphological features related to shape and structure.
- Multi-format Image Support: NIfTI, DICOM, MHA, PNG, JPG, etc.

Interface Overview
------------------

GlioMap consists of four main interactive windows:

1. Main Window – Load images, preprocess, skull-strip, and adjust brightness/contrast.
2. Selected Slice Window – Navigate through MRI slices and select target slices.
3. Segmentation Window – Apply FMC or manual segmentation tools and save results.
4. Edit Mask Window – Generate masks, apply to other sequences, and extract features.

Requirements
------------

- MATLAB (R2020b or newer recommended)
- Image Processing Toolbox

Installation
------------

1. Clone the repository:
   git clone https://github.com/GlioMap-GUI/GlioMap.git

2. Open MATLAB and add the cloned folder to the MATLAB path:
   addpath(genpath('GlioMap'))

3. Launch GlioMap:
   "GlioMap.m"

or

1. Download all the files in repository as a zipfile

2. Extract zipfile

3. Run "Gliomap.m" file


User Manual
-----------

Detailed instructions and visual walkthroughs are available on the GlioMap Documentation Site:
https://gliomap-gui.github.io/index.html

Use Case Example
----------------

1. Load MRI sequence (.nii, .dcm, etc.)
2. Apply skull stripping to remove non-brain tissues.
3. Normalize and correct bias in image intensities.
4. Select slices containing tumor regions.
5. Apply FMC segmentation or manually draw ROIs.
6. Generate tumor masks.
7. Extract radiomic and morphological features.
8. Save outputs for clinical or research use.

Supported File Formats
----------------------

.nii, .nii.gz, .dcm, .mha, .mhd, .nrrd, .jpg, .png, .tif, etc.

Radiomic & Morphological Features
---------------------------------

- Radiomic feature definitions: https://gliomap-gui.github.io/radiomic.html
- Morphological feature definitions: https://gliomap-gui.github.io/morphological.html

Limitations
-----------

- Only supports 2D slice-by-slice visualization.
- Does not support 3D feature extraction (planned for future versions).

Developers
----------

- Isira Senanayaka – thilanga8.314@gmail.com
- T. Sangavi – tsangavi291@gmail.com
- Dr. Mohan Jayathilaka – jayatiml@gmail.com
- Prof. P.B. Hevavithana – padmabh@gmail.com
- Dr. Sunil Kulathunga - 

License
-------

This project is licensed under the MIT License.

GlioMap is developed as a non-commercial academic tool to support the radiology research community with a reproducible and lightweight image analysis platform.
