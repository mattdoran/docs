# Water

![Enter your water report values as ppm \(mg/l\)](../.gitbook/assets/image%20%2811%29.png)

## Water Report Conversion

Brewfather uses ppm values for the water profile, so your water report have to be converted to this. Below you will find help converting your values to ppm.

1 **mg/L** = 1 ppm

From **Alkalinity mmol/l** to ppm Bicarbonate HCO3: **multiply by 61**  
From **Alkalinity mg/l CaCO3** to ppm Bicarbonate HCO3: **multiply by 1.22**  
_From Alkalinity mmol/l to mg/l CaCO3: multiply by 50_  
  
1000 **ug/L** = 1 ppm  
**ug/L** / 1000 = ppm

### Ion Conversion

Calcium as **CaCO3** ppm \* 0.401 = **Calcium \(Ca\)** ppm  
Magnesium as **CaCO3** ppm \* 0.243 = **Magnesium \(Mg\)** ppm  
Sulfate as Sulfur ppm as **SO4-S** \* 3 = **Sulfate \(SO4\)** ppm  
Bicarbonate as **CaCO3** ppm \* 1.22 = **Bicarbonate \(HCO3\)** ppm  
  
US Hardness _grains/gallon_ \* **6.86** = **Calcium \(Ca\)** ppm  
°Clark / °e \(English\) Hardness _grain/imp gallon_ \* **5.71** = **Calcium \(Ca\)** ppm  
German Hardness \(°dH, deutsche Härte\) \* **7.14** = **Calcium \(Ca\)** ppm  
Calcium Hardness mEq/L or mval \* **20** = **Calcium \(Ca\)** ppm  
  
Karbonate Hardness dKH \* **21.8** = **Bicarbonate \(HCO3\)** ppm  
**Alkalinity mEq/L** or mval \* **61** = **Bicarbonate \(HCO3\)** ppm  
  
_Minor Ions \(Currently not in use\)_  
_Carbonate as **CaCO3 ppm** \* 0.6 = Carbonate \(CO3\) ppm  
Nitrate as Nitrogen **ppm as NO3-N** \* 4.43 = Nitrate \(NO3\) ppm_

### pH

If the water report does not inlcude the pH you can use 8.0 as pH.

{% page-ref page="../recipes/water-calculator.md" %}

