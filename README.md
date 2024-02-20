# Automatic Razer HyperPolling Dongle polling rate changer FORK 
## Added support for inline cfg polling rate setting

## Behavior
Polling rate will be limited to the inactive one when not running the processes in the process list to conserve battery.

It will automatically switch to the active one as soon as an added process is running.

Any polling rate changes in Razer Synapse will be overwritten but will **not** display in it's menu.

## Instructions
- Install the application from the latest release
- Right click the tray icon to select the inactive and active polling rates (default is 500hz and 4000hz)
- Right click the tray icon to open the process list (processlist.cfg):
    - add any process name including the .exe ending (case insensitive)
    - you can add multiple processes by simply adding their name to a new line
- Processes.CFG requires strict formatting, and no input validation is done. Example:

application.exe space polling-rate


Discovery.exe 2000

FPSAimTrainer-Win64-Shipping.exe 2000

DOOMEternalx64vk.exe 8000

LatMon.exe 8000

FortniteClient-Win64-Shipping.exe 2000

## Additional Information
- Razer Synapse does not have to be running
- Available polling rates are 125hz, 250hz, 500hz, 1000hz, 2000hz, 4000hz and 8000hz (only for the Viper Mini SE). (250hz will work even though it is not an option in Razer Synapse)
- The lower the inactive polling rate is set to the more battery you will save. (Halving polling rate roughly halves power consuption)

