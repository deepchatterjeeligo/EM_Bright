# EM_Bright
This repository contains the tools required for the "EM-Bright analysis" of LIGO-Virgo gravitational wave triggers. You will need LValert tools and pycbc installation to run the EM-Bright analysis.


*** Subscribe to the cbc_gstlal node ***
lvalert_admin --user <user.name> --password <your password> --subscribe --node cbc_gstlal

*** Start listening ***
lvalert_listen --user <user.name> --password <your password> -c /home/shaon/analysis/o2/EM_Bright_classification/auto_EM_Bright/myLVAlertListen.ini -r alertInstance & 

Notes: 

1. Need PyCBC installation 

2. Make sure your lalsuite installation is later than 23rd June.


3. Before running make sure the paths are correct in the two ini files (configFile.ini and myLVAlertListen.ini). Also make sure that the paths are correct in lvalert-run_cbc_gstlal_lowmass.sh. Change mode for lvalert-run_cbc_gstlal_lowmass.sh to 777.

4. Sample run command:

lvalert_listen --user shaon.ghosh  --netrc /home/shaon/.netrc -c /home/shaon/ANALYSIS/EM_Bright/myLVAlertListen.ini  -r alertInstance &

*** Patrick's Change ***
