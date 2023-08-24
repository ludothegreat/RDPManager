# RDPManager PowerShell Module

The RDPManager.psm1 module provides a set of functions to manage Remote Desktop Protocol (RDP) hosts and connections. The module allows you to add, list, remove, and connect to RDP hosts easily.

## Features

Add-Host: Adds one or more RDP hostnames.
Get-Hosts: Lists all the RDP hostnames with their index numbers.
Remove-Host: Removes a specific RDP host by its index number.
Connect-Host: Connects to an RDP host using its index number.
Show-RDPHelp: Shows a help message with information about available functions.
## Usage

### Add-Host

Adds one or more hosts to the list.

```powershell
Add-Host "host1" "host2"
```
### Get-Hosts
Lists all the hosts with their index numbers.

```powershell
Get-Hosts
```
### Remove-Host
Removes a host by its index number.

```powershell
Remove-Host <index>
```

### Connect-Host
Connects to a host using its index number.

```powershell
Connect-Host <index>
```

### Show-RDPHelp
Displays a help message with information about available functions.

```powershell
Show-RDPHelp
```

## Hosts File
The host information is stored in a file located at `\$env:USERPROFILE\RDPHosts.txt`. The file is automatically created if it does not exist, and the hosts are loaded from the file upon module initialization.
## Installation
You can import this module into your PowerShell session using the following command:

```powershell
Import-Module .\RDPManager.psm1
```

## License
Please refer to the associated license file for details on using and distributing this code.
