# Setting up your equipment profile

To set up your Equipment profile, select the Profiles page from the menu. Click Equipment, and add a new profile, or edit the default profile.

![Equipment profile is customizable to get the right numbers for your system](../.gitbook/assets/image%20%2874%29.png)

**Name:** Name for your equipment profile

**Boil Time:** Boil time for this equipment profile, if you adjust boil time when "Calc boil volume" is activated, the pre-boil volume will change to match the new boil time based on boiloff.

**Description:** Free text field for details about the equipment.

## Volumes

**Batch Volume Target:** Select if you want your Batch Volume to match final volume in **Fermenter** or end of boil **Kettle** volume \(hot\) also know as Post-Boil Volume.

{% hint style="info" %}
Using **Kettle** as **batch volume target** will be **easier** to set up since the Original Gravity calculation will be the same **independent of** your amount of **Trub/Chiller loss** \(except fermenter additions\). Also you only have to know your **mash efficiency** to set this up and **brewhouse efficiency is not needed**.
{% endhint %}

**Batch Volume:** Your final batch volume target, a factor in calculating your Original Gravity.

**✔ Calc boil volume:** Automatically calculates your Pre-Boil Volume if this is active, calculated back from batch volume. Based on your boiloff rate, trub/chiller loss, and **4%** shrinkage/expansion.

**Pre-Boil Volume:** Set your pre-boil volume manually or have it calculated automatically \(recommended\). This volume is measured at near boiling temp \(after expansion\). **Post-Boil Volume** is also measured at boiling temp \(before chill\).

**Boil Off:** How much you boiloff per hour with your setup, important factor in calculating Pre-Boil Volume.

**Trub/Chiller Loss:** How much you loose as trub \(and/or left in chiller and/or pipes\) **from kettle to fermenter**, important factor in brewhouse efficiency. Total volume of the trub left in the kettle and/or cooler/tubes/hoses, including hop trub.

**Mash-Tun Deadspace:** Recoverable deadspace volume in your mash-tun, used for calculating mash water amount. In a system with a malt pipe, it is the volume before the water reaches the bottom of the malt pipe. Usually 0 in BIAB.  
  
_Recoverable volume is volume that is not lost in mashing, but will be inlcuded in the boil._

**Mash-Tun Loss:** **Unrecoverable** deadspace volume in your mash-tun and/or mash volume lost in your mash process. This is usually 0 in a one-vessel setup. A factor in mash efficiency. _Unrecoverable volume not transferred to boil._

**Fermenter Loss:** Expected loss from fermenter to bottle/keg. Used to estimate bottling volume and gravity potential from fermentables added as _use_ = _Bottling_.

**HLT Deadspace** is any dead space in the Hot Liquor Tank \(Sparge Water Heater\). For example, if you use a sparge water heater that has the tap that draws higher than the bottom of the pot, you can set the liters that are not drawn. This volume will be added to the sparge water amount in the Water Adjustment Calculator, for calculating your sparge water additions.

_Post-Boil Volume in Brewfather reefers to hot end of boil kettle volume, before shrinkage \(4%\)._

## Efficiency

**Brewhouse Efficiency:** The overall efficiency of you system - includes all losses to the fermenter. Important factor in calculating you Original Gravity. If you don't know you system, a good number to start with might be 65-75%. And you can dial in your excact efficiency after a couple of brews.

**Mash Efficiency:** The efficiency of your mash procedure, up to pre-boil, including sparging. Important factor in calculating your Pre-Boil Gravity.

If you enable "calculate mash efficiency" by enabling the **Calc mash efficiency** checkbox, the mash efficiency will be back-calculated from the brewhouse efficiency based on the equipment profile numbers. If disabled, the brewhouse efficiency will be calculated based on the mash efficiency \(**recommended**\).

## Advanced

**Hop Utilization:** Normally left at 100%. Average hop utilization for your equipment. This is a global multiplier to the IBU calculation.

**Aroma Hop Utilization:** For calculating IBU on hopstand/whirlpool hops, also used as a factor to calculate increased IBU from boil hops when you have a hopstand. This utilization is used only when no temperature is entered separately on the hop-stand/whirlpool hop in the recipe.

**✔ Calc aroma hop utilization:** If checked, it will automatically calculate your Aroma Hop Utilization based on the entered hopstand temperature. 

**Hopstand Temperature:** The average temperature of your hopstand, used to automatically calculate your _Aroma Hop Utilization_ when _Calc aroma hop utilization_ is checked. This is also displayed in the brew sheet if temperature is not specified on the hopstand hop.

## Mash and sparge water

**Grain Absoprtion Rate**: Amount of water absorbed by the grain per unit of grain. L/kg when using metric units, and qt/lb when using gal/lbs as volume/weight units.

**Water/Grain Ratio**: Amount of effective mash water per unit of grain. L/kg when using metric units, and qt/lb when using gal/lbs as volume/weight units.

**Mash/Sparge Water Calculation Method**:  
  **Default**: Normal calculation of mash/sparge water amounts.  
  **No Sparge**: No sparge, full mash volume.  
  **Custom**: Define your own custom formula. Formulas must result in water amount in Liter.

### Mash Water/Volume

_Settings for calculating mash water_

**✔ Include grain volume in mash limits**: When this is checked the min and max mash **water** limit turns into mash **volume** limit. Which means that the wet mash grain volume is included in the numbers. Then the max mash volume limit becomes the mash-tun max capacity.

**Min:** Minimum limit of mash water, **Max:** Maximum limit of mash water

If the calculated mash water is under the minimum limit, it will take water from the sparge water amount and move it to increase the mash volume, dynamically increasing your water/grain ratio.

If the calculated mash water is over the maximum limit, it will move water to sparge or top-up water to not exceed the limit, dynamically decreasing your water/grain ratio.

### Sparge Water Limit

Use this to avoid getting to much sparge water calculated, if you have limited room in your HLT.

**Min:** Will take water from calculated mash water if possible to reach a miminum sparge water amount. Minimum mash water will be prioritized.

**Max:** Maximum amount of room in your HLT / Sparge Water Heater.

**Overflow Taget:**   
  **Top-Up:** overflow is moved to top-up water \(boil\).  
  **Mash:** If the calculated sparge water amount is above the limit, it will move water to mash \(until maximum mash volume is reached\) and/or top-up water to not exceed the limit.

**Min HLT water amount**: Define the minimum amount of suggested HLT water you want, so you can cover the coil or heating element.

### Strike Water Temperature

**✔ Calc strike water temperature:** When this is checked a calculated strike temperature is added as a first step in your mash schedule.

**Mash-Tun Heat Capacity in** _**L equivalient water volume**_**:** If your mash-tun is pre-heated set heat capacity to 0. Otherwise use the **Mash-Tun Calibration tool** to get the value for your equipment. This is **not** Mash-Tun volume.

### Sparge Temperature

Enter your desired sparge temperature.

## Basic steps to set up an equipment profile for a single vessel system

1. **Mash-tun deadspace**: Add water until you reach the bottom of the malt-pipe, note exactly how much water you need to add.
2. With the malt-pipe inserted, add water until it reaches 2-3 cm from the top of the malt pipe, note exactly how much water. This will be the **max mash volume** \(including **grain**\). If the brewer has overflow function, stop right before it overflows instead.
3. **Boiloff** test, adjust the power % \(if possible\) to get a reasonable boil, ideally wort, but water will work also, note how much water has boiled off per hour. Remember to measure the volumes at the same temperatue, either both hot or cold.
4. Measure how much water is left in the system after pumping/draining all the water/wort out \(not center/dump drain\), estimate of **trub loss**. Dip tube should be adjusted down \(if applicable\).
5. To figure out a reasonable **water/grain ratio** ideally, one should do multiple mashes and get experience, but one alternative is to do a brew with about 1.060 OG and note how much water added to get a good mash thickness. Substract the Mash-tun deadspace, then divide amount of water on amount of grains to get the water/grain ratio.
6. Start out with for example a brewhouse **efficiency** of 70%, or **mash-efficiency** of 75%, and adjust it to your result after the first few brews.

We should be able to set up a basic profile from that, which can be fine-tuned as you get more experience with the efficiency and losses.

