---
description: Instructions for installing MultiMC
---

# Installing MultiMC

MultiMC is a Minecraft launcher that allows you to manage multiple versions of the game, as well as multiple game accounts, under one platform. This is our preferred launcher, though the Vanilla launcher will work perfectly well with our server.

{% hint style="info" %}
These instructions are for Windows. If you are using a different operating system, some details may vary.
{% endhint %}

1. Install the MultiMC Launcher
   1. Download a copy of MultiMC for your computer from [their website](https://multimc.org/#Download).
   2. This will download a file called `mmc-stable-win32.zip` to your computer (filename may vary for other operating systems)
   3. Open the downloaded ZIP file
   4. Extract the `MultiMC` folder from within the zip file to somewhere safe on your computer
      1. In my case, I extracted this to `C:\MultiMC`
   5. Open the folder you just extracted, You should see a collection of files, most of which will seem technical and can be ignored.
   6. Find `MultiMC.exe` in the folder and pin it to your start menu (optional, but will make life easier)
      1. Right click on `MultiMC.exe`
      2. In the context menu, click "Pin to Start"
   7. Close the `MultiMC` folder
   8. Hit start and click on MultiMC in your start menu
      1. Windows may inform you that this program is a security risk. If it does, click "More Info" then select the "Run Anyway" button.
   9. Select your language from the language selection (Default is English)
   10. Click "Next"
   11. In the Java selection window, you will need to specify a copy of Java 17 (for Minecraft versions 1.17 and above). If you do not see an entry listed for Version 17, follow the sub-steps on this step.
       1. Download a copy of Java 17 ([Windows](https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17\_windows-x64\_bin.zip)) ([Mac](https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17\_macos-x64\_bin.tar.gz))
       2. Extract the downloaded zip file somewhere safe on your computer (I recommend `C:\Program Files\Java\`)
       3. Back in the MultiMC Setup Dialogue, select "Browse"
       4. Navigate to `C:\Program Files\Java\jdk-17\bin` and select the `Java.exe` file
       5. Click the "Open" button
   12. In memory settings, you may specify the minimum and maximum amount of memory (RAM) Minecraft is allowed to use. This will be limited by your computers technical specifications, but I recommend a minimum of `1024 MiB` and a maximum of `8192 MiB`. If you are unsure how much memory your computer has, leave these settings alone.
   13. Click "Next"
   14. In the Analytics screen, you can opt out of performance analysis by unchecking the "Enable Analytics" box. This is checked by default, and you don't need to worry about it.
   15. Click "Finish"
2. Log In to the MultiMC Launcher
   1. In the top right-hand corner, select the "Profiles" dropdown
   2. Click "Manage Accounts"
   3. In the right-hand side of the Accounts dialogue, you can add either a Microsoft or Mojang account. Sign in using the credentials you used when purchasing the game.
   4. Once you have signed in, click "Close"
