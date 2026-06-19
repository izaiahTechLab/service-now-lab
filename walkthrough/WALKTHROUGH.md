# Project Walkthrough 🎫

---

## Step 1 — Creating Users in ServiceNow
Users were provisioned using a standardized corporate naming convention (`firstname.faction`) to match the organizational structure of the Active Directory enterprise environment (e.g., `brodie.magma`).

![Creating Users](Creating_Users_Service_Now.jpg)

---

## Step 2 — Setting User Passwords
Following initial user record creation, account passwords were configured using the **Set Password** utility. Security controls were set to "Password never expires" strictly for isolated lab testing purposes.

![Creating Password](Creating_Password.jpg)

---

## Step 3 — Creating Assignment Groups
Five distinct assignment groups were created within ServiceNow to mirror the enterprise factions established in the AD lab environment: **TeamAqua**, **TeamGalactic**, **TeamMagma**, **TeamPlasma**, and **TeamRocket**.

![Created Groups](Created_Groups_in_ServiceNow.jpg)

![Assigning Groups](Assigning_Groups.jpg)

---

## Step 4 — Assigning Roles
Role-Based Access Control (RBAC) principles were applied at the group level. Group administrative accounts were granted full platform access, while standard user accounts were restricted to read/write-only permissions.

![Assigning Roles](Assigning_Roles.jpg)

---

## Step 5 — Incident Triage & Simulation
An end-user, **Mars** (*TeamGalactic* group), submitted incident ticket `INC0010001` stating: *"I forgot my password and request a reset."* The ticket was successfully triaged and the state updated to **In Progress**.

![Mars Incident](Mars_Incident.jpg)

---

## Step 6 — Account Remediation (Active Directory)
To address the credential issue, the administrator performed a secure password reset within **Active Directory Users and Computers** under the designated `TeamGalactic` Organizational Unit (OU). The security control **"User must change password at next logon"** was enforced to ensure identity integrity.

![AD Password Reset](Mars_Password_Reset.jpg)

![AD Password Changed](Mars_Password_Change.jpg)

---

## Step 7 — Incident Resolution in ServiceNow
Once account remediation was verified, a customer-visible communication note was posted to the ticket, and the ServiceNow incident state was officially closed out as **Resolved**.

![Mars Incident Resolved](Mars_Incident_Resolved.jpg)
