# Windows-Tweaks
List of useful tweaks to keep your Windows machine fast as the first day.
A.A. Please, if you are planning to re-use this data, make proper credits to my profile, I spent hours to get the best configuration without messing up my system.

## LET'S BEGIN!

### 1. If you come from a fresh-clean installation, install/update your drivers

### 2. Disable Windows Update service:
   - Search for "services"
   - Find Windows Update
   - Right click on it -> Boot type: Disabled -> Stop service
   
### 3. Disable superfetch/Ottimizzazione avvio (in italian)
   A.A. I have analyzed this service, and I discovered that it could be the first useful Windows service ... why am I saying that? Do you think I'm crazy?
   Well, on the web you can find a lot of threads, dealing with such Superfecth, how bad it is, how much space it wastes, how much hdd/cpu it uses at boot and so on.
   I made some tests and I have discovered some curious aspects.
   - If you disable its service: bios boot is the same, Desktop loading is slower (noticeably), no 100% hdd usage by it (of course).
   - If you have it enabled: Desktop loading is fast, sometimes when Desktop has been loaded, hdd usage is at 100%
   
   Why is it happening?
   SuperFetch service (Ottimizzazione avvio) purpose is to cache most used resources in order to speed up boot (that should be obvious). 
   But why is it always overloading the hdd on boot?
   - It loads stuff from the superfetch file.
   - It updates the superfetch file.
   
   Now that you have cleared your ideas, you should probably know what to to.
   
   STEPS TO DISABLE IT
   - Search for "services"
   - Once opened, find the Superfetch/Ottimizzazione avvio service
   - Set the boot type to Disabled
   - Stop it
   - Apply
   
### 4. Disable Windows Defender and Security center (I noticed that it noticeably slows down the boot)
   - Extract the two files from "Windows Defender tweaks.zip"
   - Double click on "Disable AntiMalware Executable.reg"
   - Confirm
   - If you want to re-enable it, just double click on the other file.
   - In both of cases, you have to reboot.
   A.A. It should appear a Windows notification that reminds you that you have no Anti virus defense enabled. What I say to you: if you are planning to install another AntiVirus software, ok then you are good to go. Otherwise, you should decide if it could be useful to you; probably if you reached this page, you are as smart to understand that if you are careful on the net (you do not click on stupid ads, you have ad-blocker, you do not.. bla bla) AntiVirus are totally USELESS, even on Windows, indeed they are just resource-wasters.
   
### To return to default state, just re-enable the two services (Update and SuperFecth) and set their boot types to "Auto".
