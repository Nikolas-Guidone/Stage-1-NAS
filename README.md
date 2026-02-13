# Stage 1 - Physical Build and Installation of the OS

## Objective

Overview of the physcial build of my NAS as well as choosing and installing the Operating System

---

## Date of start and completion

11/2025 - 12/2025

---

## Physical Build

I chose to recycle old hardware lying around in order to build my first NAS. I used an old Dell XPS 8700 workstation as the basis and external shell for my project. Knowing that this hardware is older generation, I also got 2x WD Red Plus 4 TB hard drives, as well as an Samsung 870 EVO 500GB Internal SSD. I chose to install TrueNAS (OS) onto the 500GB SSD for a few advantages, such as faster boot / response time, more reliability vs a hard drive, and allows various services and applications to pull cached data faster. Initially, for testing purposes, my NAS consisted only of a Seagate 1TB Desktop HDD (the original stock drive) and the SSD (boot drive). Once the build was complete, I used my personal computer to download and install Rufus — an open source application used for creating bootable USB drives — to install TrueNAS onto a USB drive. Once installed on the drive, it was a simple plug and play to install the OS onto the NAS. As the OS was installing, I went into my router's settings and blocked off a range of 20 IP addresses so that the router did not assign any device one of those 20 IPs. Once installation was complete, I used the terminal with an attached keyboard and mouse to set a static IP address for the NAS that fell within the blocked off range. This ensures consistent connectivity and access, as I now will always know the IP to connect to for the Web UI. Initial testing consisted only of setting up a pool on the hard drive, setting up an SMB share, and moving files to and from the NAS with my PC. Once I was familiarized with the Web UI and SMB, I added in the 2x WD Red Plus 4 TB hard drives to the NAS. I decided, since there wasn't going to be data stored on the NAS right away that would be crucial if lost, to use one drive for an app pool, and the other drive was going to be the basis of my storage, where all important files would end up. Due to limited hardware, this resulted in not enough drives for any redundancy, hence why I chose not to store any crucial data on the drives. 
