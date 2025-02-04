🚀 A comprehensive collection of essential Linux commands and best practices for system administrators, DevOps engineers, and power users. This repository provides useful commands for process management, log analysis, network troubleshooting, system monitoring, and more.

💡 Whether you're a beginner or an advanced user, this guide will help you optimize your workflow and efficiently manage Linux systems.

🔹 Topics Covered:
✔️ Process Management
✔️ Log Management (journalctl, syslog, messages, etc.)
✔️ Networking & Firewall Commands
✔️ System Monitoring (htop, vmstat, iostat, etc.)
✔️ File & Disk Management
✔️ Automation & Scripting

📖 Contributions are welcome! Feel free to fork, improve, and share. 🚀


# Welcome to Linux-xox-tools by othmane tahir 

# Table of content:
1. [Linux Architecture](#linux-architecture)
1. [Linux Distributions](#linux-distributions)
1. [Using The Shell](#using-the-shell)
1. [Navigating The Shell](#navigating-the-shell)
1. [Usefull Commands](#usefull-commands)

#### Hy i'm Linux  and this... 🐧 is my penguin. He's my PR guy.  He handles all the "cute" and "cuddly" aspects of my image. I handle the "power," "flexibility," and "not crashing every five minutes" parts.  We're a team. A brilliant team.

## Linux Architecture 
Linux: Not Just a Penguin, It's a Whole Ecosystem!

Hi, I'm Linux, and this... is my penguin, Tux. He's my public face.  He's adorable, right?  Distracts everyone from how ridiculously powerful I am under the hood.  Because beneath the fluff, I'm a finely-tuned machine, a masterpiece of open-source engineering.

Let's talk architecture, baby!  Think of me as a layered cake, but instead of frosting and sponge, it's code and… well, more code.

![alt text](https://linuxsimply.com/wp-content/uploads/2023/11/architecture.png "linux-architecture")
*   **The Kernel (The Heart❤️):** This is my core, the brains of the operation.  It's responsible for talking to the hardware, managing memory, and scheduling processes.  Think of it as the conductor of an orchestra, making sure everything plays nicely together.  Linus Torvalds built this, and it's the foundation of everything Linux.

*   **The Shell (The Translator):** This is how you, the user, communicate with the Kernel.  It's a command-line interpreter.  You type in commands, and the Shell translates them into instructions the Kernel understands.  It's like having a conversation with your computer, but instead of emojis, you use cryptic commands.  (Don't worry, there are graphical interfaces too!)

*   **Applications (The Fun Stuff):** These are the programs you actually use, like web browsers, text editors, and games.  They sit on top of the Shell and Kernel and provide the functionality you need.  Think of them as the instruments in the orchestra, playing the music the Kernel conducts.

![alt text](https://preview.redd.it/linux-distro-family-chart-with-distros-based-derivatives-i-v0-0h0jbzn8ca2d1.png?width=640&crop=smart&auto=webp&s=585946b5ab371aa61ef6b4b5ad84cca58e92a835 "linux-architecture")

Now, the beauty of Linux is that it's open-source.  This means anyone can take my Kernel and build a *distribution* around it.  Think of distributions like different remixes of the same song.  They all use the same Kernel, but they have different sets of applications, desktop environments, and configurations.  It's like choosing your favorite flavor of ice cream – they're all ice cream, but they have different tastes.

![alt](https://media.geeksforgeeks.org/wp-content/uploads/20240501185858/KDE-vs-Genome.webp "linux-architecture")

And speaking of desktop environments, that's the graphical interface you actually interact with.  It's what makes Linux look and feel like… well, an operating system.  You can choose from a variety of desktop environments, each with its own look and feel.  It's like choosing the furniture for your operating system house.

![alt text](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2021/05/run-linux-commands-in-the-background.jpg "linux-architecture")

So, why choose Linux?  Because it's powerful, flexible, and free!  It's like having a superpower for your computer.  And if you're ever stuck, the Linux community is incredibly helpful.  It's like having a global network of experts ready to assist you.

## Linux Distributions

Linux comes in various distributions (distros), each tailored for specific use cases, from personal computing to enterprise servers and cybersecurity. Below is a **categorized breakdown** of the most commonly used Linux distributions, along with their **strengths, similarities, and differences**.

---

### 🔹 1️⃣ General-Purpose Linux Distributions
These are designed for **everyday users, developers, and system administrators**.

| Distribution | Based On | Best For | Package Manager | Default Desktop |
|-------------|---------|----------|----------------|----------------|
| 🐧 **Ubuntu** | Debian | Beginners, Workstations, Servers | APT (`.deb`) | GNOME |
| 🏗️ **Debian** | Independent | Stability, Servers, DevOps | APT (`.deb`) | GNOME |
| 🔵 **Fedora** | Red Hat | Developers, Cutting-edge Tech | DNF (`.rpm`) | GNOME |
| 💻 **Arch Linux** | Independent | Advanced Users, Customization | Pacman (`.pkg.tar.xz`) | No Default |
| 🎯 **Linux Mint** | Ubuntu/Debian | Windows-like Experience | APT (`.deb`) | Cinnamon |

🔹 **🟢 Similarities:**  
- Ubuntu, Debian, and Mint use `.deb` (Debian-based) packages.  
- Fedora and Debian focus on **stability**, while Arch offers **customization**.  
- Ubuntu and Mint are **user-friendly** with a graphical installer.

---

### 🖥️ 2️⃣ Enterprise & Server Linux Distributions
These are built for **business environments, cloud computing, and large-scale infrastructures**.

| Distribution | Based On | Best For | Package Manager | Key Feature |
|-------------|---------|----------|----------------|-------------|
| 🔴 **Red Hat Enterprise Linux (RHEL)** | Fedora | Corporate Servers | DNF (`.rpm`) | Enterprise Support |
| 🟣 **CentOS Stream** | RHEL | Cloud & Hosting | DNF (`.rpm`) | RHEL-Compatible |
| 📦 **SUSE Linux Enterprise (SLES)** | Independent | Enterprise IT | Zypper (`.rpm`) | YaST Management |
| ☁️ **Ubuntu Server** | Debian | Cloud & DevOps | APT (`.deb`) | OpenStack Support |

🔹 **🟢 Similarities:**  
- RHEL, CentOS, and SUSE use `.rpm` packages.  
- Ubuntu Server and Debian are **lightweight** and **Debian-based**.  
- All offer **long-term support (LTS)** for critical workloads.

---

### 🛡️ 3️⃣ Security & Pentesting Linux Distributions
These are designed for **cybersecurity professionals, ethical hackers, and forensics**.

| Distribution | Based On | Best For | Pre-installed Tools |
|-------------|---------|----------|---------------------|
| 🐉 **Kali Linux** | Debian | Penetration Testing | Metasploit, Wireshark, Nmap |
| 🦉 **Parrot OS** | Debian | Security, Privacy | Anonsurf, Forensics Tools |
| 🏴‍☠️ **BlackArch** | Arch Linux | Advanced Pentesting | 2,500+ Hacking Tools |

🔹 **🟢 Similarities:**  
- All include **penetration testing frameworks** and security tools.  
- Kali and Parrot are **Debian-based**, while BlackArch extends **Arch Linux**.  
- Parrot OS focuses more on **privacy & anonymity**.

---

### 📦 4️⃣ Lightweight Linux Distributions
Perfect for **old computers, embedded systems, or minimal installations**.

| Distribution | Based On | Best For | RAM Requirement |
|-------------|---------|----------|----------------|
| 🟢 **Alpine Linux** | Independent | Containers, Security | 64MB |
| 🏎️ **Puppy Linux** | Various | Old Hardware | 128MB |
| 🏠 **Lubuntu** | Ubuntu | Lightweight Desktop | 512MB |

🔹 **🟢 Similarities:**  
- All are **resource-efficient** and run on **low-end systems**.  
- Alpine is commonly used in **Docker containers** due to its small size.  
- Lubuntu and Puppy provide **graphical desktops** for older machines.

---

### 🛠️ Choosing the Right Linux Distribution
🔹 **For Beginners** → 🐧 Ubuntu, 🟢 Linux Mint  
🔹 **For Developers** → 🏗️ Fedora, 🔵 Arch Linux  
🔹 **For Enterprise** → 🔴 RHEL, 🟣 CentOS Stream  
🔹 **For Hacking** → 🐉 Kali Linux, 🦉 Parrot OS  
🔹 **For Old PCs** → 🏎️ Puppy Linux, 🏠 Lubuntu  

---

### 📖 Additional Learning Resources
Here are some helpful references to dive deeper into Linux distributions and system administration:  
📚 [DistroWatch](https://distrowatch.com/) – Compare Linux distros  
📖 [The Linux Command Line](https://linuxcommand.org/) – Beginner to Advanced Guide  
📙 [Arch Wiki](https://wiki.archlinux.org/) – The best technical documentation  

---
## Using the shell

- Home directory and `~`

In most cases, your home directory will look something like this:

```bash
[xox@pc-name ~]$
```
The `~` character indicates that you are in the home directory, whilst `&` tells that you are not the root user. At the prompt, you can type a command, i.e `date`, which will be interpreted by the shell:

```bash
[xox@pc-name ~]$ date
Tue May 11 17:15:18 EDT 2021
[xox@pc-name ~]$
```

You can pass certain arguments to a shell command, such as `echo`, which prints outs a passed argument:

```bash
[xox@pc-name ~]$ echo Hello Linux!
Hello Linux!
[xox@pc-name ~]$
```

- `echo $PATH`, `which`

But how does the shell know how to find the `date` or `echo` programs? When you run commands in your shell, you are really writing a small bit of code that your shell interprets. If the shell is asked to execute a command that doesn’t match one of its programming keywords, it consults an environment variable called `$PATH` that lists which directories the shell should search for programs when it is given a command:

```bash
[xox@pc-name ~]$ echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
[xox@pc-name ~]$ which echo
/bin/echo
[xox@pc-name ~]$ /bin/echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

When we run the `echo` command, the shell sees that it should execute the program `echo`, and then searches through the :-separated list of directories in `$PATH` for a file by that name. When it finds it, it runs it (assuming the file is executable). We can find out which file is executed for a given program name using the `which` program. We can also bypass `$PATH` entirely by giving the path to the file we want to execute.

- contents of the shell

For the next command, let's type `ls -lh` to list the contents of a folder. For instance, you can observe here the contents of my home directory:

```
-rw-r--r-- 1 xox usrgrp 3.5K May 11 10:34 environment.yml
drwxr-xr-x 3 xox usrgrp    3 Apr 24 16:46 github/
lrwxrwxrwx 1 xox usrgrp   24 Jan 26 09:03 mydata -> /apps/data/
drwxr-xr-x 3 xox usrgrp    3 Jan 28 10:06 scikit_learn_data/
drwxr-xr-x 2 xox usrgrp    4 Nov 30 09:21 scripts/
drwxr-xr-x 3 xox usrgrp    3 Nov  6  2020 workshops/
```

To understand what does it mean, check the following example:

```
-rwxrw-r--    10    root   root 2048    Jan 13 07:11 afile.exe
?UUUGGGOOOS   00  UUUUUU GGGGGG ####    ^-- date stamp and file name are obvious ;-)
^ ^  ^  ^ ^    ^      ^      ^    ^
| |  |  | |    |      |      |    \--- File Size
| |  |  | |    |      |      \-------- Group Name (for example, Users, Administrators, etc)
| |  |  | |    |      \--------------- Owner Account
| |  |  | |    \---------------------- Link count (what constitutes a "link" here varies)
| |  |  | \--------------------------- Alternative Access (blank means none defined, anything else varies)
| \--\--\----------------------------- Read, Write and Special access modes for [U]ser, [G]roup, and [O]thers (everyone else)
\------------------------------------- File type flag
```

In the order of ouput:

- File permissions (`-rwxrw-r--`),
- Number of (hard) links (`1`),
- Owner name (`root`),
- Owner group (`root`),
- File size in bytes (`2048`),
- Time of last modification (`Jan 13 07:11`)
- File/directory name (`afile.exe`)

File permissions is displayed as following;

- First character is most often `-`, `l` or `d`. A `d` indicates a directory, a `-` represents a regular file, `l` is a symlink (or soft link) and other letters are used for other types of special files.
- Three sets of characters, three times, indicating permissions for owner, group and other:
        `r` = readable
        `w` = writable
        `x` = executable (for files) or accessible (for directories)
- This may be followed by some other character of there are extended permissions, like e.g. Linux ACL that are marked with a `+`.

In our example `-rwxrw-r--`, this means the line displayed is:

- A regular file (displayed as `-`)
- Readable, writable and executable by owner (`rwx`)
- Readable, writable, but not executable by group (`rw-`)
- Readable but not writable or executable by other (`r--`)

The number of hard links means the number of names the inode has, i.e. links created with `ln` without the `-s` option.

For more information, check this [link](https://unix.stackexchange.com/questions/103114/what-do-the-fields-in-ls-al-output-mean).

### Navigating the shell

- `pwd`

Print name of current/working directory.

```bash
[username@pc-name ~]$ pwd
/home/username
```
- `cd`

Change a directory.

```bash
[username@pc-name ~]$ cd /home
[username@pc-name ~]$ pwd
/home
[username@pc-name ~]$ cd ..
[username@pc-name ~]$ pwd
/
[username@pc-name ~]$ cd ./home
[username@pc-name ~]$ pwd
/home
[username@pc-name ~]$ cd
[username@pc-name ~]$ pwd
/home/username
[username@pc-name ~]$ cd ../../
[username@pc-name ~]$ pwd
/
[username@pc-name ~]$ cd ~/
[username@pc-name ~]$ pwd
/home/username
```

A path on the shell is a delimited list of directories; separated by `/` on Linux and macOS and `\` on Windows. On Linux and macOS, the path `/` is the “root” of the file system, under which all directories and files lie, whereas on Windows there is one root for each disk partition (e.g., `C:\`). We will generally assume that you are using a Linux filesystem in this class. A path that starts with `/` is called an absolute path. Any other path is a relative path. Relative paths are relative to the current working directory, which we can see with the pwd command and change with the `cd` command. In a path, `.` refers to the current directory, and `..` to its parent directory

For more information on what can you find the root `/` directory, check this [YouTube video](https://www.youtube.com/watch?v=42iQKuQodW4).

- `ls`

List the contents of the folder. Some useful flags:

```
  -a, --all                  do not ignore entries starting with .
  -d, --directory            list directories themselves, not their contents
  -h, --human-readable       with -l, print sizes in human readable format
                               (e.g., 1K 234M 2G)
```

For more options, type `ls --help`.

- `chmod`

You can change permissions, by typing the following commands:

```
chmod +rwx filename                     to add permissions.
chmod -rwx directoryname                to remove permissions.
chmod +x filename                       to allow executable permissions.
chmod -wx filename                      to take out write and executable permissions
```

To be more specific, use `u` for users, `u` for group, `o` for others, and `ugo` or `a` (for all):

```
chmod ugo+rwx foldername                to give read, write, and execute to everyone.
chmod a=r foldername                    to give only read permission for everyone.
```

To change permissions in numeric code in Linux, you use numbers instead of `r`, `w`, or `x`.

```
0 = No Permission
1 = Execute
2 = Write
4 = Read
```

Basically, you add up the numbers depending on the level of permission you want to give. Permission numbers are:

```
0 = ---
1 = --x
2 = -w-
3 = -wx
4 = r-
5 = r-x
6 = rw-
7 = rwx
```

For example:

```
chmod 777 foldername                    will give read, write, and execute permissions for everyone.
chmod 700 foldername                    will give read, write, and execute permissions for the user only.
chmod 327 foldername                    will give write and execute (3) permission for the user, w (2) for the group, and read, write, and execute for the users.
```

Other tools, such as `chgrps` and `chown` allow to change groups of files and ownership, respectively.

For more about permissions, follow the [link](https://en.wikipedia.org/wiki/File-system_permissions).

- `whoami`

Print a current effective userid:

```bash
[username@pc-name ~]$ whoami
your-username
```

- `touch`

Create a single empty file.

- `cp`

Copy a file from one location to another. To copy folders, you need to add `-r` flag to perform a recursive copy.

- `mv`

Move a folder to a different location or rename a file in place.

- `mkdir`

Create a folder.

- `rm`

Remove a file. To remove a folder, you need to add a recursive `-r` flag. Sometimes, you might need to force the removal, so add `-f` flag. But be careful, every operation with `rm` is irreversable!

- Tab autocompletion and right/middle mouse button copy.

Use `tab` button to autocomplete paths, command names and search for file names. In addition, use right/middle mouse (depending on the system) button for quick copy paste actions.

- See the command history.

Press `up` and `down` buttons to cycle through your command history. If you have trully spammed a lot of commands, perhaps an easier way would be to read `~/.bash_history` file. Or press `ctrl + r` for recursive command history search.

- Display the contents of a file.

## Usefull Commands

### 1- Process Management

| Command | Description | Options/Examples |
|---|---|---|
| `ps` (Process Status) | Displays running processes. | `ps aux` (details), `ps -ef` (UID/PPID), `ps -u <user>` (user), `ps -p <PID>` (PID), `ps --forest` (hierarchical tree) |
| `top` (Table Of Processes) | Displays real-time process monitoring. | `top` (real-time), `top -u <user>` (user), `top -p <PID>` (PID), `Shift + M` (sort by memory), `Shift + P` (sort by CPU), `k` (kill), `1` (CPU per core) |
| `htop` | Interactive alternative to `top`. | `htop` (graphical interface), `htop -u <user>` (user), navigation with arrows, color coding |
| `pgrep` (Process Grep) | Searches for a process by name. | `pgrep nginx` (PID of "nginx"), `pgrep -u root` (root processes), `pgrep -l ssh` (PID and name) |
| `kill` | Terminates a process by PID. | `kill <PID>` (SIGTERM), `kill -9 <PID>` (SIGKILL), `kill -HUP <PID>` (reload) |
| `pkill` | Kills by process name. | `pkill apache` (process "apache"), `pkill -9 firefox` (force kill), `pkill -u <user>` (user) |
| `killall` | Kills all processes of a name. | `killall nginx` (all "nginx"), `killall -9 firefox` (force kill) |
| `xkill` | Kills by clicking on the window (X11). | `xkill` (graphical environment) |
| `nice` | Starts with a specific priority. | `nice -n 10 ./script.sh` (low priority), `nice -n -5 ./script.sh` (high priority) |
| `renice` | Modifies the priority of a process. | `renice -n 5 -p <PID>` (modify), `renice -n -10 -u root` (modify for root) |
| `&` | Runs a process in the background. | `./long_script.sh &` |
| `jobs` | Lists background processes. | `jobs` |
| `fg` | Brings a process to the foreground. | `fg %1` (job number 1) |
| `bg` | Resumes a process in the background. | `bg %1` (job number 1) |
| `nohup` | Runs in the background (disconnection). | `nohup ./long_script.sh &` (output to nohup.out) |
| `disown` | Detaches a process from the terminal. | `disown -h %1` (job 1) |
| `strace` | Traces system calls. | `strace -p <PID>` (real-time), `strace -c ls` (analysis) |
| `lsof` | Lists open files. | `lsof -p <PID>` (open files), `lsof -i :80` (port 80) |
| `watch` | Executes a command at intervals. | `watch -n 2 ps aux` (every 2 seconds) |
| `timeout` | Limits the execution time. | `timeout 10s ./script.sh` (10 seconds) |
| `ps aux | grep Z` | Identifies zombie processes. |  |
| `kill -HUP <PPID>` | Cleans zombie processes. | (if parent PID = 1) |

### Zombie and Orphan Process Management

* **Zombie:** A process that has finished execution but remains in the process table.
* **Orphan:** A process whose parent has terminated.


### 2- Log Management

<a id="log-management-with-journalctl"></a>
### <span style="color:green;">- Log Management with journalctl</span>

`journalctl` is the primary tool for querying and managing systemd journal logs.

| Command | Function |
|---|---|
| `journalctl` | Displays all system logs. |
| `journalctl -n 50` | Displays the last 50 lines of logs. |
| `journalctl -f` | Displays logs in real time (equivalent to `tail -f`). |
| `journalctl -b` | Displays logs from the last boot. |
| `journalctl -b -1` | Displays logs from the previous boot. |
| `journalctl -u nginx` | Displays logs from the Nginx service. |
| `journalctl -p 3` | Displays only error logs (p 3 = ERR). |
| `journalctl --since "1 hour ago"` | Displays logs from the last 60 minutes. |
| `journalctl --since "2024-02-01 10:00:00" --until "2024-02-01 12:00:00"` | Displays logs for a specific time period. |
| `journalctl --disk-usage` | Displays disk space used by logs. |
| `journalctl --vacuum-size=500M` | Removes logs to keep them under 500 MB. |
| `journalctl --vacuum-time=2d` | Removes logs older than 2 days. |
| `journalctl --flush` | Forces logs in memory to be written to disk. |

<a id="var-log-syslog"></a>
### <span style="color:green;">- /var/log/syslog (General System Logs)</span>

This file contains logs from various services and applications, excluding authentication logs.

| Command | Function |
|---|---|
| `cat /var/log/syslog` | Displays the entire file content. |
| `tail -n 50 /var/log/syslog` | Displays the last 50 lines of logs. |
| `tail -f /var/log/syslog` | Displays logs in real time. |
| `grep "error" /var/log/syslog` | Searches for the word "error" in the logs. |

<a id="var-log-messages"></a>
### <span style="color:green;">- /var/log/messages (General System Logs for Certain Distributions)</span>

Similar to `/var/log/syslog`, this file is primarily used on RHEL/CentOS for storing general system logs.

| Command | Function |
|---|---|
| `cat /var/log/messages` | Displays the entire file content. |
| `tail -f /var/log/messages` | Displays logs in real time. |

<a id="other-log-files"></a>
### <span style="color:green;">- Other Common Log Files</span>

| File | Content |
|---|---|
| `/var/log/auth.log` | Authentication and login logs (SSH, sudo...). |
| `/var/log/dmesg` | Kernel logs (boot, hardware errors, devices). |
| `/var/log/kern.log` | Detailed kernel logs. |
| `/var/log/secure` | Security logs (mainly on CentOS/RHEL). |
| `/var/log/nginx/access.log` | Access logs for the Nginx server. |
| `/var/log/nginx/error.log` | Error logs for Nginx. |
| `/var/log/apache2/access.log` | Access logs for the Apache server. |
| `/var/log/apache2/error.log` | Error logs for Apache. |

<a id="log-rotation-with-logrotate"></a>
### <span style="color:green;">- Log Rotation with logrotate</span>

`logrotate` is used for archiving and cleaning up logs automatically.

| Command | Function |
|---|---|
| `sudo logrotate -f /etc/logrotate.conf` | Forces manual log rotation. |
| `cat /etc/logrotate.conf` | Checks the configuration. |

<a id="tips-for-log-management"></a>
### <span style="color:green;">- Tips for Log Management</span>

*   **Log Centralization:** Use tools like `rsyslog` or `Elasticsearch` to collect and manage logs from multiple servers in one place. This makes it easier to search and analyze logs.

*   **Log Analysis:** Use tools like `grep`, `awk`, `sed`, or dedicated log analysis tools to search for errors, warnings, or unusual behavior in your logs.

*   **Log Monitoring:** Set up alerts to be notified of important events in your logs, such as critical errors or intrusion attempts.

*   **Log Archiving:** Regularly archive your logs to keep a historical record of events and meet compliance requirements.

*   **Log Security:** Protect your log files with appropriate permissions to prevent unauthorized access.

*   **Log Rotation:** Configure `logrotate` for regular log rotation to prevent logs from taking up too much disk space.

*   **Using `journalctl`:** `journalctl` offers many options for filtering and displaying systemd logs. Learn to master this tool to make your work easier.

*   **Log Structure:** Adopt a clear and consistent log structure to facilitate analysis and searching for information.



## 3- Gestion de réseau

<a id="affichage-configuration-reseau"></a>
### <span style="color:green;">- Affichage de la configuration réseau</span>

| Commande | Description | Options clés |
|---|---|---|
| `ip a` | Affiche les interfaces réseau et adresses IP. | `show`, `add`, `del` |
| `ip link` | Gère les interfaces réseau. | `set <interface> up/down`, `show` |
| `ip route` | Affiche et modifie les routes. | `show`, `add`, `del` |
| `ifconfig` | Ancienne commande pour afficher la configuration réseau. | `up`, `down`, `netmask`, `broadcast` |

<a id="surveillance-connexions-ports"></a>
### <span style="color:green;">- Surveillance des connexions et des ports</span>

| Commande | Description | Options clés |
|---|---|---|
| `ss -tulnp` | Liste les ports ouverts et les connexions actives. | `-t` (TCP), `-u` (UDP), `-l` (listening), `-n` (numérique), `-p` (processus) |
| `netstat -tulnp` | Alternative à `ss`, affiche les connexions réseau. | `-a` (tout), `-t` (TCP), `-u` (UDP), `-p` (PID) |
| `lsof -i` | Affiche les processus qui utilisent des connexions réseau. | `-i :80` (port spécifique), `-iTCP` |

<a id="capture-analyse-trafic"></a>
### <span style="color:green;">- Capture et analyse du trafic réseau</span>

| Commande | Description | Options clés |
|---|---|---|
| `tcpdump` | Capture et affiche le trafic réseau. | `-i eth0`, `-n` (pas de résolution DNS), `port 80` |
| `wireshark` | Interface graphique pour l'analyse du trafic. |  |
| `ngrep` | Recherche de motifs dans le trafic réseau. | `-d eth0 'GET'` (capture requêtes HTTP) |

<a id="gestion-regles-pare-feu"></a>
### <span style="color:green;">- Gestion des règles de pare-feu (iptables & nftables)</span>

| Commande | Description | Options clés |
|---|---|---|
| `iptables -L` | Liste les règles du pare-feu. | `-v` (détails), `-n` (numérique) |
| `iptables -A INPUT -p tcp --dport 22 -j ACCEPT` | Autorise SSH (port 22). | `-A` (ajouter), `-D` (supprimer), `-F` (flush) |
| `iptables -A INPUT -p tcp --dport 80 -j DROP` | Bloque HTTP (port 80). | `-p tcp` (protocole), `-j DROP` (action) |
| `iptables-save > rules.v4` | Sauvegarde les règles actuelles. |  |
| `iptables-restore < rules.v4` | Restaure les règles enregistrées. |  |
| `nft list ruleset` | Liste les règles nftables. |  |
| `nft add rule ip filter input tcp dport 22 accept` | Ajoute une règle acceptant SSH. |  |

<a id="diagnostic-tests-reseau"></a>
### <span style="color:green;">- Diagnostic et tests réseau</span>

| Commande | Description | Options clés |
|---|---|---|
| `ping google.com` | Teste la connectivité avec un hôte. | `-c 4` (nombre de paquets) |
| `traceroute google.com` | Affiche le chemin des paquets. | `-n` (évite DNS lookup) |
| `mtr google.com` | Alternative interactive à traceroute. | `-rw` (rapport en ligne de commande) |
| `dig google.com` | Recherche DNS avancée. | `@8.8.8.8 google.com` (serveur DNS spécifique) |
| `host google.com` | Résolution DNS rapide. |  |

<a id="configuration-surveillance-reseau"></a>
### <span style="color:green;">- Configuration et surveillance du réseau</span>

| Commande | Description | Options clés |
|---|---|---|
| `dhclient -r && dhclient eth0` | Renouvelle l'adresse IP via DHCP. |  |
| `nmcli` | Gère les connexions avec NetworkManager. | `connection show`, `device status` |
| `systemctl restart networking` | Redémarre les services réseau. |  |
| `ethtool eth0` | Affiche et modifie les paramètres d'une interface. | `-s eth0 speed 100 duplex full` |
| `iwconfig wlan0` | Affiche et configure une interface Wi-Fi. | `essid` (SSID), `mode` (Managed/Ad-hoc) |

## 4- stockage

<a id="affichage-espace-disque-partitions"></a>
### <span style="color:green;">- Affichage de l'espace disque et partitions</span>

| Commande | Description | Options clés / Astuces |
|---|---|---|
| `df -h` | Affiche l'espace disque utilisé et disponible. | `-h` (taille humaine), `-T` (type de FS) |
| `lsblk` | Liste les périphériques de stockage et leur hiérarchie. | `-f` (système de fichiers), `-o NAME,SIZE,MOUNTPOINT` |
| `fdisk -l` | Liste les partitions et informations des disques. | `-l` (liste toutes les partitions) |
| `blkid` | Affiche les UUID et types de systèmes de fichiers. | Utile pour identifier les disques |
| `mount` | Affiche les partitions montées ou monte un disque. | `mount /dev/sdb1 /mnt` |
| `umount` | Démonte un système de fichiers. | `umount /mnt` |
| `findmnt` | Liste les systèmes de fichiers montés en arbre. | `-t ext4` (filtrer par type) |

**Astuce ✨:** `df -ih` pour l'espace disque en inodes. 

<a id="gestion-partitions"></a>
### <span style="color:green;">- Gestion des partitions (fdisk, parted)</span>

| Commande | Description | Options clés |
|---|---|---|
| `fdisk /dev/sdX` | Outil interactif pour les partitions. | `n` (nouvelle partition), `d` (supprimer) |
| `parted /dev/sdX` | Outil avancé pour les partitions GPT et MBR. | `mklabel gpt`, `mkpart primary ext4 1MiB 100%` |
| `mkfs.ext4 /dev/sdX1` | Formate une partition en ext4. | `-L mydisk` (label) |
| `mkfs.xfs /dev/sdX1` | Formate en XFS. | `-f` (forcer le formatage) |
| `tune2fs -c 10 /dev/sdX1` | Check auto après 10 montages. | `-i 30d` (check après 30 jours) |

**Astuce ✨:** `parted` pour les disques GPT (> 2 To). 

<a id="gestion-avancee-stockage-lvm"></a>
### <span style="color:green;">- Gestion avancée du stockage avec LVM</span>

| Commande | Description | Options clés |
|---|---|---|
| `pvcreate /dev/sdX` | Initialise un disque pour LVM. |  |
| `vgcreate my_vg /dev/sdX` | Crée un volume group. |  |
| `vgdisplay` | Affiche les infos du VG. |  |
| `lvcreate -L 10G -n my_lv my_vg` | Crée un volume logique. | `-l 100%FREE` (tout l'espace libre) |
| `mkfs.ext4 /dev/my_vg/my_lv` | Formate le volume logique. |  |
| `mount /dev/my_vg/my_lv /mnt` | Monte le volume LVM. |  |
| `lvextend -L +5G /dev/my_vg/my_lv` | Augmente la taille du LV. |  |
| `resize2fs /dev/my_vg/my_lv` | Adapte le FS après l'extension. |  |
| `lvreduce -L 5G /dev/my_vg/my_lv` | Réduit un LV (⚠️ Risque de perte). | `e2fsck -f` avant réduction |
| `vgextend my_vg /dev/sdY` | Ajoute un disque au VG. |  |
| `vgreduce` | Retire un disque du VG. |  |

**Astuce ✨:** LVM idéal pour redimensionner sans redémarrer. 

<a id="controle-reparation-systemes-fichiers"></a>
### <span style="color:green;">- Contrôle et réparation des systèmes de fichiers</span>

| Commande | Description | Options clés |
|---|---|---|
| `fsck /dev/sdX1` | Vérifie et répare un système de fichiers. | `-y` (accepte les corrections) |
| `e2fsck -f /dev/sdX1` | Vérifie un système de fichiers ext4. |  |
| `xfs_repair /dev/sdX1` | Répare un système XFS. |  |
| `badblocks -sv /dev/sdX` | Vérifie les secteurs défectueux. |  |

**Astuce ✨:** `fsck` pour réparer un disque en lecture seule. 

<a id="sauvegarde-clonage-disques"></a>
### <span style="color:green;">- Sauvegarde et clonage de disques</span>

| Commande | Description | Options clés |
|---|---|---|
| `rsync -avh /source /destination` | Copie de fichiers en préservant les permissions. | `--progress` (afficher la progression) |
| `dd if=/dev/sdX of=/dev/sdY bs=4M status=progress` | Clone un disque brut (⚠️ Attention à l'ordre). |  |
| `tar -czf backup.tar.gz /home/user` | Archive un dossier en .tar.gz. | `-xzf` (extraction) |
| `mount -o loop image.iso /mnt` | Monte une image ISO. |  |

**Astuce ✨:** `rsync` pour copier un disque à chaud. 

<a id="surveillance-disques-performances"></a>
### <span style="color:green;">- Surveillance des disques et des performances</span>

| Commande | Description | Options clés |
|---|---|---|
| `iostat -dx 1` | Affiche l'utilisation des disques en temps réel. | `-x` (détails avancés) |
| `vmstat 1` | Surveille l'utilisation mémoire et disques. |  |
| `iotop` | Affiche les processus consommant le plus d'I/O. | `-o` (afficher seulement les actifs) |
| `smartctl -a /dev/sdX` | Vérifie l'état SMART d'un disque. | `-t short` (lance un test) |

**Astuce ✨:** `iotop` et `smartctl` pour détecter les pannes. 

<a id="chiffrement-securisation-donnees"></a>
### <span style="color:green;">- Chiffrement et sécurisation des données</span>

| Commande | Description | Options clés |
|---|---|---|
| `cryptsetup luksFormat /dev/sdX` | Chiffre un disque avec LUKS. |  |
| `cryptsetup open /dev/sdX my_secure_disk` | Monte un disque chiffré. | `close` pour démonter |
| `mkfs.ext4 /dev/mapper/my_secure_disk` | Formate la partition chiffrée. |  |

**Astuce ✨:** LUKS pour chiffrer un disque entier. 

## 5- Gestion des utilidateurs 

<a id="gestion-utilisateurs"></a>
### <span style="color:green;">- Gestion des utilisateurs</span>

| Commande | Description | Options clés / Astuces |
|---|---|---|
| `whoami` | Affiche l'utilisateur actuel. |  |
| `id` | Affiche l'UID, GID et groupes d'un utilisateur. | `id username` (voir un autre utilisateur) |
| `who` | Liste les utilisateurs connectés. |  |
| `w` | Affiche plus de détails sur les sessions actives. |  |
| `last` | Montre l'historique des connexions. | `last -a` (ajoute l'IP des connexions) |

**Astuce ✨:** Utiliser `w` au lieu de `who` pour voir la charge CPU et les processus actifs. 

<a id="creation-suppression-utilisateurs"></a>
### <span style="color:green;">- Création et suppression d'utilisateurs</span>

| Commande | Description | Options clés |
|---|---|---|
| `useradd -m username` | Crée un utilisateur avec son répertoire. | `-m` (crée `/home/username`) |
| `passwd username` | Définit ou modifie le mot de passe. |  |
| `usermod -l newname oldname` | Renomme un utilisateur. |  |
| `usermod -aG groupname username` | Ajoute un utilisateur à un groupe. | `-aG` (ajout sans retirer d'autres groupes) |
| `userdel -r username` | Supprime un utilisateur et son home. | `-r` (supprime les fichiers) |

**Astuce ✨:** Ne jamais modifier `/etc/passwd` à la main ! Utiliser `usermod`. 

<a id="gestion-mots-de-passe"></a>
### <span style="color:green;">- Gestion des mots de passe</span>

| Commande | Description | Options clés |
|---|---|---|
| `passwd username` | Modifie le mot de passe d'un utilisateur. |  |
| `passwd -l username` | Verrouille un compte. | `-u` (déverrouille) |
| `passwd -e username` | Force le changement au prochain login. |  |
| `chage -l username` | Affiche les infos d'expiration du mot de passe. |  |
| `chage -M 90 username` | Définit un mot de passe valide 90 jours. | `-W 7` (prévenir 7 jours avant expiration) |

**Astuce ✨:** Activer l'expiration automatique des mots de passe avec `chage -M 90 -W 7`. 

<a id="gestion-groupes"></a>
### <span style="color:green;">- Gestion des groupes</span>

| Commande | Description | Options clés |
|---|---|---|
| `groups username` | Liste les groupes d'un utilisateur. |  |
| `groupadd groupname` | Crée un groupe. |  |
| `groupdel groupname` | Supprime un groupe. |  |
| `usermod -aG sudo username` | Ajoute un utilisateur au groupe sudo. | `-aG` (ajout sans retirer les autres groupes) |
| `gpasswd -d username groupname` | Retire un utilisateur d'un groupe. |  |

**Astuce ✨:** Le groupe sudo permet d'exécuter des commandes root. Vérifier avec `groups username`. 

<a id="gestion-permissions-sudoers"></a>
### <span style="color:green;">- Gestion des permissions et sudoers</span>

| Commande | Description | Options clés |
|---|---|---|
| `chmod 755 file` | Modifie les permissions d'un fichier. | `777` (tout le monde peut tout faire) |
| `chown user:group file` | Change le propriétaire d'un fichier. | `-R` (récursivement) |
| `sudo visudo` | Modifie le fichier sudoers en toute sécurité. | Ajouter `username ALL=(ALL) NOPASSWD:ALL` |
| `sudo -l` | Liste les commandes sudo autorisées. |  |

**Astuce ✨:** Ne jamais modifier `/etc/sudoers` directement ! Utiliser `visudo`. 

<a id="verrouillage-gestion-avancee-comptes"></a>
### <span style="color:green;">- Verrouillage et gestion avancée des comptes</span>

| Commande | Description | Options clés |
|---|---|---|
| `usermod -L username` | Verrouille un utilisateur. | `-U` (déverrouille) |
| `faillog -u username` | Affiche les tentatives de connexion échouées. | `faillog -r -u username` (réinitialise) |
| `kill -9 -1` | Déconnecte un utilisateur en session (⚠️ Ne pas exécuter en tant que root). |  |
| `pkill -u username` | Déconnecte un utilisateur spécifique. |  |

**Astuce ✨:** Utiliser `faillog` pour détecter les tentatives de connexion échouées.

## Supervision système

<a id="sar-statistiques-systeme"></a>
### <span style="color:green;">1. sar - Collecte et affichage des statistiques système</span>

Le System Activity Report (sar) collecte et affiche des données sur l'utilisation des ressources (CPU, mémoire, disque, réseau).

| Commande | Description |
|---|---|
| `sar -u 5 10` | Affiche l'utilisation CPU toutes les 5 sec, 10 fois. |
| `sar -q 1 5` | Affiche la charge système toutes les 1 sec, 5 fois. |
| `sar -r 2 5` | Affiche l'utilisation de la mémoire toutes les 2 sec, 5 fois. |
| `sar -n DEV 1 5` | Supervise l'activité réseau par interface. |
| `sar -d 2 3` | Affiche l'activité disque toutes les 2 sec, 3 fois. |
| `sar -W 1 5` | Surveille l'utilisation du swap. |
| `sar -f /var/log/sa/sa10` | Affiche les stats collectées le 10 du mois. |
| `sar -o stats.sar 10 5` | Enregistre les données pour analyse ultérieure. |
| `sar -f stats.sar` | Lit les données enregistrées. |

**Astuce ✨:** Enregistrer et analyser les données pour une analyse ultérieure.

<a id="iostat-surveillance-io-cpu"></a>
### <span style="color:green;">2. iostat - Surveillance des entrées/sorties disque et CPU</span>

L'outil iostat permet d’analyser l'activité des disques et l’utilisation CPU pour détecter des problèmes liés au stockage.

| Commande | Description |
|---|---|
| `iostat` | Affiche un résumé des stats CPU et disques. |
| `iostat -c 2 5` | Surveille l'utilisation CPU toutes les 2 sec, 5 fois. |
| `iostat -d 1 10` | Supervise l’activité disque toutes les 1 sec, 10 fois. |
| `iostat -x` | Affiche des stats détaillées des disques. |
| `iostat -x /dev/sda 1 10` | Analyse uniquement /dev/sda. |
| `iostat -x | sort -k 2 -nr` | Trie les disques par taux d'utilisation. |

**Astuce :** Trouver le disque le plus utilisé.

<a id="vmstat-memoire-cpu-swap"></a>
### <span style="color:green;">3. vmstat - Surveillance de la mémoire, CPU et swap</span>

L'outil vmstat affiche des statistiques sur la mémoire vive, le swap, les processus et l'utilisation CPU.

| Commande | Description |
|---|---|
| `vmstat 1 10` | Affiche les stats toutes les 1 sec, 10 fois. |
| `vmstat -s` | Affiche un résumé détaillé de l'état mémoire. |
| `vmstat -d` | Affiche les stats d’utilisation des disques. |
| `vmstat -p /dev/sda` | Supervise une partition spécifique. |
| `vmstat -a` | Affiche les pages allouées en mémoire. |
| `vmstat 1 5 | awk '{print $7}'` | Vérifie l'utilisation du swap. |

**Astuce ✨:** Détecter un problème de swap.

<a id="top-htop-surveillance-processus"></a>
### <span style="color:green;">4. top et htop - Surveillance des processus</span>

L’outil top permet de surveiller les processus en temps réel.

| Commande | Description |
|---|---|
| `top` | Affiche les processus actifs en temps réel. |
| `top -o %MEM` | Trie par consommation mémoire. |
| `top -o %CPU` | Trie par utilisation CPU. |
| `htop` | Alternative plus ergonomique. |

<a id="free-memoire-ram-swap"></a>
### <span style="color:green;">5. free - Surveillance de la mémoire RAM et swap</span>

| Commande | Description |
|---|---|
| `free -m` | Affiche la mémoire en Mo. |
| `free -g` | Affiche la mémoire en Go. |
| `free -h` | Affiche un format lisible humainement. |
| `watch -n 1 free -m` | Met à jour la mémoire toutes les 1 sec. |

**Astuce ✨:** Afficher en continu.

<a id="uptime-load-average-charge"></a>
### <span style="color:green;">6. uptime et load average - Vérifier la charge du système</span>

| Commande | Description |
|---|---|
| `uptime` | Affiche l'heure, le temps d’uptime et la charge système. |
| `cat /proc/loadavg` | Affiche la charge moyenne. |

**Astuce ✨:** Comprendre load average (1.23 0.98 0.75 - charge sur 1 min, 5 min, 15 min).

<a id="dstat-monitoring-temps-reel"></a>
### <span style="color:green;">7. dstat - Outil avancé de monitoring en temps réel</span>

L'outil dstat combine vmstat, iostat, netstat et mpstat pour un monitoring en temps réel.

| Commande | Description |
|---|---|
| `dstat` | Affiche un résumé des ressources utilisées. |
| `dstat -c --top-cpu` | Affiche les processus les plus gourmands en CPU. |
| `dstat -d --top-io` | Affiche les processus consommant le plus d’E/S disque. |
| `sudo apt install dstat` | Installe dstat (Debian/Ubuntu). |
| `sudo yum install dstat` | Installe dstat (RedHat/CentOS). |


![alt text](https://lh3.googleusercontent.com/gg/AJxt1KPMIsAPkGCMm8orufWRCQ76_8WwPdSCOvpV7u4FIzAVgcLyB5v9Q04pqLd5XBUhufRU2i52mrogiiPfA-QXxQaoxnkU6dGqp-i7qSMJ6recYt09A4c_AbEVSEltbEfq4o01bc99xXO4DYfgV-tQTUTW8BM9u0KvccTPc_Q5dW9EMbA7U4Aq "usefull-commands") 
