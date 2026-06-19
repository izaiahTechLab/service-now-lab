# Project Walkthrough 🗺️

---

### Step 1 — Creating Users in ServiceNow

Users were provisioned using a standardized corporate naming convention (`firstname.faction`) to match the organizational structure of the Active Directory enterprise environment (e.g., `brodie.magma`).

![Creating Users](Creating%20Users%20Service%20Now.jpg)

---

### Step 2 — Creating Assignment Groups

Five distinct assignment groups were created within ServiceNow to mirror the enterprise factions established in the AD lab environment: **TeamAqua**, **TeamGalactic**, **TeamMagma**, **TeamPlasma**, and **TeamRocket**.

![Created Groups](Created%20Groups%20in%20ServiceNow..jpg)

---

### Step 3 — Incident Triage & Simulation

To test the cross-platform integration, an end-to-end password lockout scenario was simulated. An incoming incident ticket was generated and triaged within ServiceNow to log the user account issue and track its lifecycle.

![Mars Incident](Mars%20Incident.jpg)

---

### Step 4 — Setting User Passwords

Following initial user record creation and incoming ticket verification, account passwords were configured using the **Set Password** utility. Security controls were set to "Password never expires" strictly for isolated lab testing purposes.

![Creating Password](Creating%20Password.jpg)
![Assigning Groups](Assigning%20Groups.jpg)

---

### Step 5 — Account Remediation (Active Directory)

Following help desk verification protocols, administrative actions were shifted to the Windows Server 2022 environment. The user's credentials were formally reset, updated, and unlocked within the Active Directory domain to remediate the lockout.

![Mars Password Reset](Mars%20Password%20Reset.jpg)
![Mars Password Change](Mars%20Password%20Change.jpg)

---

### Step 6 — Incident Resolution in ServiceNow

With the Active Directory remediation completed and authentication verified, the incident ticket was formally updated to a **Resolved** status within the ServiceNow PDI, closing out the service loop.

![Mars Incident Resolved](Mars%20Incident%20Resolved.jpg)
