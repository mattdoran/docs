# SmartPID

## What is SmartPID?

**SmartPID** is a powerful and flexible controller for complete **brewing process automation** and recipe management as well as **fermentation temperature control**. SmartPID is wifi connected for data logging and remote process control via web and mobile.

SmartPID is integrated with Brewfather to allow remote control and fermentation profile and recipe sending.

## Get SmartPID

SmartPID can be bought [**directly from Arzaman SRL here**](http://smartpid.com/store/).

## Need SmartPID device help?

**For SmartPID related setup, please check the** [**guides here**](http://smartpid.com/wiki/doku.php?id=demo_tutorials)**.  Please contact SmartPID on email:** [**smartpid@arzaman.com**](mailto:smartpid@arzaman.com) **or** [**facebook**](https://www.facebook.com/smartPID)**.**

## Integration features

{% hint style="info" %}
**SmartPID has some limitations to the number of recipe mashing and boil steps. And number of steps and duration in the fermentation profile. Brewfather will try to map your recipes and profiles as best as it can within these limitations. More details are noted about this further down in the documentation.**
{% endhint %}

**Smart Hombrewing Application**

* Recipe upload for starting the brew directly!
* Remote monitor of process parameters \(set point, current temperature, PID out, pump status, timers\)
* Process events listing
* Remote actions \(process start/stop pause/resume, set point change, power change, pump start/auto/stop\)

**Smart Thermostat**

* Start the fermentation profile directly from the batch based on your recipe!
* Remote monitor of process parameters \(set point, current temperature, PID out, timers\)
* Process events listing
* Remote actions \(process start/stop pause/resume, set point change\)

## Firmware Pre-Requirements

In order to use the integration a specific firwmare level is needed on SmartPID 

Both classic DIN box controller \(STC version\) and the new CUBE version are fully compatible.

**Smart Homebrewing ⇒** [**version 1.3-010**](http://smartpid.com/wiki/lib/exe/fetch.php?media=spc1000-biab-v1.3-010.bin.zip) **+**

**Smart Thermostat ⇒** [**version 0.5-014**](http://smartpid.com/wiki/lib/exe/fetch.php?media=spc1000-base-wifi-v0.5-014.bin.zip) **+**

Download the FW from the [SmartPID wiki page](http://smartpid.com/wiki/doku.php?id=sw_release) on the web site and upgrade. Click here for [upgrade instructions on video](https://youtu.be/RnQzNxVUHeo).

#### Upgrade mini guide

1. \*\*\*\*[**Download** ](http://smartpid.com/wiki/doku.php?id=sw_release)firmware from SmartPID
2. Unzip the .bin file
3. Rename .bin file to **flash.bin** before copying it to SmartPID
4. Attach SmartPID to computer via USB **while** holding the **RED** button
5. Delete **FLASH.BIN** from the SmartPID storage device that has now appeared
6. **Copy** new **flash.bin** to SmartPID storage device
7. Safetly detach device after copy has finished
8. Verify that upgrade is ok by checking firmware version in the info menu

#### Firmware upgrade troubleshooting

If you have a SmartPID Thermostat and want to switch it to a SmartPID Homebrewing controller, or vice versa, you need to contact the SmartPID seller, switching firmware directly will not work without a special flash file.

There is a know issue upgrading firmware on macOS, try a Windows computer if you have issues with Mac.

## Enable SmartPID integration

![Enable SmartPID in the Settings page in the Power-ups Section](../../.gitbook/assets/image%20%2865%29.png)

## Configure SmartPID

![Open the Devices page in the new menu option that appears](../../.gitbook/assets/image%20%2882%29.png)

## Register/Login to SmartPID account

In the devices page there will now be a **Configure** button next to the SmartPID section. Click it to set up SmartPID.

![Enter your e-mail and password, then login or register](../../.gitbook/assets/image%20%2852%29.png)

### Register new SmartPID account \(new SmartPID users\)

Enter your wanted e-mail and password then click Register. If registration is successful you will be logged in to the new account automatically. _**Warning: SmartPID Password is not encrypted and is stored in plain text**._

You can also register a new account in the SmartPID android app.

### Login to existing SmartPID account \(existing SmartPID users\)

If you already have a SmartPID account. Enter your e-mail and password then click Register. If registration is successful you will be logged in to the new account automatically. _**Warning: SmartPID Password is not encrypted and is stored in plain text**._

## SmartPID device setup

Your SmartPID needs to be set up with wifi connection and the login for your SmartPID account.

For instructions on how to set up your SmartPID device for Wifi and MQTT server connection please check the ****[**guide here**](http://smartpid.com/wiki/doku.php?id=demo_tutorials).

#### Common setups

[**SmartPID as a 1 channel thermostat for fermentation control**](thermostat-configuration.md)\*\*\*\*

#### Sampling time

SmartPID can be set up to send the status every X seconds. For best response time set this to 1 second.

## Register SmartPID device



![Configure SmartPID device](../../.gitbook/assets/image%20%2845%29.png)

1. From the SmartPID configuration window click **Add device**
2. Insert a name for your smartPID controller
3. Select the proper application \(homebrewing / thermostat\). This must be compatible with the firmware on your SmartPID
4. Enter the 12 characters serial number found in the SmartPID info menu
5. Enable **Channel 1** and/or **Channel 2**, optionally name the Channel\(s\).
6. **Save** to add to your device list
7. When you click Save the device will appear, and Brewfather will communicate with your SmartPID via MQTT messages

## Mode: Homebrewing

![Homebrewing Panel](../../.gitbook/assets/image%20%2833%29.png)

### Recipe upload and process start

{% hint style="warning" %}
**Important limitations:** Make sure the device is not in status mode, then it will be locked for control.

SmartPID is limited to a **fixed schema for the mash steps** \(listed below\), some mashing profiles might not translate 100%, you can check the recipe steps sent to the SmartPID by clicking the green **recipe** text in the Send Recipe toggle before you click start.  
  
SmartPID is limited to **max 10 boil addition** **alarms**.
{% endhint %}

1. Go to **Batches page** - **Brewing** tab
2. Click on the **Start** button in the **Brew Controller** section
3. Select your homebrewing controller from the list
4. Flag the proper options and press start to push the recipe to SmartPID controller and eventually start the recipe execution.

{% hint style="info" %}
Recipe is saved always in **position 1** in the controller and will override any recipe entered manually in that position
{% endhint %}

![Start a recipe from the batch page](../../.gitbook/assets/image%20%2896%29.png)

![Start Homebrewing SmartPID](../../.gitbook/assets/image%20%2824%29.png)

#### Optional Mash Steps Template

If you want one to one mapping of the mahing steps to the recipe format of the SmartPID you can utilize the **Mash steps template** mashing profile. Brewfather will also intelligently try to **map any mash profile** to the fixed SmartPID scheme so this step is optional. 

![](../../.gitbook/assets/image%20%2853%29.png)

1. Select profile in recipe

![](../../.gitbook/assets/image%20%2878%29.png)

2. Alter the profile by adjusting time and temperature on the steps with time greater than 0. Leave the rest as is.

## Mode: Thermostat

![Thermostat Panel](../../.gitbook/assets/image%20%2846%29.png)

### Start fermentation profile from recipe

{% hint style="warning" %}
**Important limitations**: Make sure the device is not in status mode, then it will be locked for control.

SmartPID is **limited to 8 fermentation profile steps** where the fist 7 steps have a **maximum duration of 4 days** per step. This might limit the fermentation profile possibilities if you have profiles with many steps. _Step 8 will continue with no maximum duration._ **Brewfather will try to map your profile as best as it can within these limitations**  \(splitting steps with a duration longer than 4 days into multiple steps for the SmartPID profile\). _But you are adviced to double check the profile steps._
{% endhint %}

1. Go to **Batches page** - **Fermentation** tab
2. Click on the **Start** button in the **Fermentation Controller** section
3. Select your thermostat controller from the list
4. Click **Start** to start the profile

Optionally you can also start a fermentation profile or standard/manual mode from the devices page.

{% hint style="info" %}
Profile is saved always in **position 1** in the controller and will override any profile entered manually in that position
{% endhint %}

![Start fermentation profile from Fermentation Controller in fermentation tab](../../.gitbook/assets/image%20%2897%29.png)

![When starting thermostat from the devices page you can select standard or advanced mode](../../.gitbook/assets/image%20%2875%29.png)

