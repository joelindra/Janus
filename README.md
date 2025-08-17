# Janus Shell v2.0

<img width="364" height="437" alt="image" src="https://github.com/user-attachments/assets/54b12362-b54b-4f3c-be7a-e49fe1cdbd29" />
-----

Janus Shell is a powerful, feature-rich PHP web shell with a modern, responsive user interface. It is designed for penetration testers and security professionals for authorized remote server administration and post-exploitation. It provides a comprehensive suite of tools within a single PHP file, making it easy to deploy and manage.

## ✨ Features

Janus Shell is packed with features to provide complete control over a web server environment.

### **Core Interface**

  * **Modern UI:** A clean, dark-themed, and responsive single-page application (SPA) interface built for usability.
  * **Live Dashboard:** Get real-time statistics for CPU, RAM, and Disk usage.
  * **System Information:** Detailed information about the server OS, PHP version, user, IP addresses, and disabled PHP functions.
  * **Mobile Friendly:** The interface is fully responsive and usable on mobile devices.

### **File Management**

  * **AJAX-driven File Manager:** Browse directories, view file details, and navigate the filesystem without page reloads.
  * **Full CRUD Operations:** Create, Delete, Rename files and directories.
  * **Advanced File Editor:** An in-browser editor powered by **CodeMirror** with syntax highlighting for various languages.
  * **File Upload/Download:** Easily upload multiple files directly to the current directory or download files from the server.
  * **Mass Uploader:** Upload a single file to multiple selected directories at once using a directory tree browser.
  * **Permissions Management:** View permissions in both octal (`0755`) and symbolic (`drwxr-xr-x`) formats. Change file permissions directly.
  * **Archiving:** Create ZIP archives from files/directories and extract ZIP archives on the server.

### **Execution & Control**

  * **Interactive Terminal:** A pseudo-terminal for executing shell commands, with command history support.
  * **PHP Code Evaluator:** Run PHP code on the fly and see the output immediately.
  * **Process Manager:** View a list of all running processes on the server (`ps aux`).

### **Networking & Security**

  * **Back Connect / Reverse Shell:** Easily establish a reverse shell connection to a listener for deeper interaction.
  * **Port Scanner:** A simple TCP port scanner to probe for open ports on a given host.
  * **Network Information:** View network interface details (`ip addr`/`ifconfig`) and active connections (`netstat`).
  * **SUID/GUID Scanner:** A security auditing tool to find files with potentially exploitable SUID/GUID permissions for privilege escalation reconnaissance.
  * **Wget (Downloader):** Fetch files from any URL and save them directly to the server.

### **Database Management**

  * **MySQLi Client:** Connect to a MySQL/MariaDB database and execute SQL queries directly from the shell. View results in a clean, tabulated format.

### **Stealth & Evasion**

  * **Base64 Communication:** All communication between the client and server is Base64 encoded to obscure traffic from basic inspection.
  * **Self-Destruct:** A one-click function to completely remove the shell script from the server.
-----

## Screenshots

<img width="1556" height="789" alt="image" src="https://github.com/user-attachments/assets/77da6b6b-92da-4956-a78b-c9356458aec4" />
<img width="1901" height="796" alt="image" src="https://github.com/user-attachments/assets/89e95beb-aca3-4e19-b4fa-ed6a33e47b9c" />

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](https://www.google.com/search?q=LICENSE) file for details.

**Author:** Anonre / [joelindra](https://github.com/joelindra)
