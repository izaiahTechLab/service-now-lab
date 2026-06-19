# Project Walkthrough 🎫

## Step 1 — Creating Users in ServiceNow
Users were created using the naming convention `firstname.faction` to mirror the Active Directory structure (e.g. `brodie.magma`).

![Creating Users](Creating_Users_Service_Now.jpg)

---

## Step 2 — Setting User Passwords
After saving the user record, passwords were configured using the Set Password option. Lab accounts were set with Password never expires for testing purposes.

![Creating Password](Creating_Password.jpg)

---

## Step 3 — Creating Assignment Groups
Five groups were created to mirror the Pokémon factions from the AD lab: TeamAqua, TeamGalactic, TeamMagma, TeamPlasma, and TeamRocket.

![Created Groups](Created_Groups_in_ServiceNow.jpg)

![Assigning Groups](Assigning_Groups.jpg)

---

## Step 4 — Assigning Roles
Role-based permissions were applied per group. Admin accounts received full access, standard users received read/write only.

![Assigning Roles](Assigning_Roles.jpg)

---

## Step 5 — Incident Submitted
User Mars (TeamGalactic) submitted incident INC0010001: "I forgot my password and request a reset." State set to In Progress.

![Mars Incident](Mars_Incident.jpg)

---

## Step 6 — Password Reset in Active Directory
The password for Mars was reset in Active Directory Users and Computers under the TeamGalactic OU with "User must change password at next logon" checked.

![AD Password Reset](Mars_Password_Reset.jpg)

![AD Password Changed](Mars_Password_Change.jpg)

---

## Step 7 — Incident Resolved in ServiceNow
A customer-visible comment was added and the ticket state was changed to "Resolved".

![Mars Incident Resolved](Mars_Incident_Resolved.jpg)
