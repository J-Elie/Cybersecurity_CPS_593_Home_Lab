<style>
:root {
  --accent-color: #18b5a8;
}
.accent { color: var(--accent-color); font-weight: bold; }
</style>

# Linux Security Basics Lab
$\color{#18b5a8}{\textsf{lorem ipsum}}$
<span class="accent">Student:</span> Jennifer Elie  
<span class="accent">Course:</span> CPS 593 Cybersecurity  
<span class="accent">Due:</span> March 2<sup>nd</sup> 2026  
---
<span class="accent">School:</span> SUNY New Paltz  
<span class="accent">Professor:</span> Kaitlin Hoffmann  
<span class="accent">Semester:</span> Spring 2026  
---
  

## General System Tasks: 
### 1. Open the terminal in your Virtual Machine (VM). Enter the command to retrieve available updates.
<span class="accent">Command:</span> `sudo apt update`  
<span class="accent">Command explanation:</span>  
- **`Sudo:`** Is short for superuser do. It is required for users who are not logged in as root to execute commands that require administrative privileges. It is best practice to use sudo instead of logging in as the root user for several reasons, including maintaining logs of users executing privileged commands, discouraging unauthorized access, and improving system security. It is also recommended to disable root login because root has full control over the system and is a prime target for attackers.  
- **`Apt:`** Stands for Advanced Package Tool. It is a package manager used in some Linux distributions. It allows you to update (check for available updates), install (add new packages), upgrade (update already installed packages when used alongside the update command), and remove (uninstall specified packages).  
- **`Update:`** As part of the apt command, instructs the system to check the repositories for any changes or updates to packages already installed on the system.  

<span class="accent">Command line output:</span>  
As shown in the image below, 84 packages can be upgraded to newer versions on my system. 
<p align="center">
  <img src="screenshots/q1-1.png" alt="sudo apt update command line output:" style="width: 75vw; border: 2px solid var(--accent-color);">
</p>
  
---

### 2. Upgrade your system.
<span class="accent">Command:</span> `sudo apt upgrade`  
<span class="accent">Command explanation:</span>  
- **`Sudo:`** Same as before. It temporarily grants administrator level permissions in order to execute a command.  
- **`Apt:`** The Advanced Packaging Tool is used again because it is needed to upgrade the system packages.  
- **`Upgrade:`** This keyword after the apt command checks for any packages that were logged as having changed repositories by the previously run apt update command and installs those logged upgrades.  

<span class="accent">Command line output:</span>  
A prompt will appear asking whether to proceed with the upgrade. Enter “y” to continue or “n” to stop the upgrade.
<p align="center">
  <img src="screenshots/q2-1.png" alt="sudo apt upgrade command line output:" style="width: 75vw; border: 2px solid var(--accent-color);">
</p>
