# Fuzzy-radiomics
fuzzy radiomics GUI can help extract conventional radiomics, fuzzy mask-based radiomic features, and shrunk mask and extended mask for comparison.

# Environmental requirements
MATLAB R2023b in Windows

# How to use it
1. doble click the `FuRAD.exe` and wait a few moment at the first time.
2. Set the data files' path DATA FILE FOLDER and output path OUTPUT FOLDER.

   In `DATA FILE FOLDER`, it should contain patients' folders with the image and mask in it. Following is a templet. You can choose to enter the full path of the Data directly in the text field, or you can click `Data path` botton and select the folder where the data is located.

```bash
    DATA FILE FOLDER/
    ├── Patient001
    │   │── ImageCT.mha
    │   └── MaskGTVn.mha
    └── Patient002
        │── ImageCT.mha
        └── MaskGTVn.mha
```

   In `OUTPUT FOLDER`, it contains folders for each modules. The output files for each patient are in their own folder. Following is a templet. You can choose to enter the full path of the Output file directly in the text field, or you can click `Output path` and select the appropriate folder to save the output.

```bash
    OUTPUT FOLDER/
    ├── extractionStatus.csv
    ├── radiomicsFeaturesAllPatients_Bin.csv
    └── radiomicsFeaturesAllPatients_FuzzyMask.csv
```

4. Set the data file form
   The data file could be either `.mha` or `.dicom`. Please choose it correctly.
5. Set the image file templet and mask file templet
   We need to know the names of the patient image and mask files (e.g., image file: `ImageCT.mha`, mask file: `MaskGTVn.mha`). This can be entered directly in the text field, or you can click on the previous button to directly select a patient's data and mask files, respectively.
6. Select feature extraction modules according to your demonds.
7. Set hyperparameters. Drag the slider to set the parameters. **For the fuzzy mask, the larger the parameter, the higher the fuzzy degree.**
8. Click the `Start` botton to extract features. The runing information will be displayed in the bottom text field.

If you have any questions or comments, please email us at gene-jin.cao@connect.polyu.hk
