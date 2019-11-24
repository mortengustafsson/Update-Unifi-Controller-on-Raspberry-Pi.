# Update Unifi controller running on a Raspberry Pi.

### Update your Raspberry Pi With Raspbian:

1. Update the repository package list: 

    `sudo apt update`

2. Run the upgrade command: 

    `sudo apt dist-upgrade`

3. Follow any prompts.

4. Clean up: 

    `sudo apt clean`

5. Reboot:

    `sudo reboot`

### Update your Controller:
1. Make a backup for your Unifi Controller. 

2. Find the neweste software build for Debian/Ubuntu Linix at: [Unifi Download](https://www.ui.com/download/unifi/)
and copy the direct url (ex: https://dl.ui.com/unifi/5.12.35/unifi_sysvinit_all.deb)

3. From the terminal via ssh or directly from your Raspberry Pi, download the unifi package with.

    `wget *Inset the direct url*`
    
    *`ex: wget https://dl.ui.com/unifi/5.12.35/unifi_sysvinit_all.deb`*

4. Install the package.

    `sudo dpkg -i unifi_sysvinit_all.deb`

5. Reboot.

    `sudo reboot`

