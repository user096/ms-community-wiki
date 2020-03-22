# Reinstalling Graphics Drivers

## Method 1: Windows Update

> This method will update Windows and all available drivers, however as a general troubleshooting step this is not a bad idea.

1. Open the Settings app. You can do this by searching for it in the Start menu, pressing <kbd>Win</kbd> + <kbd>I</kbd>, or pressing the Settings icon above the power button.

   ![](img/reinstalling-gpu-drivers/opensettings.png)

2. Select "Update & Security".

   ![](img/reinstalling-gpu-drivers/updateandsecurity.png)

3. If there are updates available, click "Download". Otherwise, click "Check for Updates".

   ![](img/reinstalling-gpu-drivers/checkforupdates.png)

4. Windows should begin looking for any drivers or updates available for your device. if any are available.

   ![](img/reinstalling-gpu-drivers/checkingforupdates.png)
   
   ## Method 2: Intel Driver & Support assistant
> Method 1 wont find any results?? but you sure theres a driver for it? try intel and support!
<b>THIS METHOD IS FOR INTEL DRIVERS ONLY! IF YOU USING ANY OTHERS DRIVRES (AMD, NVIDIA ETC...) GO TO METHOD3!

1.Go to https://www.intel.com.au/content/www/au/en/support/intel-driver-support-assistant.html and download the intel and support software
back to the link again and your page should be started scanning. if it doesnt click "F5"
![](img/reinstalling-sound-devices/intel-support.png)
and your graphics drivers / sound drivers should be detected in the list.
![](img/reinstalling-sound-devices/intel-support-list.png)
if theres no update you should be seeing a green bar:
![](img/reinstalling-sound-devices/intel-no-update.png)
Else, if there is you will see a bar saying update now. select that and go through the installer.
## Method 3: Device Manager

> This method may not work effectively on older versions of Windows, if this is the case then use method 3.
for graphics drivers:

1. Open Device Manager by either searching for it in Start, or pressing <kbd>Win</kbd> + <kbd>R</kbd> and typing <kbd>devmgmt.msc</kbd> afterwards.(alternatively you can use <kbd>Win</kbd> + <kbd>X</kbd> and tapping <kbd>M</kbd> afterwards.)

   ![](img/reinstalling-sound-devices/devmgmt.png)

2. Find and expand the "Display adapters" or "Sound, video and game controllers" icon. You'll be presented with a list of the graphics devices in your system. There will usually be only one or two.

   ![](img/reinstalling-gpu-drivers/devmgmtdisplayadapt.png)

3. 3. Right-click the adapter you wish to reinstall the drivers for and right-click it. Then, select "Uninstall device".

   ![](img/reinstalling-gpu-drivers/devmgmtuninstall.png)

4. Select "Delete the driver software for this device" then click "Uninstall". Note that your screen may flicker after clicking this button. For sound drivers your sound might cut for several times.
   ![](img/reinstalling-gpu-drivers/devmgmtdelete.png)

5. Go to "Action", then select "Scan for hardware changes".

   ![](img/reinstalling-gpu-drivers/devmgmtscan.png)

6. Go back to Display Adapters/ sound adaptors and find the graphics device you are attempting to reinstall. Note that it may now be called "Microsoft Basic Display Adapter". Right-click it and select "Update driver".

   ![](img/reinstalling-gpu-drivers/devmgmtupdate.png)

7. Windows will now begin installing the latest graphics driver it can find. Note this may take some time and your screen may flicker. Note that if you get a message claiming the latest drivers are already installed, attempt method 3.

## Method 3: OEM Website

> It is difficult to be precise with this method as hardware configurations and website layouts vary considerably. If you're unable to find the correct page for your drivers, searching "[device] graphics drivers" or "[device] sound drivers" may help yield the correct results. Just make sure you're getting them from the manufacturer's website (or intel support assistant [method2]).
>
> Generic display drivers for most common adapters can be found here:
>
> - Intel: https://downloadcenter.intel.com/
> - NVIDIA: https://www.nvidia.com/Download/index.aspx
> - AMD: https://www.amd.com/en/support
> - sound drivers should be ususally realtek:
> - https://realtek-download.com/download-hd/

> You may also want to use DDU for this if you're using an NVIDIA or Intel GPU. If that's the case, there is an excellent guide on that [here](https://www.wagnardsoft.com/content/ddu-guide-tutorial). If you're using an AMD GPU, then the Radeon installer's built-in "factory reset" (under Additional Options) function is preferred over DDU.

1. Open your web browser and navigate to the website of your device or graphics adapter's manufacturer. For example, if this is a Dell laptop then go to Dell's website, however if it's a custom-built desktop with an NVIDIA graphics card, then head to NVIDIA's website etc.

2. Locate the option for downloading drivers for your product. If it is a pre-built computer such as a laptop you may need to model or serial number to find the download page.

3. Find the download for the drivers, agree to any terms and conditions, then download the file.

4. Run the downloaded executable file and follow the on-screen instructions.
