# twincat-lv-ads-library
TwinCAT ADS library written in LabVIEW

This library was written to interface LabVIEW applications with Beckhoff PLCs. With this library it is possible to read PLC variables through a Client connected to the PLC network using the TwinCAT Runtime.
This library is written and maintained with LabVIEW 2016.

# prerequisites
The Client must run TwinCAT ADS Runtime. This library was tested with TwinCAT ADS Runtime 3.1.4024.10. The run-time can be found at the following link https://www.beckhoff.com/english.asp?download/tc3-download-xar.htm.

This library uses the .NET interface therefore it can only be used in a Windows environment.

# twincat ads static route setup
Once installed the TwinCAT ADS Runtime on the Client, a static route must be set.

1. Right-click on the TwinCAT sys-tray icon and select 'Router > Edit Routes'; the 'Add Route Dialog' panel pops up.
2. Enter the Server (PLC) Host Name or the IP address and press 'Enter Host Name / IP:' button
3. Select 'ADS_UDP' as Transport Type
4. Press 'Add Route' button; the 'Add Remote Route' panel pops up.
5. Enter the Server access credentials: User Name and Password. Press 'Okay' button.
![Step4](Pictures/1_AddRouteDialog.PNG?raw=true "Step 4")
![Step5](Pictures/2_AddRemoteRoute.PNG?raw=true "Step 5")
6. The panel 'TwinCAT Static Routes' will shows up. An 'x' in the 'Connected' field indicate a succesful connection Client <> Server.
![Step6](Pictures/3_TwinCATStaticRoutesDialog.PNG?raw=true "Step 6")

# how to use the library
Usage example is shown below.
![Example](Pictures/4_LabVIEWExample.PNG?raw=true "LabVIEW Example")

This project is maintained by MET. For support write to support@met.it
