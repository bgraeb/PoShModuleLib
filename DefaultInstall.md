# Simple installer scripts

(only because I can't remember things)

```powershell
if($PSVersionTable.Platform -ne "Unix"){
    Install-Module "Chocolatey" -Force -Scope "CurrentUser"
    Install-ChocolateySoftware
    Install-ChocolateyPackage git,vscode
}
```
