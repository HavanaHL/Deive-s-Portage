# ⚙️ Portage Configuration

[![Gentoo](https://img.shields.io/badge/Gentoo-54487A?style=for-the-badge&logo=gentoo&logoColor=white)](https://www.gentoo.org/)
[![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)](https://git-scm.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

My personal `/etc/portage` configuration for Gentoo Linux. Because why not version control the thing that controls everything? 

## 📋 System Specs

This configuration is tailored for a humble but honest setup:

- **CPU**: Intel Celeron N2840 (dual-core, but it tries its best)
- **GPU**: Intel HD Graphics BYT (integrated)
- **RAM**: 8 GB
- **Storage**: 500 GB HDD 
- **WM**: Wayfire

> ⚠️ **Note**: Compilation times may vary. Chromium builds measured in geological epochs.

## 🎯 What's Inside

- `make.conf` - The heart of the operation
- `package.use/` - USE flags, because we choose our bloat carefully
- `package.accept_keywords/` - Living on the edge (responsibly)
- `package.mask/` - Things we don't talk about
- `env/` - Custom build environments, Clang and LTO 🗣️

## 🛠️ Installation

**DON'T** just blindly copy this to your system. Seriously.

```bash
# Backup your current config first
sudo cp -r /etc/portage /etc/portage.backup

# Clone this repo
git clone https://github.com/HavanaHL/Deive-s-Portage.git ~/deive-portage

# Review the configs
cd ~/deive-portage
less make.conf

# Copy what makes sense for YOUR system
# sudo cp -r * /etc/portage/
