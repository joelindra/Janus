# Janus Web Shell v6.0

<div align="center">

![Version](https://img.shields.io/badge/version-6.0-blue.svg)
![PHP](https://img.shields.io/badge/PHP-7.0%2B-purple.svg)
![License](https://img.shields.io/badge/license-Authorized%20Use%20Only-red.svg)

**Advanced PHP Web Shell with Modern UI and Advanced Security Features**

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Documentation](#-documentation) • [Warning](#-warning)

</div>

---

## 📋 Description

**Janus** is a sophisticated PHP web shell designed for authorized system administration and penetration testing. It features a modern, intuitive web interface with comprehensive security features, anti-delete protection, and advanced WAF bypass capabilities.

### Key Highlights

- 🎨 **Modern UI** - Beautiful dark-themed interface with responsive design
- 🛡️ **Auto-Defend** - Multi-layer protection system with auto-restore
- 🔒 **Anti-Delete** - Advanced backup and watchdog system
- 🌐 **Network Tools** - Port scanning, reverse/bind shells, port forwarding
- 🗄️ **Database Management** - MySQL support with query execution
- 🔍 **Discovery Tools** - File search, credential harvesting, domain intelligence
- 🚀 **80+ Features** - Comprehensive toolset for system administration

---

## ⚠️ WARNING

> **This software is intended ONLY for authorized use.**
> 
> Unauthorized access to computer systems is illegal and may result in severe legal consequences. Users are solely responsible for ensuring they have proper authorization before using this tool. The authors and contributors are not responsible for any misuse or damage caused by this software.

---

## 🎯 Features

### Core Features

- **🛡️ Auto-Defend & Anti-Delete Protection**
  - Multi-layer protection system
  - Auto-restore mechanism
  - Real-time monitoring
  - Command blocking

- **📁 File Management**
  - Advanced file browser with syntax highlighting
  - File editor with CodeMirror integration
  - Mass upload/download
  - Archive operations (zip/unzip)

- **💻 Command Execution**
  - Multiple execution methods with fallback
  - PHP eval support
  - Interactive terminal interface
  - Command chaining support

- **🌐 Network Tools**
  - Port scanner
  - Reverse/Bind shell
  - Port forwarding
  - C2 communication
  - Remote file download (wget)

- **🗄️ Database Management**
  - MySQL query execution
  - Database/column dumper
  - WordPress user creation
  - Config file finder

- **📊 System Information**
  - Real-time system stats (CPU, RAM, Disk)
  - System profiler
  - Process manager
  - User/group management

- **🔒 Security & Stealth**
  - WAF bypass testing
  - Advanced log cleaner
  - Stealth features
  - Timestomp

- **🔄 Persistence & Recovery**
  - Enhanced persistence (cron/htaccess)
  - Multi-location backup
  - Auto-restore system

- **🎯 Multi-Shell Management**
  - Shell registry
  - Command broadcasting
  - Remote shell support

- **🔐 Encryption & Encoding**
  - HADES multi-layer encryption
  - WAF evasion encoding
  - Code obfuscator
  - File encryption/decryption

- **🔍 Search & Discovery**
  - File/content search
  - Credential harvester
  - Domain intelligence
  - SUID/GUID finder

- **⚙️ System Administration**
  - Cron management
  - SSH key manager
  - Firewall control
  - Sudo checker

- **💉 Code Injection & Backdoors**
  - Code injection
  - Backdoor installer
  - Web shell generator/lister

- **🚀 Advanced Features**
  - Privilege escalation checker
  - Subnet scanner
  - Exploit suggester
  - Data exfiltration
  - Memory dump analysis
  - DNS tunneling
  - Password cracking
  - Ransom creator/decryptor
  - Phishing page deployer
  - And many more...

---

## 📦 Installation

### Requirements

- PHP 7.0 or higher
- Web server (Apache/Nginx)
- Write permissions in target directory

### Quick Start

1. **Upload the file**
   ```bash
   # Upload janus.php to your target server
   chmod 644 janus.php
   ```

2. **Access the shell**
   ```
   http://your-server/janus.php
   ```

3. **First-time setup**
   - Shell will automatically setup protection on first access
   - Secret token will be generated and stored
   - Backup and watchdog files will be created

---

## 🚀 Usage

### Basic Operations

#### File Management
- Navigate directories using the File Manager
- Edit files with syntax highlighting
- Upload/download files
- Create/delete files and directories

#### Command Execution
- Execute system commands via Terminal
- Run PHP code directly with PHP Eval
- View real-time output

#### Network Operations
- Scan ports on target hosts
- Establish reverse/bind shells
- Forward ports for tunneling
- Download files from remote URLs

#### Database Operations
- Connect to MySQL databases
- Execute SQL queries
- Dump databases/tables
- Create WordPress admin users

### Advanced Features

See [Complete Documentation](JANUS_DOCUMENTATION.md) for detailed usage instructions for all 80+ features.

---

## 📚 Documentation

For complete documentation, see [JANUS_DOCUMENTATION.md](JANUS_DOCUMENTATION.md)

The documentation includes:
- Detailed feature descriptions
- Usage guides for all features
- Configuration options
- API reference
- Troubleshooting guide

---

## 🛡️ Security Features

### Auto-Defend System
- `.htaccess` protection with secret token
- PHP-based fallback for Nginx
- Auto-restore redirect mechanism

### Anti-Delete Protection
- Multiple backup locations
- Watchdog system for auto-restore
- Real-time monitoring
- Command blocking

### WAF Evasion
- Multiple encoding methods
- Case variation
- Comment injection
- Whitespace manipulation
- String concatenation

---

## 📡 API

Janus uses an action-based API system. All requests are sent via POST with an `action` parameter.

### Example Request

```javascript
{
    action: 'browse',
    path: '/var/www/html'
}
```

### Available Actions

- File Management: `browse`, `get_file_content`, `save_file`, `delete`, `create`, `rename`, `chmod`, `zip`, `unzip`
- Command Execution: `exec`, `php_eval`
- Network: `port_scan`, `reverse_shell`, `bind_shell`, `wget`, `c2_communicate`
- Database: `database_query`, `database_dumper`, `column_dumper`
- System: `get_live_stats`, `system_profiler`, `get_users_groups`, `get_kernel_info`
- Security: `waf_bypass_test`, `log_cleaner`, `advanced_log_cleaner`
- Advanced: `multi_shell_register`, `enhanced_persistence_install`, `multi_location_backup`

See [Complete Documentation](JANUS_DOCUMENTATION.md) for full API reference.

---

## 🐛 Troubleshooting

### Shell Cannot Be Accessed
- Check file permissions: `chmod 644 janus.php`
- Check `.htaccess` restrictions
- Use secret token: `?janus_token=SECRET_TOKEN`
- Verify PHP functions are not disabled

### Command Execution Failed
- Shell automatically falls back to alternative execution methods
- Check `disable_functions` in php.ini
- Verify user permissions

### Auto-Defend Not Working
- Ensure server supports `.htaccess` (Apache) or use PHP-based protection (Nginx)
- Check write permissions in directory

---

## 📝 Important Notes

1. **Password Protection**: Change default password after first access
2. **Auto-Defend**: Enabled automatically on first access
3. **Anti-Delete**: Active by default with auto-restore
4. **WAF Evasion**: Multiple techniques available, no 100% guarantee
5. **Logging**: Some features may leave traces - use log cleaner
6. **Persistence**: Can be detected by security tools - use with caution

---

## 🔄 Updates

### Version History

- **v6.0** - Current version with enhanced WAF evasion and bug fixes
  - Enhanced auto-defend system
  - Improved anti-delete protection
  - Advanced features suite
  - Modern UI improvements

---

## 📚 Reference

### Main Functions

- `setup_auto_defend($shell_path)` - Setup auto-defend protection
- `setup_anti_delete($shell_path)` - Setup anti-delete protection
- `hades_encrypt($data, $password)` - Multi-layer encryption
- `waf_evade_encode($data, $method)` - WAF evasion encoding
- `execute_command($cmd)` - Command execution with fallback

---

## ⚖️ License & Disclaimer

This software is provided for **educational and authorized use only**. 

**IMPORTANT**: 
- Unauthorized access to computer systems is illegal
- Users are fully responsible for their actions
- Authors are not liable for misuse
- Use only on systems you own or have explicit permission to test

---

## 👤 Author

**Joel Indra**

- GitHub: [@joelindra](https://github.com/joelindra)

---
