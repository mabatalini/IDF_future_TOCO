# IDF_future_TOCO

in EQM_downscaling you will find:
- The functions to format the PROJETA data (the csv files containing the projected historical and future data, downloaded directly from the PROJETA website).
- The functions to perform the EQM downscaling method.

in bias_correction you will find:
- The functions to perform the quantile mapping bias correction
- The functions to perform the daily bias correction
- The functions to format the files obtained from CMhyid to power transformation and mapping distribution bias correction

in error_calculation you will find the functions to calculate the error of the IDF calculated with projected corrected data.

in idf_generator_subdaily you will find the functions to calculate the IDF based on subdaily data (table and coefficients)
- To calculate the IDF we use the equation i = K.RP^m/(t + t0)^n. I think is different from the eq. Karisma is using. We will need to choose just one for our work.

FOLDERS TO CREATE
You will need to create the following folders:
- PROJETA -> It must contain the files dowloaded directly from projeta website (this are the csv files that I have shared with you)
- GCM_data -> The code will save the formatted csv files in this folder
- CMhyd -> Where we will save the data obtained from CMhyd
- Results -> It must contain the historical observed data in the formats that I shared with you.



!!! NEW INFO:
Use the transform_daily_data to calculate the subdaily max.
The "fatores_desagregacao.csv" contain the disagreggation factors for the Sao Paulo state. This file should be in the main directory where you are running the code (not inside any folder).
I put one file "INMET_conv_daily" as an example of how is the input file. I believe you already have the observed data like this. One important note is that in the code this file is inside the "Results" folder. You can change this as you want!!
