VirtualBox Installation Report

1. Objective
To install Oracle VirtualBox on my host system and verify that it runs correctly.  
This tool will be used to create isolated virtual machines for my cybersecurity lab.


2. Host System Details
- Host OS: Windows 10 (or Linux / macOS – write your actual one)
- Processor: Intel Core i5 (write your actual one)
- RAM: 8 GB
- Virtualization: Enabled in BIOS


3. Installation Steps
1. Downloaded VirtualBox from the official website:  
   https://www.virtualbox.org/wiki/Downloads
2. Selected installer for my OS (Windows host).
3. Ran the setup → followed default options (Next → Next → Install).
4. Allowed network adapter installation when prompted.
5. After installation, opened **Oracle VM VirtualBox Manager** successfully.


4. Network Configuration
- Opened **File → Host Network Manager**.
- Created a **Host-only Adapter** named `vboxnet0`.
- Default settings:
  - IPv4: 192.168.56.1
  - DHCP: Enabled
- This adapter will allow communication between my Kali (attacker) and Metasploitable (target) VMs.


 5. Verification
- Checked that VirtualBox runs without errors.
- Verified network adapters from command line:
  - `ipconfig` (Windows) or `ifconfig` (Linux/Mac)
- Confirmed presence of `VirtualBox Host-Only Network`.


 6. Screenshots
(Save these in `/screenshots/` folder)
- Screenshot 1: VirtualBox installation complete window.
- Screenshot 2: VirtualBox Manager main window.
- Screenshot 3: Host-only adapter settings.



7. Conclusion
VirtualBox has been successfully installed and configured with a Host-only adapter.  
It is ready for creating and running Kali Linux and Metasploitable virtual machines for my cybersecurity lab.
