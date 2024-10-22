# Installing TrollStore (TrollRestore) on iPad Air 2

## Prerequisites

- iPad Air 2 running iPadOS 15.2 or later
- Latest version of Python 3 installed
- Latest version of iTunes (for Windows users)
- The appropriate TrollRestore version for your platform:
  - **Windows**: `TrollRestore.exe`
  - **Apple Silicon Macs**: `TrollRestore_macOS_arm64.zip`
  - **Intel-based Macs**: `TrollRestore_macOS_amd64.zip`
  - **Linux**: `TrollRestore_Linux.zip`

> **Note:** If you’re using macOS or Linux, extract the downloaded TrollRestore `.zip` file before continuing.

Make sure to disable **Find My** before proceeding, as this method uses a modified backup. You can re-enable **Find My** after installation is complete.

---

## Installation Instructions

### macOS/Windows

1. Connect your iPad to your computer and ensure it’s trusted to allow file access.
2. Open **File Explorer** (Windows) or **Finder** (macOS) and navigate to the TrollRestore file (usually in your **Downloads** folder).
3. Double-click the TrollRestore file to run it.
   - **Intel Mac Users**: If the file is not notarized, either hold **Control** while double-clicking or attempt to open it normally, then go to **System Settings > Privacy & Security** and select **Open Anyway**.
4. When prompted, enter the name of a system app to overwrite and press **Enter**.
   - If unsure, overwrite the **Reminders** app by typing `Reminders`.

Once the process starts, there will be no on-device feedback, but your iPad will reboot automatically once it’s done.

---

### Linux

If you’re using Linux or prefer using the Linux method on other platforms, follow these steps:

#### Install Dependencies

1. Open a terminal on your computer.
2. Navigate to the TrollRestore folder by running:
   ```bash
   cd ~/Downloads/TrollRestore_Linux
   ```
3. Install the necessary dependencies by running:
   ```bash
   pip3 install -r requirements.txt
   ```
   Follow the instructions in the terminal to complete the installation.

#### Run TrollRestore

1. Connect your iPad to your computer and ensure it’s trusted.
2. In the terminal, run:
   ```bash
   python3 trollstore.py
   ```
3. When prompted, enter the name of a system app to overwrite and press **Enter**.
   - If unsure, overwrite the **Reminders** app by entering `Reminders`.

As with other platforms, there will be no visual indication during the process, and your device will reboot once the TrollStore Helper is restored.

---

## Final Steps

1. After your device reboots, unlock it and open the app you chose to overwrite (e.g., **Reminders**).
2. Tap **Install TrollStore** within the app.

Your device will respring, and TrollStore will be installed.

### Installing Persistence Helper

1. Open the **TrollStore** app from your home screen.
2. Go to **Settings** and select **Install Persistence Helper**.
3. Choose **Reminders** from the list of apps.

At this point, TrollStore and the Persistence Helper should be fully installed on your iPad Air 2.
