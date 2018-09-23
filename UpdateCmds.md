# Standard update command for powershell

```powershell
Set-PSRepository -Name PSGallery -Installationpolicy Trusted

$Splat=@{
    Scope = "CurrentUser"
    Name = @(
        "Pester"
        "PowershellGet"
        "PSReadLine"
        "Psake"
    )
    Force = $True
}
Install-module @Splat

```
