# Core Commands

Set of cmdlets to manage items in datastores exposed by PowerShell providers.

You can use these cmdlets in the same ways to manage all the
different types of data that the providers make available to you.

For example, you can use the `Get-ChildItem` cmdlet to list the files in a
file system directory, the keys under a registry key, or the items that are
exposed by a provider that you write or download.

List of the PowerShell cmdlets that are designed for use with providers:
* ChildItem cmdlets
  - Get-ChildItem
* Content cmdlets
  - Add-Content
  - Clear-Content
  - Get-Content
  - Set-Content
* Item cmdlets
  - Clear-Item
  - Copy-Item
  - Get-Item
  - Invoke-Item
  - Move-Item
  - New-Item
  - Remove-Item
  - Rename-Item
  - Set-Item
* ItemProperty cmdlets
  - Clear-ItemProperty
  - Copy-ItemProperty
  - Get-ItemProperty
  - Move-ItemProperty
  - New-ItemProperty
  - Remove-ItemProperty
  - Rename-ItemProperty
  - Set-ItemProperty
* Location cmdlets
  - Get-Location
  - Pop-Location
  - Push-Location
  - Set-Location
* Path cmdlets
  - Join-Path
  - Convert-Path
  - Split-Path
  - Resolve-Path
  - Test-Path
* PSDrive cmdlets
  - Get-PSDrive
  - New-PSDrive
  - Remove-PSDrive
* PSProvider cmdlets
  - Get-PSProvider


For more information about a cmdlet, type `get-help <cmdlet-name>`

For more information about providers, type `get-help about_providers`

