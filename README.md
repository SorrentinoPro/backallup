# Backallup: 
### A Backup Tool for Linux Systems
Lightweight, easy-to-use command-line backup tool for Linux systems. Create backups of files, directories, or entire systems with customizable options.

## Overview
Backallup is a command-line backup tool designed for Linux systems. It provides a simple and efficient way to create backups of files, directories, and entire systems. With Backallup, you can easily create and manage backups, ensuring that your data is safe and secure.

## Key Features
- Easy to use command-line interface
- Flexible backup options for files, directories, and entire systems
- Customizable backup process with include/exclude options
- Robust error handling for reliable backups
- Schedule cron jobs seamlessly

## Installation
### apt install
```bash
apt install backallup
```
or
### Clone the repository
```bash
git clone https://github.com/SorrentinoPro/backallup.git
```

### Change into the repository directory
```bash
cd backallup
```
### Make the backallup_installer script executable
```bash
chmod +x ./backallup_installer
```

### Run the installer script
```bash
./backallup_installer
```
### Directory Structure post installation:
```
/.backallup/
    ├── backups/
    ├── LICENSE
    ├── README.md
```

## Usage

### Create a backup of a specific file or directory
```bash
backallup <file_or_directory>
```

### Create a backup of the entire system
```bash
backallup -server
```
or skip the .backallup/backups folder containig all backups
```bash
backallup -s --skipbks 
```

### Create a backup of a specific profile
For all domains in profile backup
```bash
backallup -p <profilename>
```
or profile specific domain backup
```bash
backallup -p <profilename> -d <domain>
```

### Restore a backup from a custom tar.gz file
Restore to copy path adding a __BAU extension 
```bash
backallup -r <custom_tar_gz_file>
```
or Restore to original path
```bash
backallup -r <custom_tar_gz_file> -o
```

### Yes to all prompts, avoiding all prompts selecting defaults (useful for complex integretions)
```bash
backallup <ANY PARAMETERS> -y
```

### Create a crontab job for the same command 
```bash
backallup <ANY PARAMETERS> -j
```

### Profiles
Backallup includes several pre-defined profiles for common use cases. Up to date list of supported profiles are:

*** 
- **cyberpanel**
- TBC ...
***
Usage: 
```bash
backallup -p cyberpanel -d example.com
```  
## Troubleshooting
If you encounter any issues with Backallup, please refer to the [troubleshooting guide](https://github.com/SorrentinoPro/backallup/wiki) in the wiki.

## Contributing
Backallup is an open-source project, and we welcome contributions from the community. 
If you'd like to contribute, please fork the repository and submit a pull request.
I would appriciate help adding and testing, more profiles besides **cyberpanel** such as:
- cPanel
- VestaCP
- aaPanel
- CloudPanel
- ISPConfig
- Ajenti
- Froxlor
- Virtualmin
- Zpanel
- HestiaCP
- Ploi
- SPanel
- SpinupWP
- Cloudways
- InterWorx
- OviPanel
- CyberPanel
- Vesta
- Sentora
- Forge
- GridPane
- DirectAdmin
- CentOS Web Panel
- Plesk
- CloudPages
- Hestia Control Panel"
  
Also more databases support besides **MySql** such as:
- postgresql
- mangodb
- More ...
  
Thanks in advance! :neckbeard:

## License
Backallup is licensed under the MIT License.

## Acknowledgments
Backallup was created by Your Name. We'd like to thank the following contributors for their help and support:
- None Yet :(

## Contact
If you have any questions or need help with my script, please don't hesitate to contact me:

- **Email**: [francesco@sorrentino.pro](mailto:francesco@sorrentino.pro)
- **X/Twitter**: [@SorrentinoPro](https://x.com/SorrentinoPro)
