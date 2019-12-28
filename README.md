# Plaster Template PS Module
Author: [it-joe](https://github.com/it-joe)

> Custom Plaster template to generate a PowerShell module structure.

## Prerequisites 
### Install Plaster
Install Plaster from the [PowerShell Gallery](https://www.powershellgallery.com/packages/Plaster):

```powershell
PS> Install-Module -Name Plaster
```
### Clone repository
Use Git to clone the template:
```powershell
PS> git clone https://github.com/it-joe/plaster-template-ps-module
```

## Usage
Run `Invoke-Plaster` to create a new PowerShell module structure based on the Plaster template.

#### Workflow:

1. Create GitHub repository
2. Clone repository with `git clone <https://github.com/user/repo>`
3. Create hash table containing all required parameters:
    ```powershell
      PS> $PlasterParameters = @{
          TemplatePath      = "<PathToPlasterTemplate>"
          DestinationPath   = "<PathToNewRepo>"
          AuthorName        = "it-joe"
          AuthorEmail       = "joku@it-joe.de"
          ModuleName        = "ModuleName"
          ModuleDescription = "Brief description on this module."
          ModuleVersion     = "0.1"
          ModuleFolders     = @("Private", "Public")
          GitIgnore         = "Yes"
      }
    ```
4. Call Plaster to generate the PowerShell module structure
    ```powershell
      PS> Invoke-Plaster @PlasterParameters
    ```
6. Push your module to GitHub whenever you are ready.
