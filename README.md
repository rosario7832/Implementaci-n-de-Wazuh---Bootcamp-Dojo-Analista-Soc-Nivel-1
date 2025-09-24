# Lab: SIEM with Wazuh

## Description
Practical implementation of an **open-source SIEM** in a local environment for educational and cybersecurity training purposes.

## Objectives

- Implement the **open-source SIEM Wazuh** in a local environment.
- Install log collection agents on devices or services.
- Become familiar with the main functionalities of the SIEM.
   
# Lab: SIEM with Wazuh

## Part I - Importing the Wazuh OVA

1.**Download the OVA from the official Wazuh website:**
   👉 [Wazuh Virtual Machine](https://documentation.wazuh.com/current/deployment-options/virtual-machine/virtual-machine.html)

2. **Open VirtualBox (or your preferred virtualization software).**
   
**Download VirtualBox from the [official Oracle VirtualBox website](https://www.virtualbox.org/).**

3. **Import the OVA:**
- In VirtualBox, go to **File > Import Appliance**.  
- Select the downloaded `.ova` file.  
- Review and adjust the hardware settings (CPU, RAM, disk) according to available resources.  
<img src="https://i.imgur.com/3Z1ypRp.png" height="75%" width="80%"/>
4. **Start the Wazuh virtual machine.**

<img src="https://i.imgur.com/vynkWp6.png" height="75%" width="70%"/>

- Username: `wazuh-user`  
- Password: `wazuh`
  
***Validate the IP address assigned to the Wazuh machine using the command: `ip addr`***
 
 <img src="https://i.imgur.com/4lQx3WD.png" height="75%" width="70%"/>
**Note:** The IP to use is the one identified as `inet` on the `eth0` interface.


5. **Access the Wazuh web interface:**
   - Once the VM is running, open your browser and navigate to:  
     ```
     https://192.168.50.206
     ```
**Credentials to log in as administrator:**
- Username: `admin`  
- Password: `admin`


 <img src="https://i.imgur.com/GYQSldS.png" height="75%" width="70%"/>

Once you log in to **Wazuh**, you will have access to multiple resources typical of a **SIEM** and will be able to view each connected agent, as shown in the following image.

To deploy an agent, it is recommended to consult the [official Wazuh documentation](https://documentation.wazuh.com/current/deployment-options/index.html), as the procedure will depend on the device where it needs to be installed.

 <img src="https://i.imgur.com/Cgosn0H.png" height="75%" width="90%"/>
