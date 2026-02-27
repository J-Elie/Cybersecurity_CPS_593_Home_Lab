# Linux Security Basics Lab
**Student:** Jennifer Elie  
**Course:** CPS 593 Cybersecurity  
**Due:** March 2<sup>nd</sup> 2026  
---
**School:** SUNY New Paltz  
**Professor:** Kaitlin Hoffmann  
**Semester:** Spring 2026  
---
  

## General System Tasks: 
### 1. Open the terminal in your Virtual Machine (VM). Enter the command to retrieve available updates.
**Command:** `sudo apt update`  
**Command explanation:**  
- **`Sudo:`** Is short for superuser do. It is required for users who are not logged in as root to execute commands that require administrative privileges. It is best practice to use sudo instead of logging in as the root user for several reasons, including maintaining logs of users executing privileged commands, discouraging unauthorized access, and improving system security. It is also recommended to disable root login because root has full control over the system and is a prime target for attackers.  
- **`Apt:`** Stands for Advanced Package Tool. It is a package manager used in some Linux distributions. It allows you to update (check for available updates), install (add new packages), upgrade (update already installed packages when used alongside the update command), and remove (uninstall specified packages).  
- **`Update:`** As part of the apt command, instructs the system to check the repositories for any changes or updates to packages already installed on the system.  

**Command line output:**  
As shown in the image below, 84 packages can be upgraded to newer versions on my system. 
<p align="center">
  <img 
    src="Screenshots/q1-1.png" 
    alt="sudo apt update command line output" 
    width="75%"
  />
</p>
  
---

### 2. Upgrade your system.
**Command:** `sudo apt upgrade`  
**Command explanation:**  
- **`Sudo:`** Same as before. It temporarily grants administrator level permissions in order to execute a command.  
- **`Apt:`** The Advanced Packaging Tool is used again because it is needed to upgrade the system packages.  
- **`Upgrade:`** This keyword after the apt command checks for any packages that were logged as having changed repositories by the previously run apt update command and installs those logged upgrades.  

**Command line output:**  
A prompt will appear asking whether to proceed with the upgrade. Enter “y” to continue or “n” to stop the upgrade.
<p align="center">
  <img 
    src="Screenshots/q2-1.png" 
    alt="sudo apt upgrade command line output:" 
    width="75%"
  />
</p>
