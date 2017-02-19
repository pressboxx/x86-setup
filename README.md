#Configuring PressBoxx on Gigabyte Brix

- Link to: [Gigabyte Brix GB-BXBT-2807](http://www.gigabyte.com/Mini-PcBarebone/GB-BXBT-2807-rev-10)

##Install Ubuntu 
- Link to: [Ubuntu 16.04 LTS Server](http://releases.ubuntu.com/16.04/)

###Installation Process
#### Language, Keyboard, Location
- Language: `English`
- Select: `Install Ubuntu Server`
- Language: `English - English`
- Location: `United States`
- Detect Keyboard Layout: `<No>`
- Country of Origin for Keyboard: `English (US)`
- Keyboard Layout: `English (US)`

#### Network Configuration
- Configuring the network with DHCP: `<Cancel>`
- Network Autoconfiguration Failed: `<Continue>`
- Configuring the network: `Configuring network manually`
- IP Address: `192.168.1.175`  _(Or something else that works for your network)_
- Netmask: `255.255.255.0`
- Gateway: `192.168.1.1`  _(Or something else that works for your network)_
- Name Server Addresses: `8.8.8.8 8.8.4.4` _(note the space in the middle)_
- Hostname: `boxx`
- Domain name: `boxx.local` _(Not sure this is best answer. Is it?)_

#### User and Boxx Identity
- Full name for the new user: `PressBoxx`
- Username for your account: `pressboxx`
- Choose a password for the new user: `boxx`
- Re-enter password to verify: `boxx`
- Use weak password: `<Yes>`
- Encrypt your home directory: `<No>`
- Setting up the clock: _Wait..._
- Select your time zone: `Eastern`

#### Mounting and Formatting Drives
- Unmount partitions that are in use: `<Yes>`
- Partitioning Method: `Guided - use entire disk`
- Select Disk to Partition: _Select the one you want to install Ubuntu to_
- Partition Disks: `Finish partitioning and write changes to disk` _(May not appear)_
- Write changes to disks: `<yes>`
- _Wait for a long time..._

#### Repository and Software
- HTTP proxy information (blank for none): _Leave blank_ 
- Configuring Apt: `<Cancel>`
- How do you want to manage upgrades on this system? `No automatic upgrades`
- Choose Software to install:
	- [*] Manual package selection
	- [*] Samba file server
	- [*] Standard system utilities
	- [*] OpenSSH server
- _Wait for a really long time..._	

#### Booting and Wrapup
- Install the GRUB boot loader to the master boot record: `<Yes>`
- Installation Complete: _Remove USB drive w/Ubuntu installer then_ `<Continue>`

##Install Network Manager

- Mount thumb drive with local repo
	- Configure to use local repo	
- Install Network Manager
		
		sudo apt-get install network-manager
	
- Restart Network Manager

		sudo service network-manager restart

- 

- Run `nmtui` _(Network Manager Text UI)_

	- Activate a WiFi network
	

	
# x86-setup
