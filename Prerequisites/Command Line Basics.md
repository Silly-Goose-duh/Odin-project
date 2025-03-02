# Introduction to the Command Line

## What is a Command Line?
The **command line** is an interface where users can type commands to interact with the computer’s operating system. It provides more control and flexibility compared to graphical interfaces.

## Opening the Command Line
- **Windows**: Open the Command Prompt (`cmd`) or PowerShell.
- **macOS/Linux**: Open the Terminal.

## Basic Commands

### 1. Navigating the Filesystem
- `pwd` - Print the current working directory.
- `ls` - List files and directories in the current location.
- `cd <directory>` - Change directory.
  - Example: `cd Documents`
- `cd ..` - Move up one directory level.

### 2. File and Directory Operations
- `mkdir <directory_name>` - Create a new directory.
- `touch <file_name>` - Create an empty file (Linux/macOS).
- `echo "text" > file.txt` - Create a file and write text to it.
- `cat <file_name>` - Display file contents.
- `rm <file_name>` - Remove a file.
- `rm -r <directory_name>` - Remove a directory and its contents.

### 3. File Permissions
- `chmod` - Change file permissions.
  - Example: `chmod +x script.sh` (make executable)
- `chown` - Change file ownership.
  - Example: `chown user:group file.txt`

### 4. Process Management
- `ps` - List running processes.
- `kill <PID>` - Terminate a process.
- `top` / `htop` - Display system resource usage.

### 5. Networking
- `ping <domain>` - Check connectivity to a website or server.
- `curl <url>` - Fetch data from a URL.

### 6. Package Management
- **Linux (Debian-based)**:  
  - `apt-get install <package>` - Install a package.
  - `apt-get update` - Update package lists.
- **macOS**:  
  - `brew install <package>` (using Homebrew).
- **Windows**:  
  - `winget install <package>` (using Windows Package Manager).

## Conclusion
Mastering the command line can greatly enhance your productivity, allowing for faster navigation, automation, and system control. Keep practicing these commands to build confidence!

