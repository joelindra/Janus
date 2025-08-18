## Janus v5.0 - Anti Logger

Janus v5.0 is a sophisticated and feature-rich web shell designed for penetration testers and security professionals. It provides a comprehensive suite of tools for post-exploitation, privilege escalation, and network reconnaissance, all accessible through a modern and intuitive web interface.

<img width="364" height="437" alt="image" src="https://github.com/user-attachments/assets/54b12362-b54b-4f3c-be7a-e49fe1cdbd29" />

### Features

Janus v5.0 is equipped with a wide array of functionalities, categorized for ease of use:

#### **Core & File Management**
* **Dashboard:** An overview of the system with live stats on CPU, RAM, and disk usage.
* **File Manager:** A comprehensive file explorer with capabilities to browse, view, edit, create, rename, delete, and manage permissions of files and directories.
* **Uploader:** Upload single or multiple files to the target server.
* **Mass Uploader:** Upload a single file to multiple directories simultaneously.
* **Zipper/Unzipper:** Create and extract zip archives.
* **Self-Destruct:** Remove the web shell from the server with a single click.

#### **Command & Control**
* **Terminal:** An interactive terminal for executing system commands.
* **PHP Eval:** Execute arbitrary PHP code on the server.
* **Reverse Shell:** Establish a reverse shell connection to a specified IP and port.
* **Bind Shell:** Create a bind shell on the server for remote access.

#### **Reconnaissance & Enumeration**
* **Domain Intel:** Gather intelligence on the server's domain, including DNS records, other sites on the same server, and common subdomains.
* **Port Scanner:** Scan for open ports on a given host.
* **SUID/GUID Finder:** Locate files with SUID/GUID permissions for potential privilege escalation.
* **User & Group Enumeration:** List all users and groups on the system.
* **Kernel Info:** Display detailed information about the server's kernel and operating system.
* **Config Grabber:** Automatically search for and display common configuration files.
* **Server Fingerprint:** Gather detailed information about the server's software, services, and packages.
* **Find Writable Files/Dirs:** Locate world-writable files and directories.

#### **Privilege Escalation & Post-Exploitation**
* **Privilege Escalation Checker:** Run automated checks for common privilege escalation vectors on both Linux and Windows.
* **Credential Harvester:** Search for credentials, API keys, and private keys within a directory.
* **Log Cleaner:** Remove specific lines from log files to cover tracks.
* **Sudo Check:** Check the current user's sudo permissions.
* **SSH Manager:** View and add SSH keys to the `authorized_keys` file for persistent access.
* **WordPress Admin Creator:** Create a new WordPress administrator user by providing the path to `wp-config.php`.
* **cPanel Credential Finder:** Search for cPanel credential files.
* **Symlink cPanel:** Attempt to read config files of other users on a shared hosting environment via symbolic links.

#### **Network & Pivoting**
* **Subnet Scanner:** Scan an internal network range to discover live hosts and open ports.
* **Port Forwarder:** Forward a local port to a remote host and port, enabling access to internal services.
* **Firewall Control:** View and flush firewall rules (iptables).
* **Wget:** Download files from a specified URL.

#### **Attack & Evasion**
* **Phishing Page Deployer:** Deploy a generic admin login phishing page.
* **Timestomp:** Change the timestamp of a file to match another file, helping to evade detection.
* **Code Injector:** Inject custom PHP code into existing files.
* **Backdoor Installer:** Inject a simple `shell_exec` backdoor into specified files.
* **CPU Hog:** Run an intensive process to consume CPU resources, potentially causing a denial of service.
* **Keylogger (Experimental):** Attach to a running process and capture read/write syscalls.

#### **Data Management & Exfiltration**
* **Database Client:** A MySQLi client to execute queries on the server's database.
* **Data Exfiltration Packager:** Create a downloadable ZIP archive of selected files and directories.
* **Exfiltrate via Pastebin:** Upload the content of a file to a public pastebin service.
* **Sensitive File Finder:** Scan a directory for files containing sensitive data or with sensitive extensions.
* **Change Monitor:** Monitor a directory for a specified duration and report any file changes.

## Disclaimer

This tool is provided for educational and authorized security testing purposes only. Unauthorized use of this tool to access systems without permission is illegal. The developers assume no liability and are not responsible for any misuse or damage caused by this tool. By using this software, you agree to use it responsibly and in compliance with all applicable laws.

## Screenshot

<img width="1606" height="898" alt="image" src="https://github.com/user-attachments/assets/1c60f8db-b882-4eed-83a1-d4280f69fbf3" />
<img width="1675" height="903" alt="image" src="https://github.com/user-attachments/assets/a0532bce-5c14-4286-b91a-ee10287f02bd" />
<img width="1251" height="880" alt="image" src="https://github.com/user-attachments/assets/74b6dce7-f2cc-4d83-b06d-5b00e7630174" />

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

**Remember: With great power comes great responsibility. The developers are not responsible for any misuse or illegal activities conducted with this tool.**
