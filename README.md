# How-to-create-azure-virtual-machine
- step by step guide to creating azure virtual machine

----------------------------------------------------------------------------------------------
Environments used and srevices used

- Azure

----------------------------------------------------------------------------------------------

- Accessing the Azure Platform

- Starting the Virtual Machine Creation Process

- Input Basic Setup Information

- Configuring Storage

- Networking Setup

- Setting Management Options

- Advanced Configuration (Optional)

- Assign Tags (Optional)

-  Connecting to Your Virtual Machine
 
-  Deleting the Virtual Machine (Optional)
 ______________________________________________________________________________________________

<img width="984" alt="Screen Shot 2025-03-21 at 8 05 22 PM" src="https://github.com/user-attachments/assets/de03413e-70ea-42ed-b3b8-68b00077ee50" />
Step 1: Access the Azure Portal
Open your browser and go to Azure Portal.

Log in using your Microsoft or Azure Active Directory credentials.
------------------------------------------------------------------------------------------------

<img width="1018" alt="Screen Shot 2025-03-21 at 8 20 29 PM" src="https://github.com/user-attachments/assets/a0ee5d6b-623c-4a41-9e6b-dacdbc1c0ec3" />
Step 2: Initiate Virtual Machine Creation
locate and click "Create a resource". Alternatively, you can search for Virtual Machine in the top search bar.

Select "Virtual Machine" from the available options.

-------------------------------------------------------------------------------------------------

<img width="1030" alt="Screen Shot 2025-03-21 at 8 22 54 PM" src="https://github.com/user-attachments/assets/c4d019c4-1c49-43ff-b6bd-d71a5541bb48" />
Step 3: Set Up Basic Information
Subscription: Choose the subscription associated with your Azure account.

Resource Group: Pick an existing group or create a new one for organizational purposes.

VM Name: Give your virtual machine a name.

Region: Pick the Azure region for deploying the machine, considering latency and proximity to users.

Image: Choose the OS image, whether it's Linux (Ubuntu) or Windows (Windows Server).

VM Size: Select an appropriate size based on required resources like CPU and memory.

Login Options: Choose between using a password or SSH key for access (this will vary depending on whether you're using Linux or Windows).

Inbound Ports: Allow specific ports like SSH (22) or RDP (3389) to enable remote access.

----------------------------------------------------------------------------------------------------

<img width="1013" alt="Screen Shot 2025-03-24 at 8 40 27 AM" src="https://github.com/user-attachments/assets/74019151-2930-4609-bb9b-da4e1a32d148" />


Step 4: Configure Storage Options
OS Disk Type: Select the disk type ( Standard HDD or SSD) for your VM’s operating system disk.

Optionally, add data disks if your project requires additional storage space.

Continue to the "Networking" section.

-----------------------------------------------------------------------------------------------------

<img width="1020" alt="Screen Shot 2025-03-24 at 8 42 16 AM" src="https://github.com/user-attachments/assets/e0ad0bd9-6014-44c7-aba9-a8b78e50cec6" />


Step 5: Set Up Networking Details
Virtual Network (VNet): Either choose an existing virtual network or create a new one. This helps in managing network configurations.

Subnet: Choose or create a subnet within your virtual network.

Public IP Address: Decide if you want a dynamic or static public IP for accessing the machine remotely.

Network Security Group (NSG): This defines the firewall rules to control the inbound/outbound traffic to your VM.

Once finished, click "Next: Management".

------------------------------------------------------------------------------------------------------

<img width="1012" alt="Screen Shot 2025-03-24 at 8 46 58 AM" src="https://github.com/user-attachments/assets/8d522368-397f-45dd-9d5e-0346b64a8e8a" />


Step 6: Management Settings
Monitoring Options: Enable monitoring via Azure Monitor to get insights on VM health and performance.

Boot Diagnostics: This is an optional feature that can capture screenshots of the VM's boot sequence.

Auto-shutdown: Optionally, enable auto-shutdown at a specific time to save costs when not in use.

Move on to "Next: Advanced".

---------------------------------------------------------------------------------------------------------

<img width="1011" alt="Screen Shot 2025-03-24 at 8 48 37 AM" src="https://github.com/user-attachments/assets/032ed3e4-ff21-4352-98e9-2cdc61812676" />


Step 7: Advanced Settings (Optional)
If needed, apply specific extensions or configure additional custom settings for your VM. click "Next: Tags".

----------------------------------------------------------------------------------------------------------

<img width="1012" alt="Screen Shot 2025-03-24 at 8 49 34 AM" src="https://github.com/user-attachments/assets/236b01a5-3154-4266-b9fc-ab886533d56b" />


Step 8: Apply Tags (Optional)
Tags allow you to organize resources for better management and reporting (e.g., adding Environment: Development).

After adding any tags, click "Next: Review + Create".

-----------------------------------------------------------------------------------------------------------

<img width="1012" alt="Screen Shot 2025-03-24 at 8 49 51 AM" src="https://github.com/user-attachments/assets/74207282-2375-4529-a267-2895bb96c589" />


<img width="1016" alt="Screen Shot 2025-03-24 at 8 50 03 AM" src="https://github.com/user-attachments/assets/f4e5d147-b6f0-4f2b-8fbe-f9d47d24979e" />


Step 9: Review Configuration
Review all choices to ensure everything is set up correctly.

Once verified, click Create. Azure will validate your choices before starting the deployment process. It may take several minutes for the VM to be created.

------------------------------------------------------------------------------------------------------------

<img width="1016" alt="Screen Shot 2025-03-24 at 8 50 03 AM" src="https://github.com/user-attachments/assets/d2491347-3443-4a2c-b6b9-a8792801a352" />


Step 10: Connect to Your Virtual Machine
After successful deployment:

Go to the "Virtual Machines" section of the portal.

Find your VM and click on it.

Click "Connect" to access your VM using RDP (for Windows) or SSH (for Linux). You'll need the VM’s IP address and credentials to log in.

----------------------------------------------------------------------------------------------------------------

<img width="1022" alt="Screen Shot 2025-03-24 at 8 55 19 AM" src="https://github.com/user-attachments/assets/cc97d577-45b2-413e-b7b6-2504415dcf89" />


<img width="1021" alt="Screen Shot 2025-03-24 at 8 55 36 AM" src="https://github.com/user-attachments/assets/7a051639-49b7-4a0c-91ff-a65c30009c25" />


<img width="1018" alt="Screen Shot 2025-03-24 at 8 55 49 AM" src="https://github.com/user-attachments/assets/f1853519-2b88-427c-a2c9-c73a3da21286" />



Step 11: Deletion or stop Resources (Optional)
Once your work is complete, remember to delete the VM to avoid incurring additional charges. If you want to continue using the VM for later, you can press the stop button so you wont be charged. Go to your VM’s page and select Delete if you are complete.
Always go back to the VM page to make sure the VM was deleted.


