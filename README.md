

# Scanning for Vulnerabilities Project - Using a DISA STIG Scan Template

This project is about Scanning a Windows VM: Authenticated vs. Unauthenticated

![Scanning Windows Authenticated vs Unauthenticated](https://github.com/user-attachments/assets/0475b1a7-3e0e-40a8-9341-08d97ee65d6e)

---
# Tools & Technology:
- Tenable (enterprise vulnerability management platform)
- Azure Virtual Machine


---
# Table of contents

- [Step 1) Create a Windows virtual machine in the Azure portal](#step-1-create-a-windows-virtual-machine-in-the-azure-portal)
- [Step 2) Log into the VM and disable the Windows Firewall](#step-2-log-into-the-vm-and-disable-the-windows-firewall)
- [Step 3) Run a PowerShell command:](#step-3-run-a-powershell-command)
- [Step 4) Create a Network Security Group](#step-4-create-a-network-security-group)
- [Step 5) Login to tenable](#step-5-login-to-tenable)
- [Step 6) Run a Basic Scan: Unauthenticated](#step-6-run-a-basic-scan-unauthenticated)
- [Step 7) Run a Basic Scan: Authenticated](#step-7-run-a-basic-scan-authenticated)
- [Difference in Scan Duration](#difference-in-scan-duration)

---


### Step 1) Create a Windows virtual machine in the Azure portal

#### Configure the Basics Tab: 

<img width="600" alt="vm1" src="https://github.com/user-attachments/assets/152b83d4-1303-49df-b467-df2170872c0b" />


#### Configure the Disks Tab:

<img width="600" alt="vm2" src="https://github.com/user-attachments/assets/6d3819c9-b532-45f5-a509-2d89942ffbd6" />


#### Configure the Setup Networking:

<img width="600" alt="vm3" src="https://github.com/user-attachments/assets/af658652-0581-41c0-bcdf-e208ed950b41" />


#### Review + Create:
<img width="600" alt="vm5" src="https://github.com/user-attachments/assets/d65013ec-3c25-426d-ba6a-cbe3e0f3351f" />


#### Deployment:
<img width="600" alt="vm7" src="https://github.com/user-attachments/assets/9e8c5e4a-3348-47c4-9565-a3958e21ee9b" />


---
### Step 2) Log into the VM and disable the Windows Firewall 

#### Bastion Connection:

<img width="600" alt="rdp" src="https://github.com/user-attachments/assets/cbed6adf-9061-4fe8-a49e-5e4061ac9ebb" />


#### Disable Windows Firewall 

<img width="600" alt="wf" src="https://github.com/user-attachments/assets/b2cc7376-5bc6-4cf1-82ad-e549a2c393ee" />

#### Create Administrator user account & assign to administrators group

<img width="600" alt="wf" src="https://github.com/user-attachments/assets/d3ed6359-bbd9-4332-9515-e873b4f354fd" />

#### Assign to administrators group

<img width="600" alt="wf" src="https://github.com/user-attachments/assets/4301bbb7-6801-4595-9106-5ed69624cdad" />

#### Enable Guest Account

<img width="600" alt="wf" src="https://github.com/user-attachments/assets/9fa00fea-21ea-45dc-8de9-38ead71fc399" />


#### Assign Guest to administrators group

<img width="600" alt="wf" src="https://github.com/user-attachments/assets/2d124c00-76c0-47c3-88f2-3c2c16a29e86" />
---


### Step 3) Run a PowerShell command: 
This command sets a registry key that allows local accounts to connect remotely with full administrative privileges without requiring elevation. 

<img width="600" alt="powershell" src="https://github.com/user-attachments/assets/7dad2e05-ecd1-4632-8203-72e80b47ea58" />

---

### Step 4) Create a Network Security Group
#### Inbound Security Rule to allow all traffic

<img width="600" alt="powershell" src="https://github.com/user-attachments/assets/cf486cee-1961-4e11-97e0-0a66e71a7028" />

#### Test the NSG using Ping Command: 

<img width="600" alt="ping command" src="https://github.com/user-attachments/assets/ee909eb2-e99b-48c9-abc9-823685faf7fa" />

---

### Step 5) Login to tenable

<img width="600" alt="tenablelogin" src="https://github.com/user-attachments/assets/65aa3c73-113b-4b85-8b79-de3a142d4e4b" />

---
### Step 6) Run a Basic Scan: Unauthenticated
#### Configure Scan basic settings

<img width="600" alt="scan" src="https://github.com/user-attachments/assets/3acb6537-65cf-4df7-8bdc-8ebb6543ceea" />

#### Scan Results
<img width="600" alt="scan results" src="https://github.com/user-attachments/assets/fa337ccc-ab06-4b78-880e-982fa3ddeab1" />

#### Tenable Vulnerability Management Report
[Tenable Vulnerability Management Report - UnAuthenticated](https://drive.google.com/file/d/11Gtks85b8GboGLymJlLQIehsnZ-NUOhL/view?usp=sharing)


---

### Step 7) Run a Basic Scan: Authenticated
#### Configure Credentials

<img width="600" alt="credentials" src="https://github.com/user-attachments/assets/d91cbe35-6577-434a-99b7-23db1c4b0ac6" />

#### Scan Results
<img width="600" alt="scan results" src="https://github.com/user-attachments/assets/9b1c8f8e-0ff2-45d8-80a6-c801e99d5fe8" />

#### Tenable Vulnerability Management Report
[Tenable Vulnerability Management Report - Authenticated](https://drive.google.com/file/d/1crKF3tikhzv756wu7t05l9pV3MXs9rhR/view?usp=sharing)


---
### Difference in Scan Duration

![scantime](https://github.com/user-attachments/assets/c2f715f4-fbdb-429e-9fd5-d9aa93477e94)
