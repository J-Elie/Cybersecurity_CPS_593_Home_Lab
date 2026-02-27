<p align="center">
  <img 
    src="Screenshots/Linux-Security-Basics-Lab.png" 
    alt="Linux Security Basics Lab" 
    width="100%"
  />
</p>

**Student:** Jennifer Elie  
**Course:** CPS 593 Cybersecurity  
**Due:** March 2<sup>nd</sup> 2026  
---
**School:** SUNY New Paltz  
**Professor:** Kaitlin Hoffmann  
**Semester:** Spring 2026  
---
  

<p>
  <img
    src="Screenshots/General-System-Tasks.png"
    alt="General System Tasks"
    width="50%"
  />
</p>
<!-- ## General System Tasks:  -->

## 1. Open the terminal in your Virtual Machine (VM). Enter the command to retrieve available updates.
**Command:** `sudo apt update`  
**Command explanation:**  
- **`sudo:`** Is short for superuser do. It is required for users who are not logged in as root to execute commands that require administrative privileges. It is best practice to use sudo instead of logging in as the root user for several reasons, including maintaining logs of users executing privileged commands, discouraging unauthorized access, and improving system security. It is also recommended to disable root login because root has full control over the system and is a prime target for attackers.  
- **`apt:`** Stands for Advanced Package Tool. It is a package manager used in some Linux distributions. It allows you to update (check for available updates), install (add new packages), upgrade (update already installed packages when used alongside the update command), and remove (uninstall specified packages).  
- **`update:`** As part of the apt command, instructs the system to check the repositories for any changes or updates to packages already installed on the system.  

**Command line output:**  
As shown in the image below, 84 packages can be upgraded to newer versions on my system. 
<p align="center">
  <img 
    src="Screenshots/q1-1.png" 
    alt="sudo apt update command line output" 
    width="75%"
  />
</p>

## 2. Upgrade your system.
**Command:** `sudo apt upgrade`  
**Command explanation:**  
- **`sudo:`** Same as before. It temporarily grants administrator level permissions in order to execute a command.  
- **`apt:`** The Advanced Packaging Tool is used again because it is needed to upgrade the system packages.  
- **`upgrade:`** This keyword after the apt command checks for any packages that were logged as having changed repositories by the previously run apt update command and installs those logged upgrades.  

**Command line output:**  
A prompt will appear asking whether to proceed with the upgrade. Enter “y” to continue or “n” to stop the upgrade.
<p align="center">
  <img 
    src="Screenshots/q2-1.png" 
    alt="sudo apt upgrade command line output" 
    width="75%"
  />
</p>

## 3. Reboot your system.
**Command:** `sudo reboot`  
**Command explanation:**  
- **`sudo:`** Temporarily allows administrator-level permissions for command execution. It is required for rebooting the system because not every user should have the ability to restart or temporarily take down the system.    
- **`reboot:`** This is the command used to restart the system.  

**Command line output:**  
<p align="center">
  <img 
    src="Screenshots/q3-1.png" 
    alt="sudo reboot command line output" 
    width="75%"
  />
</p>
<p align="center">
  <img 
    src="Screenshots/q3-2.png" 
    alt="reboot screen" 
    width="75%"
  />
</p>

---  

<p>
  <img 
    src="Screenshots/User-Tasks.png" 
    alt="User Tasks" 
    width="50%"
  />
</p>

## 4. Change the current user to root using the command sudo su root. What does the prompt look like?  
**Command:** `sudo su root`  
**Command explanation:**  
- **`sudo:`** Temporarily allows administrator level permission for command execution.  
- **`su:`** Stands for substitute user. This command allows switching to and running commands as another user. If no user is specified, the default user is root.  
- **`root:`** The user to switch to after executing the substitute user command. Root is the default user for this command, but explicitly specifying it is not an issue.

**Command line output:**  
As can be seen in the image, the username changes from jelie to root, and the shell changes from bash to shell. This indicates that the system is now signed in as the root user.  
<p align="center">
  <img 
    src="Screenshots/q4-1.png" 
    alt="sudo su root command line output" 
    width="75%"
  />
</p>












<p>
  <img 
    src="Screenshots/Group-Tasks.png" 
    alt="" 
    width="50%"
  />
</p>

<p>
  <img 
    src="Screenshots/Permission-and-ACL-Tasks.png" 
    alt="" 
    width="50%"
  />
</p>