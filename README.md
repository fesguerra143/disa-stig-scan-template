

# DISA STIG Compliance Project

This project is about Scanning a Windows VM using DISA STIG Compliance

![Scanning Windows DISA STIG Compliance](https://github.com/user-attachments/assets/0475b1a7-3e0e-40a8-9341-08d97ee65d6e)

---
# Tools & Technology:
- Tenable (enterprise vulnerability management platform)
- Azure Virtual Machine


---
# Table of contents

- [Step 1) Create a Windows virtual machine in the Azure portal](#step-1-create-a-windows-virtual-machine-in-the-azure-portal)
- [Step 2) Log into the VM and disable the Windows Firewall](#step-2-log-into-the-vm-and-disable-the-windows-firewall)
- [Step 3) Administrator Account & Assign Group](#step-3-administrator-account--assign-group)
- [Step 4) Guest Account & Assign Group](#step-4-guest-account--assign-group)
- [Step 5) Login to tenable](#step-5-login-to-tenable)
- [Step 6) Create a Scan Template](#step-6-create-a-scan-template)
- [Step 7) Create a Custom Scan](#step-7-create-a-custom-scan)

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

---
### Step 3) Administrator Account & Assign Group

#### Create Administrator user account 

<img width="600" alt="wf" src="https://github.com/user-attachments/assets/d3ed6359-bbd9-4332-9515-e873b4f354fd" />

#### Assign to administrators group

<img width="600" alt="wf" src="https://github.com/user-attachments/assets/4301bbb7-6801-4595-9106-5ed69624cdad" />

---

### Step 4) Guest Account & Assign Group
#### Enable Guest Account

<img width="600" alt="wf" src="https://github.com/user-attachments/assets/9fa00fea-21ea-45dc-8de9-38ead71fc399" />


#### Assign Guest to administrators group

<img width="600" alt="wf" src="https://github.com/user-attachments/assets/2d124c00-76c0-47c3-88f2-3c2c16a29e86" />

---

### Step 5) Login to tenable

<img width="600" alt="tenablelogin" src="https://github.com/user-attachments/assets/65aa3c73-113b-4b85-8b79-de3a142d4e4b" />

---
### Step 6) Create a Scan Template
#### Configure Scan Basic settings

<img width="600" alt="scan" src="https://github.com/user-attachments/assets/d4250fe1-8622-492b-8d4c-1e3886e99b31" />

#### Configure Scan Discovery settings

<img width="600" alt="scan" src="https://github.com/user-attachments/assets/59c72b13-4c4a-47ad-8e52-d8a6e93ffb35" />


#### Configure Scan Assessment settings

<img width="600" alt="scan" src="https://github.com/user-attachments/assets/a8059fd5-dfe6-4d70-b22c-a7969569a71f" />


#### Configure Scan Credentials settings

<img width="600" alt="scan" src="https://github.com/user-attachments/assets/a8e8a96e-186d-4556-8a2d-49728dde31c7" />

#### Configure Scan Compliance settings

<img width="600" alt="scan" src="https://github.com/user-attachments/assets/4ace1c7b-e033-42bd-bcb7-3583e1a36e17" />


#### Configure Scan Plugins settings

<img width="600" alt="scan" src="https://github.com/user-attachments/assets/9fbe50c2-8b2c-4e97-a158-e34384fad8ae" />


---

### Step 7) Create a Custom Scan

#### Select a DISA STIG Template

<img width="600" alt="scan" src="https://github.com/user-attachments/assets/4f4080e2-8a6f-478c-bbb8-d03fc46a32a9" />


#### Configure Scan Basic settings

<img width="600" alt="credentials" src="https://github.com/user-attachments/assets/18a0ca1f-7065-4e2a-9d10-8c28267efaf0" />


#### Scan Results 

##### Vulns by Plugin
<img width="600" alt="scan results" src="https://github.com/user-attachments/assets/a4f25d56-2ffd-4694-9bda-058c08fba39a" />

##### Audits
<img width="600" alt="scan results" src="https://github.com/user-attachments/assets/fd8d6565-aef6-47c9-aed9-bb3227d63248" />


##### Vulns by Asset
<img width="600" alt="scan results" src="https://github.com/user-attachments/assets/89386387-01af-4017-a7c2-2a4ee8ca4ad6" />


##### Remediations
<img width="600" alt="scan results" src="https://github.com/user-attachments/assets/6b0af59f-559b-42c1-9015-365ddbbd5e6e" />


##### History
<img width="600" alt="scan results" src="https://github.com/user-attachments/assets/2cf0f6bb-51c9-4052-9649-7a3049937a0e" />

#### Tenable Vulnerability Management Report
[Tenable Vulnerability Management Report](https://drive.google.com/file/d/1wsiYlNjNFqvXqji4pbG02z2_a-n1-Hs_/view?usp=drive_link)


---

