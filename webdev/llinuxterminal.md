# Linux Terminal

## File and Directory Operations

* List files and directories: `ls`
* Change directory: `cd [directory]`
* Create a directory: `mkdir [directory]`
* Remove an empty directory: `rmdir [directory]`
* Remove a directory and its contents: `rm -r [directory]`
* Create a file: `touch [file]`
* Display file contents: `cat [file]`
* Copy a file or directory: `cp [source] [destination]`
* Move a file or directory: `mv [source] [destination]`
* Remove a file: `rm [file]`
* Create a symbolic link: `ln -s [target] [link]`

## System Information

* Display system information: `inxi -F`
* Display disk usage: `df -h`
* Display memory usage: `free -h`
* List running processes: `ps aux`
* List all PCI devices: `lspci`
* List all USB devices: `lsusb`

## Package Management (APT)

* Update package list: `sudo apt update`
* Upgrade installed packages: `sudo apt upgrade`
* Install a package: `sudo apt install [package]`
* Remove a package: `sudo apt remove [package]`
* Search for a package: `apt search [package]`
* Display package information: `apt show [package]`
* List installed packages: `apt list --installed`

## File Permissions

* Change file ownership: `sudo chown [user]:[group] [file/directory]`
* Change file permissions: `sudo chmod [permissions] [file/directory]`
  * Example (read, write, execute for owner): `chmod 700 [file/directory]`

## Networking

* Display network interfaces: `ip addr`
* Display network connections: `ss -tuln`
* Ping a host: `ping [host]`
* Perform a DNS lookup: `dig [domain]`
* Download a file: `wget [URL]`

## Text Manipulation

* Find text in files: `grep [pattern] [file]`
* Sort lines of text: `sort [file]`
* Count words, lines, or characters: `wc [options] [file]`

## Miscellaneous

* Clear the terminal: `clear`
* Display command history: `history`
* Run a command as another user (e.g., root): `sudo [command]`
* Shutdown the system: `sudo shutdown -h now`
* Reboot the system: `sudo reboot`
