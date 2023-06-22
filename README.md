# ROG Ally Notes
Just various notes on setting up my ROG Ally, stuff to remember myself if I ever need to reinstall

## Windows 11 Tweaks

Changes to make Windows 11 perform better, use less ressources or be less annoying.

### Turn off Memory Integrity
From: [support.microsoft.com](https://support.microsoft.com/en-us/windows/options-to-optimize-gaming-performance-in-windows-11-a255f612-2949-4373-a566-ff6f3f474613)

- From start, search "Core Isolation"
- Under "Memory Integrity" turn Off


### Turn off Virtual Machine Platform
From [support.microsoft.com](https://support.microsoft.com/en-us/windows/options-to-optimize-gaming-performance-in-windows-11-a255f612-2949-4373-a566-ff6f3f474613)

- From start, search "Windows Features"
- Deselect "Virtual Machine Platform" and press OK


### Uninstall "bloatware"

- Simply uninstall all unnecessary pre-installed applications


### Enable Battery Care Mode

For my use case, it's going to be on charger most of the time, so makes sense to limit charging to 80%

- In MyAsus
- Under Customization > Power & Performance
- Enable "Battery Care Mode"


### Uninstall / Disable Widgets

To get rid of Widgets, even running in background, we can forcefully uninstall it

- Open a PowerShell terminal in Administrator mode
- Run 
  ```powershell
  Get-AppxPackage *WebExperience* | Remove-AppxPackage
  ```


### Disable Windows Search Indexing

No need to index files on a gaming handheld, only used for gaming

- Open "Services"
- Locate "Windows Search"
- Stop and set "Startup type" to "Disabled"