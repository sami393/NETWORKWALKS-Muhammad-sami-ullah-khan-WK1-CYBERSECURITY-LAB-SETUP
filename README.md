# Cybersecurity Lab Environment Setup

Building an isolated virtual lab for penetration testing and ethical hacking practice as part of the Networkwalks Academy Cybersecurity Internship Program (Batch B083).

## 📌 Project Overview
This project focuses on setting up a secure, isolated cybersecurity testing laboratory on a local machine using Oracle VirtualBox. The environment is configured with a dedicated attacking machine (Kali Linux) to simulate real-world penetration testing workflows safely without interfering with the host network.

## 💻 Host System Specifications
* **Operating System:** Windows 10 / 11
* **Processor:** [e.g., Intel Core i5 / AMD Ryzen 5]
* **RAM:** [e.g., 16 GB]
* **Storage:** [e.g., 512 GB SSD]

## 🛠️ Network Architecture & Configurations
The lab environment utilizes a highly controlled, custom virtual network architecture:
* **Hypervisor Platform:** Oracle VirtualBox (Latest Version)
* **Attacking Machine:** Kali Linux (Rolling Release)
* **Network Mode:** Custom NATNetwork
* **Network Subnet Prefix:** `10.0.0.0/24`
* **Kali Linux Target IP:** `10.0.0.2` (Manually configured static IP)
* **Gateway IP:** `10.0.0.1`
* **DNS Server:** `8.8.8.8` (Google Public DNS)
* **Guest Integration Features:** Shared Clipboard & Drag-and-Drop enabled; Shared host `/downloads` folder mapped.

## 🚀 Step-by-Step Implementation Flow

### Phase 1: Environment Preparation
1. Downloaded and configured the virtualization engine using Oracle VirtualBox.
2. Verified local archive management utilities using 7-Zip to extract the required appliance packages.

### Phase 2: Virtual Network Infrastructure Setup
1. Opened VirtualBox Network Manager and generated a custom **NATNetwork**.
2. Adjusted the global network preferences to match the designated subnet mask address (`10.0.0.0/24`) and explicitly verified that the localized DHCP service was active.

### Phase 3: Attacking Machine Importation & Optimization
1. Imported the pre-configured Kali Linux virtual appliance into the VirtualBox inventory.
2. Modified individual VM hardware options to authorize shared clipboard bidirectionality and drag-and-drop file features.
3. Created a persistent shared directory connecting the virtual instance to the host OS downpour point (`/downloads`).

### Phase 4: Network Target Interface Configuration
1. Initiated the Kali system instance and navigated into the advanced network connection interface profiles.
2. Transitioned the automated connection method to manual handling to apply a fixed IP configuration of `10.0.0.2/24` pointing towards the base operational gateway `10.0.0.1`.
3. Validated internet availability directly from the command terminal environment.
4. Generated a fallback environment state baseline using a system snapshot recovery anchor point.

## 📸 Lab Proof & Screenshots

### 1. VirtualBox Global NATNetwork Configuration
<img width="959" height="507" alt="Screenshot 2026-10-29 075443" src="https://github.com/user-attachments/assets/b08f4497-7f4c-4cb4-94f8-33541123b609" />


### 2. Kali Linux Advanced VM Adaptation Properties
<img width="584" height="380" alt="Screenshot 2026-10-29 075339" src="https://github.com/user-attachments/assets/2fd02521-645b-4764-8ef3-7d82e539d066" />



### 3. Static IP Assignment Verification
<img width="348" height="269" alt="Screenshot 2026-10-29 080504" src="https://github.com/user-attachments/assets/50929085-4a7f-4310-947d-af7579bfe4a5" />


### 4. Operational Network Connectivity Validation Test
<img width="458" height="299" alt="Screenshot 2026-10-29 080604" src="https://github.com/user-attachments/assets/22a126db-32d5-469e-b047-d1e69e249ba5" />

