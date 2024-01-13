This folder contains the plate reader data used to plot growth of strains expressing sfGFP under the control of YTK promoters. 

Every '.xlsx' file contiains the raw data, with the timepoint of each reading indicated in the file name. 
The layout of the 96-well plate can be found in the '...layout.csv' file. Within this file, the promoter for each strain is indicated below:
896 = pTDH3
897 = pCCW12
898 = pPGK1
899 = pHHF2
900 = pTEF1
901 = pTEF2
902 = pHHF1
903 = pHTB2
904 = pRPL18B
905 = pALD6
906 = pPAB1
907 = pRET2
908 = pRNR1
909 = pSAC6
910 = pRNR2
911 = pPOP6
912 = pRAD27
913 = pPSP2
914 = pREV1

In the platecurver script, the 'plater' package is used to match sample names in the layout.csv file and OD600 readings in the .xlsx files. Then a series of functions are used to plot the blank-corrected values. 

'tidy_new.csv' contains the non blank-corrected OD600 readings for all of the samples at different time points. It can be generated from the platecurver script.

In the '...metrics' folder:
The plots produced by the platecurver script can be found here. PDFs named '311020...' were generated and used to monitor growth curves in real time during the experiment.
The plots named 'plate...' have been produced after fitting a sigmoidal curve to the blank-corrected OD600 values, at the end of the experiment, using the growthcurver package. The growthcurver package also calculates growth metrics like doubling time, time to midlog etc. (https://cran.r-project.org/web/packages/growthcurver/vignettes/Growthcurver-vignette.html). 
The metrics for promoters in specific media conditions has been saved in the corresponding .xlsx files in this folder too. 
ypdx = YPD 10% glucose media
ypd = YPD media
sm = YNB media
yepg/yepgminus = YEPG media


