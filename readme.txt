Here are Huawei devices for eNSP. Please read this carefully.

The boot is not very fast. It may take about 2-5 minutes to load. Please try to type something in console to see the progress. 
When you see "#######" symbols, it means that the Windows has booted, the eNSP has loaded the topology and now the device is loading.

Please try to boot Huawei routers twice. Their appliances use "-cpu host" option and the first boot may fail, as the Windows requires reboot after your CPU has been initialized.

You may try to set less RAM and CPU, but the work is not guaranteed, as it's below eNSP's system requirements. 
To explore or change the internals, you may select vnc console type. The password is ensphost.

Please don't change the number of adapters. Otherwise, additional steps are required: 
 - you need to start the device with vnc console type, 
 - connect to the vnc console, 
 - get the list of _NPF IDs of adapters with the getmac utility in the Command Prompt
 - and edit the C:\Users\mnadmin\Desktop\ubridge\ubridge.ini, so that the IDs there to be correct.

These appliances are based on Windows 7 Professional MSDN installation. You need the license, otherwise the usage is not legal. This one is Volume License version.
