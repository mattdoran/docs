# Calibration

Boil 3 liters of water with 1kg of sugar to begin with.  
  
Use a hydrometer to water out and creating solutions **1.050**, **1.040**, **1.030**, **1.020**, **1.010** and last clean water **1.000**.  
  
Configure the iSpindel to report every 60 seconds in to Brewfather, from the devices page you can then read the current value every minute. Starting out with reading the angle in SG 1.000 and if needed adjusting the weight to give a start angle of around 25 degrees.  
  
After reading out all angles in the different solutions and recording them. Fill in the values in the calibration spreadsheet for the iSpindel project and it will calculate the formula based on your unit.   
  
Copy the formula into your Polynominal under Configuration and start reading out the values in the different solutions again. **Make sure to use the formula that reports in Plato**. Brewfather then converts it into the unit you have choosen in the settings. If the gravity is displaying 1.004 in Brewfather you are using the wrong formula.

If you are using Plato in Brewfather for the SG solutions above you should see values close to 0, 2.5, 5, 7.5, 10 and 12.5 Plato matching the correct SG.

#### Resources

Excel calibration sheet: [https://github.com/universam1/iSpindel/blob/master/docs/Kalibrierung\_en.xlsm](https://github.com/universam1/iSpindel/blob/master/docs/Kalibrierung_en.xlsm)

More info: [https://github.com/universam1/iSpindel/blob/master/docs/Calibration\_en.md\#formula](https://github.com/universam1/iSpindel/blob/master/docs/Calibration_en.md#formula)  
  


