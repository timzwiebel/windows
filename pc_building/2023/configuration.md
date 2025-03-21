# 2023 Computer Configuration

## BIOS Updates
1.  Download the
    [latest BIOS](https://www.asus.com/us/motherboards-components/motherboards/tuf-gaming/tuf-gaming-b650-plus-wifi/helpdesk_bios)
1.  Prepare the updated BIOS file:
    1.  Unzip the file
    1.  Run `BIOSRenamer.exe`
    1.  Copy the `.CAP` file to the root directory of a FAT32 USB drive
        (although simply copying the file to `D:\` seems to work as long as it's
        in the root directory)
1.  Reset the BIOS to its default settings (recommended by the manual for
    stability):
    1.  Reboot into the BIOS (by repeatedly pressing the **Delete** key during
        boot)
    1.  Switch to **Advanced Mode (F7)**
    1.  **Exit > Load Optimized Defaults**
    1.  **Exit > Save Changes & Reset**
1.  Update the BIOS:
    1.  Reboot into the BIOS (by repeatedly pressing the **Delete** key during
        boot)
    1.  Switch to **Advanced Mode (F7)**
    1.  **Tools > ASUS EZ Flash 3 Utility**
    1.  Select the `.CAP` file and follow the instructions
1.  Restore BIOS settings:
    1.  Go through the [BIOS Settings](#bios-settings) below and restore the
        settings to their desired state
1.  Clean up files:
    1.  Delete the `.CAP` file from all drives
    1.  Delete the unzipped folder containing `BIOSRenamer.exe`

## BIOS Settings
1.  Set the date/time (gear icon in the top-left corner)

1.  Switch to **Advanced Mode (F7)**

1.  Configure **MyFavorite (F3):**
    1.  Click **Delete All**
    1.  Add the following:
        - Main > System Date
        - Main > System Time
        - Monitor > Temperature Monitor
          - (Useful monitoring)
        - Monitor > Fan Speed Monitor
          - (Useful monitoring)
        - Monitor > Voltage Monitor
          - (Useful monitoring)
        - Tool > ASUS SPD Information
          - (Useful information)
        - Tool > ASUS EZ Flash 3 Utility
          - (Used to update the BIOS)
        - Ai Tweaker > Ai Overclock Tuner
        - Ai Tweaker > Memory Frequency
          - (Unchanged, but useful to know)
        - Advanced > SATA Configuration > SATA Controller(s)
        - Advanced > APM Configuration > ErP Ready
        - Advanced > Onboard Devices Configuration > LED lighting > When system
          is in working state
        - Advanced > Onboard Devices Configuration > LED lighting > Windows
          Dynamic Lighting
        - Advanced > Onboard Devices Configuration > LED lighting > When system
          is in sleep, hibernate or soft off states
        - Advanced > Onboard Devices Configuration > USB power delivery in Soft
          Off state (S5)
        - Advanced > Onboard Devices Configuration > Wi-Fi Controller
        - Advanced > Onboard Devices Configuration > Bluetooth Controller
        - Advanced > NB Configuration
          - (Unchanged, but useful for changing between integrated graphics and
            PCIe)
        - Monitor > Q-Fan Configuration
        - Tool > ASUS Armoury Crate > Download & Install ARMOURY CRATE app
        - Tool > MyASUS > Download & Install MyASUS service & app

1.  Change BIOS settings:
    - **Ai Tweaker > Ai Overclock Tuner** from `Auto` to `EXPO II`<br>
      - A good description of these settings can be found at
        [1:06:14 of this video](https://www.youtube.com/watch?v=wzVZgTP2204&t=3974s)
        - The video discusses XMP, but EXPO is just AMD's version of XMP (which
          is from Intel)
        - TL;DW:
          - > *XMP II is actually what is considered our pure default, so this
            > is exactly reading the information just as it's provided by the
            > DRAM manufacturer. So if you want to try something, XMP II is not
            > a bad place to start because it's like the most pure basic form of
            > XMP.*
          - > *My general rule of thought is when engaging memory and doing
            > overclocking is like go first always "what's going to be the
            > highest level of stability and assured success?", so I do usually
            > default to II and then tell people "test your memory".*
    - **Advanced > SATA Configuration > SATA Controller(s)** from `Enabled` to
      `Disabled`
    - **Advanced > APM Configuration > ErP Ready** from `Disabled` to
      `Enable(S4+S5)` (Changing this value changes a few others mentioned below)
    - Ensure that **Advanced > Onboard Devices Configuration > LED lighting** is
      configured correctly:
      - **When system is in working state** should be `All On`
      - **Windows Dynamic Lighting** should be `Disabled`
      - **When system is in sleep, hibernate or soft off states** should be
        `Onboard LED off` (this value changes with **ErP Ready**)
    - **Advanced > Onboard Devices Configuration > Wi-Fi Controller** from
      `Enabled` to `Disabled`
    - **Advanced > Onboard Devices Configuration > Bluetooth Controller** from
      `Enabled` to `Disabled`
    - Ensure that **Advanced > Onboard Devices Configuration > USB power
      delivery in Soft Off state (S5)** is `Disabled` (this value changes with
      **ErP Ready**)
    - **Monitor > Q-Fan Configuration** to the following:
      - For each fan, change the **Profile** from `Standard` to `Manual`
      - Change each fan's settings:
        > **&#8505;&#65039;<!-- information emoji --> NOTE:** By running Q-Fan
        > Tuning, I determined that the CPU and bottom fans have a minimum duty
        > cycle of 25% while the front fans have a minimum duty cycle of 30%. I
        > determined the "Points" based on each fan's minimum duty cycle and...
        > TODO
        TODO: link to fan specs for "Speed Low Limit"
        - CPU
          - Q-Fan Source: **CPU Package** (use CPU Package instead of CPU
            since it seems to be a higher temperature)
          - Speed Low Limit: **400 RPM**
          - Point 4: 70°C, 100%
          - Point 3: **55°C**, **75%**
          - Point 2: **40°C**, **50%**
          - Point 1: **25°C**, **25%**
        - Chassis 1: rear and center bottom fans (RPM values are reported from
          the rear fan because a splitter is used)
          - Q-Fan Source: **Multiple Sources (CPU, CPU Package, MotherBoard)**
          - Speed Low Limit: **500 RPM**
          - Point 4: 70°C, 100%
          - Point 3: **65°C**, **75%**
          - Point 2: **55°C**, **50%**
          - Point 1: **35°C**, **25%**
        - Chassis 2: upper front fan
          - Q-Fan Source: **Multiple Sources (CPU, CPU Package, MotherBoard)**
          - Speed Low Limit: **300 RPM**
          - Point 4: 70°C, 100%
          - Point 3: **65°C**, **75%**
          - Point 2: **50°C**, **50%**
          - Point 1: **30°C**, **30%**
        - Chassis 3: forward bottom fan
          - Q-Fan Source: **Multiple Sources (CPU, CPU Package, MotherBoard)**
          - Speed Low Limit: **500 RPM**
          - Point 4: 70°C, 100%
          - Point 3: **65°C**, **75%**
          - Point 2: **55°C**, **50%**
          - Point 1: **35°C**, **25%**
        - Chassis 4: lower front fan
          - Q-Fan Source: Multiple Sources (CPU, CPU Package, MotherBoard)
          - Speed Low Limit: **300 RPM**
          - Point 4: 70°C, 100%
          - Point 3: **65°C**, **75%**
          - Point 2: **50°C**, **50%**
          - Point 1: **30°C**, **30%**
    - **Tool > ASUS Armoury Crate > Download & Install ARMOURY CRATE app** from
      `Enabled` to `Disabled`
    - Ensure that **Tool > MyASUS > Download & Install MyASUS service & app** is
      `Disabled`

1.  **Exit > Save Changes & Reset**

## Installing Windows
During the installation:
1.  Format the drive(s):
    1.  Click **New**
    1.  Set the **Size** to `262260 MB` (100 + 16 + 256*1024). This will create
        the following:
        - 100 MB System (FAT32 EFI)
        - 16 MB MSR (Microsoft Reserved Partition)
        - 256 MB Primary (NTFS for Windows)
        TODO: should these be "MiB" instead of "MB"?

After the installation:
1.  Optional: fix the monitor layout (right-click the **Desktop > Display
    Settings**)
1.  Disable OneDrive:
    1.  Open OneDrive, click the gear in the top-right, and click **Settings**
    1.  Change OneDrive settings:
        - **Settings > Start OneDrive automatically when I sign in to windows:**
          `disabled`
        - **Backup > Manage backup:** uncheck all folders
1.  Install
    [drivers](https://www.asus.com/us/motherboards-components/motherboards/tuf-gaming/tuf-gaming-b650-plus-wifi/helpdesk_download):
    - Chipset
    - LAN
    - Graphics (via [Nvidia App](https://www.nvidia.com/en-us/software/nvidia-app))
      - (Remember to perform a clean install, just in case)
      - Change **Settings > General > In-Game Overlay > Settings > Keyboard
        shortcuts > Open/close in-game overlay** from `Alt+Z` to `Alt+O`
    - Audio
1.  Run Windows Update
1.  Install
    [Western Digital Dashboard](https://support-en.wd.com/app/products/product-detailweb/p/8695):
    1.  Change WD Dashboard settings:
        - **Disable Background Tasks Minimized:** `enabled`
1.  Optional: assign the `C:` partition a volume label of `Windows`
1.  If it doesn't already exist, create the `Data (D:)` partition using the
    remainder of the space
1.  Prune **Settings > Apps > Installed apps:**
    - TODO
1.  Change Windows settings:
    - **System > Storage > Temporary files:** Refresh, then remove the
      following:
      - **Previous Windows installation(s)**
      - **Delivery Optimization Files**
    - **Network & internet > Ethernet > Network profile type:**
      `Private network`
    - **Personalization:** `Windows (dark)`
    - **Personalization > Themes:** `Windows (dark)`
    - **Apps > Startup:**
      - **Microsoft Edge:** `disabled`
      - **Microsoft Teams:** `disabled`


## Installing Software
1.  Install [Chrome](https://www.google.com/chrome):
    1.  Change the default browser in Windows to Google Chrome: go to
        **Settings > Apps > Default apps > Google Chrome** and set Google Chrome
        as the default for all of the relevant file types.
    1.  Change Chrome settings:
        - **Performance > Memory Saver:** `enabled`
        - **Settings > Downloads > Location:** `C:\Users\timzw\Desktop`
1.  Install [PortableApps](https://portableapps.com):
    1.  Change PortableApps settings:
        - **General:**
          - **Bold categories:** `enabled`
          - **Hide "Portable" in app names:** `enabled`
        - **Themes** > `PortableApps.com Flat Dark`
        - **Updater > Show updater startup errors:** `enabled`
        - **App Store > App Directory Settings > Show installed apps:**
          `enabled`
        - **Advanced:**
          - **Expand categories by default:** `enabled`
          - **Disable app splash screens (where supported):** `enabled`
          - **Start the menu minimized:** `enabled`
          - **Hide taskbar icon:** `enabled`
1.  Install [Google Drive](https://www.google.com/drive/download):
    1.  Change Google Drive settings:
        - **Sync** `D:\Virtual Machines\Shared` to Google Drive
        - **Mirror** files to `D:\Google Drive`
1.  Install [Discord](https://discord.com):
    1.  Change Discord settings:
        - **Voice & Video > Input Mode:** `Push to Talk`
          - **Shortcut:** `MOUSE4`
        - **Notifications > PTT Activate/Deactivate:** `disable`
        - **Game Overlay:**
          - **Toggle Overlay Lock:** `Shift+F2`
          - **Display Names:** `Only While Speaking`
          - **Display Users:** `Only While Speaking`
1.  Install [Steam](https://store.steampowered.com):
    1.  Change Steam settings:
        - **Storage:** add `D:\Steam`
          - Set `D:\Steam` as default
        - **In Game > Overlay shortcut key(s):** `Shift+F1`
1.  Install [Battle.net](https://us.shop.battle.net):
    1.  Change Battle.net settings:
        - **Settings > Downloads > Default Install Directory:** `D:\Battle.net`
1.  Install [Epic Games](https://store.epicgames.com): (no settings changes
    needed)
1.  Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads):
    1.  Change VirtualBox settings:
        - **General > Default Machine Folder:** `D:\VirtualMachines\Machines`
        - **Input > Virtual Machine > Host Key Combination:** `F11`
        - **Update > Check for Updates:** `enabled`
1.  Install [8GadgetPack](https://8gadgetpack.net):
    1.  ~~Install [PC Meter](http://addgadgets.com/pc_meter)~~ (PC Meter doesn't
        seem to work with modern CPUs, so use Core Temp instead)

        Install [Core Temp](https://www.alcpu.com/CoreTemp)
        1.  Change Core Temp settings:
            - **General > Start Core Temp with Windows:** `enabled`
            - **Display:**
              - **Start Core Temp minimized:** `enabled`
              - **Close Core Temp to the notification area:** `enabled`
            - **Notification Area > Icon only:** `enabled`
    1.  Change 8GadgetPack settings:
        - **Orientation:**
          - **Monitor:** `2`
          - **Show icon in taskbar:** `enabled`
        - **View:**
          - **Show buttons at top:** `disabled`
          - **Enable transparency:** `enabled`
    1.  Remove all gadgets
    1.  Add gadgets:
        - CPU Meter
          - **Display:**
            - **Size:** `125%`
            - **Show Current Domain/Username:** `OFF`
          - **Options:**
            - **Show CPU temperatures:** `ON (PC Meter)`
            - **Alert CPU Temperature:** `ON`
            - **Alerts Above (°C):** `80`
        - GPU Meter
          - **Options:**
            - **Select Method:** `Standalone`
            - **Alert GPU Temperature:** `ON`
            - **Alerts Above (°C):** `80`
          - **Display > Size:** `125%`
        - Network Meter
          - **Options:**
            - **Save Chart Data:** `OFF`
            - **Save IP Address:** `OFF`
          - **Display:**
            - **Size:** `125%`
            - **Internal IP > Interval (sec):** `60`
            - **External IP > Interval (min):** `60`
            - **Show Search:** `OFF`
        - Drives Meter
          - **Options:**
            - **Drive 1 (C) > Alerts Below:** `50 GB`
            - **Drive 2 (D):** `On`
            - **Drive 2 (D) > Alerts Below:** `500 GB`
          - **Display > Size:** `125%`
        - Clock
1.  Configure the Windows Taskbar:
    1.  Portable Apps
    1.  File Explorer
    1.  Chrome
    1.  Discord
    1.  Steam
    1.  Battle.net
    1.  Epic Games
    1.  VirtualBox
1.  Configure pinned Start items:
    1.  Calculator
    1.  Clock
    1.  Edge
    1.  Gaming (folder)
        1.  Battle.net
        1.  Discord
        1.  Epic Games
        1.  Steam
    1.  Google Chrome
    1.  Google Drive
    1.  VirtualBox
    1.  System (folder)
        1.  (Western Digital) Dashboard
        1.  File Explorer
        1.  Microsoft Store
        1.  Nvidia App
        1.  Nvidia Control Panel
        1.  Realtek Audio Console
        1.  Terminal
        1.  Windows Security
        1.  Windows Tools


TODO: disable iGPU:
- Right click Start button > Device Manager
- Display adapters > right click AMD Radeon Graphics > Disable
- https://www.reddit.com/r/LinusTechTips/comments/11ikxhp/new_pc_opening_steam_from_taskbar_is_slow


TODO: Microsoft Power Toys


Rainmeter:
1.  Download it
1.  Install it
1.  Right-click icon > Manage > Settings
    1.  Editor >
        `D:\PortableApps\PortableApps\Notepad++Portable\App\Notepad++\notepad++.exe`
    1.  Disable Dragging > `enabled`
1.
