# ⚠️ WARNING: Use Linux or WSL for MLOps Projects

## ❌ Avoid Running on Native Windows

This project is intended to be used in a **Linux** environment or with **WSL (Windows Subsystem for Linux)**.

Running directly on native Windows may result in:
- Path issues with tools like `DVC`, `Docker`, and `Git`
- Broken symlinks or Git tracking errors
- Missing dependencies or installation problems
- Inconsistent behavior across shells (e.g., PowerShell vs Bash)
- Poor compatibility with Python ML/DL libraries
- Problems with file permissions and case-sensitive filesystems

## ✅ Recommended Setup

- **Preferred OS**: Ubuntu 22.04+ / Any stable Linux distro
- **Windows Users**: Install [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install) and use Ubuntu inside it
- **Shell**: Use Bash or Zsh (not CMD or PowerShell)
- **VS Code**: Use the Remote - WSL extension for editing inside WSL

## 🛠️ Setup Commands (WSL Example)

```bash
sudo apt update && sudo apt install -y python3 python3-pip git dvc
