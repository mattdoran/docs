# Water Calculator

## Set up your Source water profile

Go to profiles in the main menu and select Water. Select the default source profile, and adjust the values to match your water report. For more info click the link below.

{% page-ref page="../profiles/water.md" %}

## Locate the water calculator

Normally you do not want to start adjusting your water until the rest of your recipe is done. When you have created your recipe and are ready to start adjusting your water you will find the water calculator in the water section of the recipe designer.

![Click the CALC button to open the water calculator](../.gitbook/assets/image%20%2819%29.png)

This will open the water calculator.

![](../.gitbook/assets/image%20%2879%29.png)

At the top you will see your current mash water room temperature pH. **All pH values should be measured when the wort is cooled down to room temperature**.

{% hint style="info" %}
_Temperature note:_ The measured pH will vary depending on what temperature you measure it at, and this is not an equipment shortcoming. Brewfather predicts the 20°C mash **pH which should be 5.2-5.6 ideally**, and if you don't cool your sample, your pH meter would read that as being 5.5-5.9 ish with ATC \(Automatic Temperature Compensation\). _Measuring pH at mash temperatures might damage your equipment and is not recommended._
{% endhint %}

There is a cog icon which allows you to change some settings regarding the water calculator. More on this later.

## Grains

![](../.gitbook/assets/image%20%2889%29.png)

The fist section of the water calculator shows your grain bill, and the calculator automatically assigns a grain type to it. Verify that the grain and **grain color** matches the grains you will be using, and that the **grain type** is correct.

If you use any **crystal**, **roasted** or **acidulated malt**, make sure they are assigned the right category as they have a big impact on the estimated pH. Adjust if needed.

![](../.gitbook/assets/image%20%2876%29.png)

You can also ignore the grain, making it not count towards the pH calculation. Useful if you are just steeping that specific grain.

## Water Volumes

Next section shows your water volumes, pulled from your recipe and equipment profile. Make sure they are correct. Adjust levels if needed. For example you might want to add more sparge water volume if you have some dead-space in the sparge water heater.

![Water Volumes](../.gitbook/assets/image%20%2862%29.png)

## Water Source

Your default water source profile is preselected and should normally not need any alterations if you have already set up your water profile. If you have multiple source water profiles, you can click the change button as needed to choose another profile as your source.

![Source Water Profile](../.gitbook/assets/image%20%2842%29.png)

## Target Profile \(optional\)

If you want to target a specific water profile for your water adjustment you can optionally select or create a target profile. The target profile is used for when you want to use the auto adjust feature to match your source water against this target. The target water profile is also what shows as a diff under your total water profile when adjusting.

![Target Water Profile](../.gitbook/assets/image%20%2841%29.png)

## Style Comparsion

![General style recommendation](../.gitbook/assets/image%20%281%29.png)

The style section allows you to compare your total water profile against a general recommended range or against a specific style recommendation.

If your target profile is above or below the recommended range it will show as red. And green if you are withing the recommended range.

![American IPA recommended style range](../.gitbook/assets/image%20%2814%29.png)

To select other style range recommendations click the dropdown to the right and select the style you want to compare against.

## Adjusting your minerals

 

![Unadjusted Water](../.gitbook/assets/image%20%2820%29.png)

This section of the water adjustment calculator is where you alter the actual water mineral additions. If you have created or selected a target profile, you can click the AUTO button to get close match or starting point to fine tune the additions.

{% hint style="info" %}
The default water calculator settings only AUTO adjusts Gypsum, Calcium Chloride and Epsom Salt. As these minerals only adjust the Calcium, Chloride, Magnesium and Sulfate levels the rest will be left as is. This can be changed in the Water Settings.
{% endhint %}

With a click on the auto button you will get a closer match to your target profile depending on what ingredients are activated and set to be auto adjusted.

![](../.gitbook/assets/image%20%2821%29.png)

In this example we got a good match on the values that the activated ingredients adjust and more or less hit our desired Calcium, Magnesium, Chloride and Sulfate levels and our desired Sulfate/Chloride ratio.

Fine tune as needed or manually adjust your values to hit your desired total water profile.

{% hint style="info" %}
The auto adjustment will not adjust your ingredients so you exceed any of your target profile values. So if you have trouble hitting your desired calcium or sulfate/chloride ratio with the auto adjust feature. Try increasing other target values, to allow for more room.
{% endhint %}

## Sparge Water

![](../.gitbook/assets/image%20%285%29.png)

When adjustment of sparge water is enabled, it will automatically calculate the needed amount to match your desired total water profile. When deactivated these minerals will be added to your mash water.

## Acid

### Mash

![](../.gitbook/assets/image%20%2810%29.png)

This section allows you to adjust your mash pH down by Lactic or Phosphoric acid. Select your acid type with the dropdown and set the concentration to your acid strength. Adjust the amount to match you desired mash pH.

### Sparge

![](../.gitbook/assets/image%20%2825%29.png)

This section allows you to get a calculated amount for how much acid to add to your sparge water to reach a desired target pH. Enter your source pH and sparge water target pH. Usually you want your sparge water pH between 5.5 and 6 to reduce tannin extraction.

## Save adjustments to your recipe

The data entered in the water calculator is saved to your recipe, so you can easily alter them later if needed.

To automatically save your ingredients to the Misc section of your recipe. Click the green **Save adjustments to recipe** button at the bottom.

![BOOM. Adjustments saved to your recipe. Ready to brew!](../.gitbook/assets/image%20%2890%29.png)

## Water Settings

To show the water settings click the cog in the top right of the water calculator.

![Water Settings](../.gitbook/assets/image%20%2817%29.png)

  
In the water settings you have a list of all the ingredients available to the calculator. By default only a few of them are activated as these are the most common ingredients used in water adjustments. And only Gypsum, Calcium Chloride and Epsom Salt is activated for auto adjustment as default.

In the advanced section you can **choose what form of Calcium Chloride** you are using. The default is Flaked. You can select Flaked, liquid or anhydrous. If you select liquid you can enter your concentration.

You can also select if your sparge water adjustment should be activated by default.

### Chalk

Using **Chalk** is **not recommended**, it is much preferred to use **Baking Soda NaHCO3** \(_or Slaked Lime_\) to increase pH. The reason for this is that under normal conditions Chalk reacts slowly and you will not get the effect on pH that you want when you need it. Much of the Chalk you add to mash will end up sitting on the grains after sparging and some will make it trough into the kettle and fermenter where it will continue to react and raising pH duing parts of the process where you would want it to be falling.

There are work-arounds such as dissolving it in acid but you need to be careful that you don't acidify below pH 8.4 \(at which pH all the carbonate has been converted to bicarbonate which does react rapidly enough to do what you want to do\). One of the acids for this purpose is carbonic acid. To use it the Chalk \(CaCO3\) is placed in a pet bottle with water and CO2 injected to raise the pressure to the point where enough H2CO3 is dissolved to, in turn, dissolve the CaCO3. The goal is to get the CO3-- converted to Bicabonate \(HCO3-\) and the tricky part is that as soon as the pressure is released the HCO3- will convert back to CO3-- and re-precipitate as microcrystals you cannot see and you think you have dissolved all the Chalk. And some of is still dissolved. The problem is that you won't really be able to tell exactly how much you have dissolved. \(Source: [AJ Delange](https://www.homebrewtalk.com/forum/threads/am-i-calculating-my-ph-right.652497/#post-8347271)\)

The option to activate Chalk is still there but use it carefully knowing the limitations.

## General help

### Solubility of minerals

Calcium Chloride is quite soluble.   
Calcium Carbonate \(Chalk\) is quite insoluble.   
Gypsum \(Calcium Sulfate\) is not as soluble as Calcium Chloride, but much more soluble that Calcium Carbonate.   
Calcium Carbonate and Calcium Sulfate are both **less** soluble in **hot water than cold** \(which is the reverse of the usual case\). \(Source: [AJ Delange](https://www.homebrewtalk.com/forum/threads/a-brewing-water-chemistry-primer.198460/#post-2324604)\)

### Calcium Chloride form

In the water calculator settings you can select between **Anhydrous**, **Dihydrate** and **Liquid**.

#### Anhydrous

**Anhydrous** is defined as without water. Therefore the anhydrous Calcium Chloride has a higher over all amount of calcium by weight.

**CaCl2** which has a molecular weight of 110.98 g/mol. Allegedly this would mean it is 100% Calcium Chloride. 

Anhydrous Calcium Chloride can be sold in pellet form. 

#### Dihydrate

Calcium Chloride **Dihydrate:** **CaCl2·2H2O** has a molecular weight of 147.0 g/mol This means the dihydrite is **theoretically at most**: \(110.98 g/mol/147 g/mol x 100%\) = **75.50 %** Calcium Chloride. 

In the real world the Calcium Chloride **Dihydrate is said to vary from 77% to 80%** Calcium Chloride. But selecting **Dihydrate / Flake** in the settings is recommended.

**Dihydrate** is typically in a flake form.

#### Liquid

When selecting Liquid as form you can enter the strengt/concentration of your solution.

\([Source](https://www.researchgate.net/post/Can_I_use_calcium_chloride_dihydrate_instead_of_calcium_chloride_for_the_preparation_of_buffer)\)

