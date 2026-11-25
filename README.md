# Windows Dev Setup

Notes and small fix scripts for getting Node, npm, and Electron projects running on
Windows without fighting the shell every time.

These are the things I hit repeatedly and had to look up more than once, written down
so I stop looking them up.

## Common blockers

### "running scripts is disabled on this system"

PowerShell blocks local scripts by default. For the current session:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
