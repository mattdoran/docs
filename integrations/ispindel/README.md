# iSpindel

Go into the settings page in [Brewfather APP](https://web.brewfather.app/), enable iSpindel. You will then get a **Server Address** and **Server URL** that you need to copy into the iSpindel configuration page.

Set your iSpidel in configuration mode, you can then access your iSpindel by WiFi.

In the iSpindel configuration page enter any **name** you want, set **Service Type**: **HTTP**, **Port**: **80**, **Update intervall**: **900**, copy the Server Address and Server URL from the Brewfather settings. \(It the port/server address fields does not show try this: Hit the HTTP button twice.\)

Make sure your polynomial contains your fully calibrated formula. And make sure your Wifi-settings are correct. Click save.

Your iSpindel should then log every 15 minutes.

After the iSpindel has done its first logging to Brewfather, it will appear in the device list located in your Batch &gt; Fermentation &gt; Readings &gt; **Devices**. Click on the Devices button and attatch your iSpindel to the batch. The next time your iSpindel logs, it will show up in your batch!

**Never log more than once every 15 minutes**, request logged more often than that will be ignored. It is **very important that your update intervall is 900 or higher**, otherwise your logging will be ignored.

{% hint style="info" %}
Make sure your iSpindel reports gravity in Plato \(it will be converted to SG\) and temperature in Celcius. Add **\[SG\]** to the name of your iSpindel if you use SG based formula. If the gravity is displaying 1.004 in Brewfather you are using the wrong formula, use the fomula that reports in Plato or use the tag above.
{% endhint %}

### Multiple devices

Having multiple iSpindels logging to Brewfather is simple, just set them all up logging to the same URL, but make sure they have unique names in the iSpindel configuration.

