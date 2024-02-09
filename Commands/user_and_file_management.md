# User and File Management Commands

**System-level commands:**

1. **uname**: Displays system information such as the kernel name, node name, kernel release, and kernel version.
   Example: 
   ```
   uname -a
   ```

2. **uptime**: Shows how long the system has been running, the number of users currently logged in, and the system load averages.
   Example:
   ```
   uptime
   ```

3. **date**: Displays or sets the system date and time.
   Example:
   ```
   date
   ```

4. **who, whoami**: `who` displays information about users currently logged in, while `whoami` prints the username of the current user.
   Example:
   ```
   who
   whoami
   ```

5. **which**: Locates the executable file associated with the given command.
   Example:
   ```
   which ls
   ```

6. **id**: Displays user identity information, including user ID (uid) and group ID (gid).
   Example:
   ```
   id
   ```

7. **sudo**: Allows users to execute commands with the security privileges of another user, typically the superuser (root).
   Example:
   ```
   sudo apt update
   ```

8. **shutdown**: Shuts down or reboots the system after a specified time.
   Example:
   ```
   shutdown -h now
   ```

9. **reboot**: Restarts the system.
   Example:
   ```
   reboot
   ```

10. **apt, yum, dnf, pacman, portage**: Package management commands for different Linux distributions (Debian-based, Red Hat-based, Arch Linux, Gentoo).
    Example (apt):
    ```
    sudo apt update
    ```

**User & Group management commands:**

1. **sudo**: Allows users to execute commands with superuser privileges.
   Example:
   ```
   sudo apt update
   ```

2. **useradd**: Creates a new user account.
   Example:
   ```
   sudo useradd newuser
   ```

3. **whoami**: Displays the username of the current user.
   Example:
   ```
   whoami
   ```

4. **su**: Allows switching to another user account.
   Example:
   ```
   su username
   ```

5. **passwd**: Changes the password of a user account.
   Example:
   ```
   passwd
   ```

6. **userdel**: Deletes a user account.
   Example:
   ```
   sudo userdel username
   ```

7. **groupadd**: Creates a new group.
   Example:
   ```
   sudo groupadd newgroup
   ```

8. **gpasswd -a, -m**: Adds a user to a group (-a) or sets a group as the primary group for a user (-m).
   Example:
   ```
   sudo gpasswd -a username groupname
   sudo gpasswd -m username groupname
   ```

9. **groupdel**: Deletes a group.
   Example:
   ```
   sudo groupdel groupname
   ```

**File permission commands:**

1. **umask**: Sets the default permissions for newly created files and directories.
   Example:
   ```
   umask 022
   ```

2. **ls -l**: Lists files and directories with detailed information, including permissions.
   Example:
   ```
   ls -l
   ```

3. **chmod**: Changes the permissions of files and directories.
   Example:
   ```
   chmod u+x filename
   ```

4. **chown**: Changes the owner and group of files and directories.
   Example:
   ```
   sudo chown username:groupname filename
   ```

5. **chgrp**: Changes the group ownership of files and directories.
   Example:
   ```
   sudo chgrp groupname filename
   ```

**Compression commands:**

1. **zip, gunzip, gzip**: Commands for compressing and decompressing files using the zip and gzip formats.
   Example (zip):
   ```
   zip compressed.zip file1.txt file2.txt
   ```

2. **tar, untar**: Commands for creating and extracting tar archives.
   Example (create tar archive):
   ```
   tar -cvf archive.tar directory/
   ```

**File transfer commands:**

1. **SCP**: Securely copies files between hosts using the SSH protocol.
   Example:
   ```
   scp file.txt username@remote_host:/path/to/destination
   ```

2. **rsync**: Synchronizes files and directories between hosts or directories on the same host.
   Example:
   ```
   rsync -avz source/ destination/
   ```

These examples demonstrate how each command is used and provide a practical understanding of their functionalities.