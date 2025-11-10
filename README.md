# Instructions to run code in Powershell from your project folder:

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
.\.venv\Scripts\Activate
## If you haven’t trained since switching to Coverage A:
python .\train_and_serialize.py --csv .\simulated_home_insurance_quotes.csv
## Fit calibration if you created calib_samples.csv and calibration_fit.py:
python .\calibration_fit.py  
python .\app.py  
