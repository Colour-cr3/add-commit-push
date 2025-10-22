### Git Automation Script

This project includes a Python script (`add-commit-push.py`) that automates Git operations.

#### Aliases

**Windows PowerShell**

1. Create a PowerShell profile file (if necessary):
```powershell
New-Item -Path $PROFILE -ItemType File -Force
```
3. Open PowerShell profile file:
```powershell
notepad $PROFILE
```
3. Add these lines to the .ps1 file:
```powershell
Set-Alias (something to represent your project directory) "cd C:\path\to\your\project"
Set-Alias acp "python C:\path\to\your\project\add-commit-push.py"
```
Now you can do:
```powershell
(something to represent your project directory)
acp -m "Updated code"
```
**MacOS Terminal**

1. Open your shell config file:
```bash
nano ~/.zshrc   # or ~/.bashrc
```
2. Add:
```bash
alias (something to represent your project directory)='cd ~/path/to/your/project'
alias acp='python3 ~/path/to/your/project/add-commit-push.py'
```
3. Save and reload:
```bash
source ~/.zshrc
```
Now you can do:
```bash
(something to represent your project directory)
acp -m "Updated code" -f
```
Credits:

By: Patrick O'Connor

Credits: ChatGPT for code and Eric Pogue for the idea and requirements
