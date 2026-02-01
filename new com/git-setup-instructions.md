# Git Installation and Setup Instructions

## Install Git on Windows

### Method 1: Download from Official Website
1. Go to https://git-scm.com/download/windows
2. Download the latest version
3. Run the installer with default settings
4. Restart your command prompt/PowerShell

### Method 2: Using Winget (if available)
```powershell
winget install --id Git.Git -e --source winget
```

### Method 3: Using Chocolatey (if installed)
```powershell
choco install git
```

## After Installing Git

1. Open a new PowerShell/Command Prompt
2. Configure Git with your information:
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

3. Navigate to your project folder and run:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/your-repo-name.git
git push -u origin main
```

## Quick Commands for Future Updates

After making changes to your website:
```bash
git add .
git commit -m "Updated schedule or made changes"
git push
```

Your website will automatically update on GitHub Pages!