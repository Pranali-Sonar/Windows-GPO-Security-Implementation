# Windows GPO Security Implementation

## 📌 Project Overview

This project demonstrates the implementation of **Group Policy Objects (GPO)** in a **Windows Server Active Directory Environment** to centrally manage and restrict user access on domain-joined client machines.

The project was performed using **VMware Workstation**, where a Windows Server acted as the **Domain Controller** and a Windows Client was joined to the domain. Security policies were configured and enforced through Group Policy Management.

---

## 🎯 Objective

To implement Group Policy Objects (GPO) in a Windows Server Active Directory environment and restrict access to sensitive system utilities such as:

* Task Manager
* Control Panel
* Registry Editor

This project showcases centralized administration and security policy enforcement in an enterprise environment.

---

## 🛠️ Technologies Used

* VMware Workstation
* Windows Server
* Windows Client
* Active Directory Domain Services (AD DS)
* Group Policy Management (GPMC)

---

## 🏗️ Environment Setup

```text
Windows Server (Domain Controller)
            │
            │
Windows Client Machine
```

The client machine was joined to the Active Directory domain, allowing policies configured on the Domain Controller to be applied centrally.

---

## ⚙️ Implementation Steps

### 1. Configure Active Directory Domain Services

* Set up Windows Server as a Domain Controller.
* Create and configure the Active Directory domain.

### 2. Join Client Machine to Domain

* Connect the Windows Client to the domain.
* Verify successful domain membership.

### 3. Create and Configure Group Policy Object

* Open Group Policy Management Console (GPMC).
* Create a new Group Policy Object (GPO).

### 4. Apply Security Restrictions

Configured policies to:

#### 🔒 Disable Task Manager

Prevent users from opening Task Manager.

#### 🔒 Disable Control Panel

Restrict access to Control Panel settings.

#### 🔒 Disable Registry Editor

Prevent modifications to the Windows Registry.

### 5. Update Policies

Run:

```cmd
gpupdate /force
```

to immediately apply the configured policies.

### 6. Verify Policy Enforcement

Validate restrictions on the client machine.

---

## ✅ Results

Successfully implemented Group Policy restrictions from the Domain Controller.

After applying the policies:

* Task Manager access was blocked.
* Control Panel access was blocked.
* Registry Editor access was blocked.

The restrictions were enforced centrally through Active Directory Group Policy.

---

## 📚 Key Learning Outcomes

* Active Directory Administration
* Domain Management
* Group Policy Management
* Windows Server Administration
* Centralized Security Enforcement
* Enterprise User Access Control

---

## 🚀 Future Enhancements

* USB Device Restrictions
* Folder Redirection
* Software Deployment via GPO
* Password Policies
* Login Scripts
* Windows Firewall Management through GPO

---

## 👩‍💻 Author

**Pranali Kiran Sonar**

* GitHub: https://github.com/Pranali-Sonar
* LinkedIn: https://www.linkedin.com/in/pranali-kiran-sonar

---

## 📄 Project Documentation

Detailed step-by-step screenshots and implementation process are included in the project PDF documentation available in this repository.
