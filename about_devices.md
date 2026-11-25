
### ADAM Devices


In the [ADAM utility software](https://www.advantech.com/en-us/support/details/utility-?id=1-2AKUDB), device settings can be changed and firmware can be updated if needed. MAC addresses for devices can be found in the network tab. Your host PC shows up in the top left corner. Select it and then "search devices" in the toolbar to see what devices are on the network. 

[The 6000 series manual can be found here.](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://advdownload.advantech.com/productfile/Downloadfile4/1-2B6FKTG/ADAM-6000_User_Manaul_Ed.12-FINAL.pdf&ved=2ahUKEwjRyp2OneOTAxUSSjABHWhZJwQQFnoECAwQAQ&usg=AOvVaw1ShTVVehOvGWRFBkxTfZde)


#### ADAM 6051
The ADAM-6051 has 12 digital inputs, 2 counter channels, and 2 digital outputs with 2000 VDC isolation. All digital inputs have a latch function and can be used as counter/frequency input channels. All of these are readable over Modbus/TCP on port 502.

### Serial Servers
To get connected to a new serial server, plug it into your computer and enure it has power. Then, find out what the default IP is and change your computer's IP to something that matches it's first three digits. When that's done, you should be able to visit the device's IP in your browser and assign it a new IP. Connect the device to the ethernet and reassign your normal IP. 

These devices use RTU over TCP rather than just straight up TCP. They connect to devices that don't have their own ethernet connectivity, included below


#### Elkor WattsOn

These devices are used to report on wattage. They can be wired in serial accross three 6 devices (`device_id`) in `pollees.csv` and can have up to three channels that report on voltage and amps. 

[Elkor WattsOn Manual](https://www.elkor.net/pdfs/WattsOn_Manual.pdf). 

## Solark Inverters

Solark inverters have a variety of data types. Registers aren't listed in the manual. Register numbers can be found via the [mysolark site](mysolark.com) by downloading data in the Operational Data tab. There is also a Github with register numbers [at a dictionary from Paul Bixel's Home Assistant repo](https://github.com/pbix/HA-solark-PV/blob/main/custom_components/solark/solark_register_map.py) (thank you Paul <3).

[More here.](https://sol-ark.com/wp-content/uploads/prod-doc/SK140-0003-002-12K-2P-N-EN-Manual-1-1.pdf) 
