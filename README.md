![Janus Shell Interface](https://img.shields.io/badge/Version-1.0--Stealth-blue.svg)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Janus Web Shell is a powerful, feature-rich PHP-based web shell designed for system administration, file management, and server monitoring. It provides a modern, user-friendly interface for interacting with server resources, executing commands, and performing security audits. **Use this tool responsibly and only on systems where you have explicit permission.**

<img width="364" height="437" alt="image" src="https://github.com/user-attachments/assets/54b12362-b54b-4f3c-be7a-e49fe1cdbd29" />

## Features

- **File Management**: Browse, edit, upload, download, zip/unzip, create, rename, delete, and change permissions of files and directories.
- **Terminal Emulator**: Execute shell commands directly from the browser with a fully interactive terminal interface.
- **System Monitoring**: View real-time CPU, RAM, and disk usage with a sleek dashboard.
- **Network Tools**: Perform port scanning and retrieve network interface and connection information.
- **PHP Code Evaluation**: Safely execute PHP code with output displayed in real-time.
- **Mass File Uploader**: Upload a single file to multiple directories efficiently.
- **Security Auditing**: Scan for SUID/GUID files and retrieve detailed network information.
- **Self-Destruct Mechanism**: Securely delete the shell from the server when needed.
- **Responsive Design**: Modern, dark-themed UI with CodeMirror integration for code editing.
- **Cross-Platform Support**: Compatible with Linux, BSD, and other UNIX-like systems (limited Windows support).

### Dashboard
- Displays system information (OS, hostname, IP, PHP version, etc.).
- Shows real-time CPU, RAM, and disk usage with progress bars.

### File Manager
- Navigate directories, view file details (size, permissions, modification time).
- Perform actions like creating files/directories, uploading, downloading, zipping, unzipping, renaming, deleting, and changing permissions.
- Edit text files with a built-in CodeMirror editor or view media files (images/videos).

### Terminal
- Execute shell commands with real-time output.
- Supports `cd` for directory navigation and updates the file manager context accordingly.
- Command history with arrow key navigation.

### Processes
- View running processes using `ps aux` (or equivalent for your OS).
- Refresh process list on demand.

### Network Tools
- **Port Scanner**: Scan specified ports on a host to check if they are open or closed.
- **Network Info**: Retrieve interface details (`ip addr` or `ifconfig`) and active connections (`netstat` or `sockstat`).

### PHP Evaluator
- Execute arbitrary PHP code (if `eval` is enabled on the server).
- View output in a formatted console.

### Mass Uploader
- Upload a single file to multiple directories selected via an interactive directory tree.

### Security Auditing
- Scan for SUID/GUID files to identify potential security risks.
- Retrieve detailed network interface and connection information.

### Wget & System
- Download files from URLs directly to the server.
- View PHP configuration via `phpinfo()`.
- Use the self-destruct feature to permanently remove the shell.

## Screenshots

<img width="1900" height="992" alt="image" src="https://github.com/user-attachments/assets/ebd64606-f38b-4a6b-8add-b30eed4d544d"/>
<img width="1918" height="821" alt="image" src="https://github.com/user-attachments/assets/92432cc7-2dd0-42f4-83e6-61eafe11e7e0" />
<img width="1423" height="754" alt="image" src="https://github.com/user-attachments/assets/4fad8f57-2805-434d-a746-81c8fa946388" />

## Security Considerations

- **Authorized Use Only**: This tool is intended for legal and authorized system administration. Unauthorized access to systems is illegal and unethical.
- **File Permissions**: Restrict access to the script (e.g., use `.htaccess` or server authentication).
- **Self-Destruct**: Use the self-destruct feature to remove the shell when no longer needed.
- **Disabled Functions**: The shell checks for disabled PHP functions and gracefully handles restrictions.
- **Secure Deployment**: Deploy on HTTPS servers to prevent interception of sensitive data.

## Requirements

- **PHP**: Version 7.4 or higher.
- **Web Server**: Apache, Nginx, or any PHP-compatible server.
- **Optional PHP Extensions**:
  - `ZipArchive` for zip/unzip functionality.
  - `fsockopen` for port scanning.
- **Browser**: Modern browser with JavaScript enabled.
- **Dependencies**: CodeMirror (loaded via CDN) for the code editor.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Created by [Joel Indra](https://github.com/joelindra).
- Inspired by the need for a secure, modern, and feature-rich web shell.
