<xaiArtifact artifact_id="287761b6-750d-4d6e-9d37-62e7db248c64" artifact_version_id="ae71304a-003c-49bb-92f3-a76fd7958104" title="README.md" contentType="text/markdown">

# Janus Shell v3.0

Janus Shell is a PHP-based web shell designed for system administration and security testing. It provides a feature-rich interface for managing files, executing commands, interacting with databases, scanning networks, and more, all from a web browser. This tool is intended for **authorized use only** on systems where you have explicit permission to perform such activities. Unauthorized use may be illegal and unethical.

<img width="364" height="437" alt="image" src="https://github.com/user-attachments/assets/54b12362-b54b-4f3c-be7a-e49fe1cdbd29" />

## Features

- **Dashboard**: Displays system information (OS, PHP version, user, etc.) and live system stats (CPU, RAM, disk usage).
- **File Manager**: Browse, upload, download, create, rename, delete, and change permissions for files and directories. Supports ZIP creation and extraction.
- **Terminal**: Execute system commands with a terminal-like interface, including command history and directory navigation.
- **Database Client**: Run MySQL queries with a simple interface to view results or perform database operations.
- **Connect**: Establish reverse or bind shells for remote command execution (requires compatible server configuration).
- **Process List**: View running processes with the ability to refresh the list.
- **Network Tools**: Perform port scanning and view network interface and connection details.
- **PHP Code Evaluator**: Execute arbitrary PHP code (if `eval` is enabled on the server).
- **Mass Uploader**: Upload a single file to multiple directories simultaneously.
- **Enumeration**: Scan for SUID/GUID files, enumerate users and groups, and retrieve OS/kernel information for security assessments.
- **Cronjob Manager**: View and edit the current user's crontab for scheduling tasks.
- **Tools**: Download files via `wget`, view PHP configuration (`phpinfo`), and a self-destruct option to remove the shell.

## Usage

1. **Dashboard**: View system stats and information upon loading the shell.
2. **File Manager**: Navigate directories, upload files, or edit files using the built-in CodeMirror editor.
3. **Terminal**: Run commands like `ls`, `cat`, or `cd` to interact with the server’s file system.
4. **Database**: Input MySQL credentials and run queries to manage databases.
5. **Connect**: Set up reverse or bind shells for advanced remote access.
6. **Network Tools**: Scan ports or view network configurations.
7. **Security Enumeration**: Use tools to find SUID/GUID files, list users/groups, or check kernel details.
8. **Cron Manager**: Edit crontabs to schedule tasks.
9. **Self-Destruct**: Permanently delete the shell from the server when done (use with caution).

## Requirements

- PHP 5.6 or higher
- Web server (e.g., Apache, Nginx)
- Optional PHP extensions: `mysqli`, `zip`
- Read/write/execute permissions for certain features
- Compatible OS for system commands (Linux, Unix, or Windows)

## Screenshots

<img width="1626" height="899" alt="image" src="https://github.com/user-attachments/assets/9eb009ee-9579-4395-9620-a186b5e2adf1" />
<img width="1301" height="829" alt="image" src="https://github.com/user-attachments/assets/c293e529-49d6-458c-ad7c-60cd50d58b96" />
<img width="1143" height="792" alt="image" src="https://github.com/user-attachments/assets/23bf9897-8e54-4489-87e2-04c56428b228" />

## Credits

Created by [Anonre](https://github.com/joelindra). Built with modern web technologies, including CodeMirror for code editing and a responsive interface for ease of use.

**Disclaimer**: The author is not responsible for any misuse of this tool. Always obtain proper authorization before deploying or using Janus Shell on any system.

</xaiArtifact>
