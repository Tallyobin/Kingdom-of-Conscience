### **Feeling at home. Ease of work. Resources? - Resources!**

2. Use the `pwd` command to display the current directory.

3. Explore directory structure using `cd` and `ls`.

4. Command to return to the home directory: `cd`

5. Change to the /etc directory using the `cd /etc` command.

6. List files in /etc using `ls -l`.

7. View the contents of the 'timezone' file using `cat timezone`.

8. Use the `history` command to display the command history and navigate through it using `history | less`.

9. Monitor system resources using commands like `top`, `last`, and `dmesg`.

10. Check disk space using `df` and `df -h`.

<br>

### **User and File Management**

1. Create a user for a friend using `sudo useradd -m dc999999` and set a password using `sudo passwd dc999999`.

2. Explore multi-user functionality by logging in from another console (Alt+F2) and checking who is logged in using `who`.

3. Return to your terminal (Alt+F1) and create a new directory named 'myfolder' using `mkdir myfolder`.

4. Change to 'myfolder' using `cd myfolder` and create files 'file1' and 'file2.txt' using `touch file1 file2.txt`.

5. Redirect the output of the `date` command to 'file1' using `date > file1`, and check the contents using `cat file1`.

6. Copy 'file1' to a new directory 'mybackup' using `cp file1 mybackup`.

7. Explore permissions and ownership using commands like `ls -l`, `chmod`, `chown`, and `chgrp`.

8. Delete the 'mybackup' directory and its contents using `rm -Rf mybackup`.

<br>

### **Package Installation & Archive**

1. Update the system using `sudo apt-get update` and upgrade installed packages using `sudo apt-get upgrade`.

2. Search for console games using `apt-cache search game | grep console` and install 'pacman4console' using `sudo apt-get install pacman4console`.

3. Install and play 'nethack-console' using `sudo apt-get install nethack-console` and `nethack-console`.

4. Use `dpkg` to gather information about 'nethack-console' and list installed files using `dpkg -L nethack-console`.

5. Archive files using `tar -cvf myarchive.tar quiz.txt marks.xls presentation.pptx` and copy the archive to 'myfolder'.

6. Extract files from the archive using `tar -xvf myarchive.tar`.

<br>

### **Package Installation & Archive**

1. **Install Network Tools:**
   ```
   sudo apt-get install net-tools
   ```
   - Command installs tools to control the network subsystem of the Linux kernel.

2. **Find IP Address:**
   ```
   ifconfig enp0s3
   ```
   - Identifies the IP address of the server from the network configuration.

4. **Install Apache (Web Services):**
   ```
   sudo apt-get install apache2
   ```
   - Installs the Apache web server.

5. **Check Apache Status:**
   ```
   service --status-all
   ```
   - Checks the status of installed services, including Apache.

6. **Modify Default Web Content:**
   - Navigate to the web server directory:
     ```
     cd /var/www/html
     ```
   - Create a backup of the default page:
     ```
     sudo cp index.html index.html.ori
     ```
   - Edit the default welcome file:
     ```
     sudo nano index.html
     ```

<br>

### **MySQL Server (Database Services)**

1. **Search for MySQL Database Services:**
   ```
   apt-cache search database | grep mysql
   ```
   - Lists available MySQL-related packages.

2. **Install MySQL Server:**
   ```
   sudo apt-get install mysql-server
   ```
   - Installs MySQL server.

3. **Install phpMyAdmin:**
   ```
   sudo apt-get install phpmyadmin php-mbstring
   ```
   - Installs phpMyAdmin for managing MySQL databases.

<br>

### **vsftpd (FTP Services)**

1. **Install vsftpd:**
   ```
   sudo apt-get install vsftpd
   ```
   - Installs vsftpd for FTP services.

<br>

### **OpenSSH (Remote Server)**

1. **Install OpenSSH Server:**
   ```
   sudo apt-get install openssh-server
   ```
   - Installs OpenSSH server for secure remote logins.

2. **Log on to SSH Server:**
   ```
   ssh -l {username} {IP-address}
   ```
   - Logs in securely to another machine over the network using SSH.

<br>

### **Email Services**

1. **Install Postfix and Mailx:**
   ```
   sudo apt-get install postfix
   sudo apt-get install mailutils
   ```
   - Installs Postfix as MTA and mailx for communication with the mail server.

2. **Send Test Email:**
   ```
   echo 'Hi student number 2. How are you today? ' | mailx -s "Mail from your sysadmin" student1
   ```
   - Sends a test email to another user.

<br>

### **Shell Scripts and Programming**

1. **Create and Execute Shell Script:**
   - Create a file `my_first` with the content and execute:
     ```
     sudo vi my_first
     ./my_first
     ```
   - Demonstrates a simple shell script with the shebang, comments, and an echo statement.

2. **Shell Script with Positional Parameters:**
   - Create a file `my_prog` with the content and execute:
     ```
     sudo vi my_prog
     ./my_prog Mr Ikhsan
     ```
   - Illustrates the use of positional parameters in a shell script.

3. **Shell Script with Variable:**
   - Create a file `my_variable` with the content and execute:
     ```
     sudo vi my_variable
     ./my_variable
     ```
   - Demonstrates the use of a shell variable in a script.

<br>

### **Windows Virtualization using Hyper-V**

1. **Enable Hyper-V:**
   - Open PowerShell
   - Run commands:
     ```powershell
     Enable-WindowsOptionalFeature –Online -FeatureName Microsoft-Hyper-V –All -NoRestart
     Install-WindowsFeature RSAT-Hyper-V-Tools -IncludeAllSubFeature
     Restart-Computer -Force -Wait
     ```
