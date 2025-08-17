# Janus Shell v4.0 - Advanced PHP Web Shell - Anti Logger!

![Version](https://img.shields.io/badge/version-4.0-blue)
![PHP](https://img.shields.io/badge/PHP-7.0%2B-green)
![License](https://img.shields.io/badge/license-MIT-red)

Janus Shell is a sophisticated PHP web shell designed for authorized security testing, system administration, and educational purposes. It provides a comprehensive set of tools for file management, system exploration, network operations, and post-exploitation tasks.

<img width="364" height="437" alt="image" src="https://github.com/user-attachments/assets/54b12362-b54b-4f3c-be7a-e49fe1cdbd29" />

## ⚠️ Important Notice

**This tool is intended for authorized use only. Unauthorized access to computer systems is illegal. Use only on systems you own or have explicit permission to test. The developers are not responsible for any misuse or illegal activities conducted with this tool.**

## Features

### Core Functionality
- **File Manager**: Browse, upload, download, edit, delete, and modify file permissions
- **Terminal**: Execute shell commands with history navigation
- **Database Client**: MySQLi interface for database operations
- **System Information**: Comprehensive system details and live resource monitoring

### Network Tools
- **Port Scanner**: Identify open ports on target systems
- **Reverse/Bind Shells**: Establish remote connections
- **Port Forwarding**: Pivot through compromised systems
- **Mass Uploader**: Distribute files to multiple directories

### Security & Enumeration
- **Privilege Escalation**: SUID/GUID discovery, sudo permissions check
- **User/Group Enumeration**: System user and group analysis
- **Kernel Information**: OS version and exploit suggestions
- **Credential Harvesting**: Search for credentials and API keys
- **Config File Discovery**: Locate common configuration files

### Post-Exploitation
- **Persistence Methods**: SSH key management, .htaccess backdoors
- **Log Cleaning**: Remove traces from log files
- **Code Injection**: Backdoor existing files
- **Cron Manager**: Schedule tasks for persistence

### Additional Tools
- **PHP Code Evaluator**: Execute arbitrary PHP code
- **File Search**: Find files by name or content
- **Timestomp**: Modify file timestamps
- **Self-Destruct**: Remove the shell after use

## Requirements

- PHP 7.0 or higher
- Common PHP extensions (mysqli, sockets, zip, etc.)
- Web server (Apache, Nginx, etc.)
- Browser with JavaScript support

## Usage

### Basic Navigation
- Use the sidebar to switch between different tool categories
- Each section provides an intuitive interface for its specific functions
- Most operations provide feedback through toast notifications

### File Management
- Navigate directories by clicking on folder names
- Upload files using the "Upload" button
- Edit files by clicking on their names
- Change permissions with the 🔒 icon
- Delete files/folders with the 🗑️ icon

### Terminal
- Type commands directly into the terminal input
- Use arrow keys to navigate command history
- The terminal maintains your current working directory

### Database Operations
1. Enter database connection details (host, user, password, database name)
2. Write your SQL query in the text area
3. Click "Execute Query" to run the query
4. Results will be displayed in a formatted table

### Security Testing
- Use the "Enumeration" section to gather system information
- Check for privilege escalation opportunities
- Harvest credentials from configuration files
- Establish persistence for continued access

## Screenshots

<img width="1675" height="867" alt="image" src="https://github.com/user-attachments/assets/fe6e4870-bada-4b40-9a89-8e2a380d8076" />
<img width="1675" height="867" alt="image" src="https://github.com/user-attachments/assets/d8ddab8d-aeae-40f7-8019-e2ba3ac5580a" />
<img width="1361" height="905" alt="image" src="https://github.com/user-attachments/assets/4dcba90c-4f80-430b-a885-0ec0ed0ac502" />

## Disclaimer

This tool is provided for educational and authorized security testing purposes only. Unauthorized use of this tool to access systems without permission is illegal. The developers assume no liability and are not responsible for any misuse or damage caused by this tool. By using this software, you agree to use it responsibly and in compliance with all applicable laws.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

**Remember: With great power comes great responsibility. The developers are not responsible for any misuse or illegal activities conducted with this tool.**
