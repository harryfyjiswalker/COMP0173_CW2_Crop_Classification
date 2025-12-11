# COMP0173_CW2_Crop_Classification

This repository contains my work for COMP0173 CW2.

[00_COMP0173_Write_Up](00_COMP0173_Write_Up.pdf) details the;
  - Replication of Baseline Model
  - Contextualisation of crop classification, sustainability analysis and ethical considerations
  - Ppreprocessing, modelling, and hyperparameter tuning methodologies
  - Ablation studies
  - Analysis of results
  - References for both write-up and poster
________________

The code is available at [COMP0173_Crop_Classiciation](COMP0173_Crop_Classification.ipynb), produced in Google Colab. To reproduce the results:
1. Create a Google Drive folder entitled 'COMP0173_Applying_New_Context' in your main drive; within this, create a folder entitled 'data' (this will match the data path to that used in the code: DATA_PATH = '/content/drive/MyDrive/COMP0173_Applying_New_Context/data'). The code for mounting the drive is available in the .ipynb file.
2. Run code cell 1 (!pip install breizhcrops)
3. Due to an unresolvable compatibility issue, the datasets must then be downloaded in the following way:
   - In code cell 2, change "dataset = bzh.BreizhCrops("frh03", level="L2A")" to "dataset = bzh.BreizhCrops("frh01", level="L2A")". Run this cell.
   - In code cell 3, change "REGIONS_TO_EXTRACT: List[str] = ["frh04"]" to "REGIONS_TO_EXTRACT: List[str] = ["frh01"]" and run this cell to locally download (X_raw_frh01.npy and y_raw_frh01.npy)
   - Repeat this process for frh02, frh03, and frh04. You should now have files named X_raw_frh0X.npy and y_raw_frh0X.npy for X=1,2,3,4 locally downloaded; if not, please change the names to this form.
   - Upload all files to the "data" folder in your Google Drive.
   - Mount Google Drive using code cell 4, and run code cell 5 to confirm the following output:

Listing files in: /content/drive/MyDrive/COMP0173_Applying_New_Context/data
\ny_raw_frh01.npy
\ny_raw_frh02.npy
\nX_raw_frh02.npy
\nX_raw_frh01.npy
\ny_raw_frh04.npy
\nX_raw_frh04.npy
\nX_raw_frh03.npy
\ny_raw_frh03.npy

The remmainder of the .ipynb file will now be reproducible.

________________

Code documenting my reproduction of the initial baseline is available at [COMP0173_Baseline_Replication](COMP0173_Baseline_Replication.ipynb); instructions for replication of this code is included in the .ipynb file.

________________

The poster summary of this coursework is available for download at [COMP0173 Final Coursework 2 Poster.pptx](https://github.com/harryfyjiswalker/COMP0173_CW2_Crop_Classification/blob/main/COMP0173%20Final%20Coursework%202%20Poster.pptx).




  
