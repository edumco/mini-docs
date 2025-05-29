## Teams Issues

Teams is a [super-app](https://en.wikipedia.org/wiki/Super-app) with multiple plugins and sub-apps that can cause some troubles from time to time.

Here are some tips to fix and to prevent a lot of small troubles and performance botlenecks.

### Cache cleaning

#### Basic Cleaning PowerShell Script


```powershel
# Closes Microsoft Teams process
taskkill /IM teams.exe /F /T

# Defines the policy for this script.
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process

# Removes specific safe to remove cache files from 3 locations

Get-ChildItem -Path ([System.Environment]::ExpandEnvironmentVariables("%AppData%\Microsoft\Teams")) -Directory `
| Where-Object { $_.Name -in ('blob_storage', 'Cache', 'Application Cache', 'Code Cache', 'databases', 'GPUCache', 'IndexedDB', '') } `
| ForEach-Object { Remove-Item $_.FullName -Recurse -Force };

Get-ChildItem -Path ([System.Environment]::ExpandEnvironmentVariables("%AppData%\Microsoft\Teams\meeting-addin")) -Directory `
| Where-Object { $_.Name -in ('Cache', '') } `
| ForEach-Object { Remove-Item $_.FullName -Recurse -Force };

Get-ChildItem -Path ([System.Environment]::ExpandEnvironmentVariables("%AppData%\Microsoft\Teams\Service Worker")) -Directory `
| Where-Object { $_.Name -in ('CacheStorage', 'ScriptCache', '') } `
| ForEach-Object { Remove-Item $_.FullName -Recurse -Force };

```

### Full Teams cleaning

```powershel
# Closes Microsoft Teams process
taskkill /IM teams.exe /F /T

# Defines the policy for this script.
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process


Get-ChildItem -Path ([System.Environment]::ExpandEnvironmentVariables("%appdata%")) -Directory `
| Where-Object { $_.Name -in ('Teams', '') } `
| ForEach-Object { Remove-Item $_.FullName -Recurse -Force };

Get-ChildItem -Path ([System.Environment]::ExpandEnvironmentVariables("%Programdata%")) -Directory `
| Where-Object { $_.Name -in ('Teams', 'SquirrelMachineInstalls', '') } `
| ForEach-Object { Remove-Item $_.FullName -Recurse -Force };

```

- C:\Users\<username>\AppData\Local\Microsoft
- C:\Users\<username>\AppData\Roaming\Microsoft
- C:\Users\<username>\AppData\Roaming

### Full app reinstall

## 

reboot system



## References

- [appuals.com/completely-uninstall-microsoft-teams-on-windows-10/](https://appuals.com/completely-uninstall-microsoft-teams-on-windows-10/)
- [neroblanco.co.uk/uninstall-microsoft-teams-cleanly/](https://neroblanco.co.uk/2020/01/uninstall-microsoft-teams-cleanly/)
- [adamtheautomator.com/uninstall-microsoft-teams/](https://adamtheautomator.com/uninstall-microsoft-teams/)
