# <%= $PLASTER_PARAM_ModuleName %>
Author: [<%= $PLASTER_PARAM_AuthorName %>](https://github.com/<%= $PLASTER_PARAM_AuthorName %>)

> <%= $PLASTER_PARAM_ModuleDescription %>

## Installing

The easiest way to get <%= $PLASTER_PARAM_ModuleName %> is using the [PowerShell Gallery](https://powershellgallery.com/packages/<%= $PLASTER_PARAM_ModuleName %>/)!

### Inspecting the module

Best practice is that you inspect modules prior to installing them. You can do this by saving the module to a local path:

``` PowerShell
PS> Save-Module -Name <%= $PLASTER_PARAM_ModuleName %> -Path <path>
```

### Installing the module

Once you trust a module, you can install it using:

``` PowerShell
PS> Install-Module -Name <%= $PLASTER_PARAM_ModuleName %>
```

### Updating <%= $PLASTER_PARAM_ModuleName %>

Once installed from the PowerShell Gallery, you can update it using:

``` PowerShell
PS> Update-Module -Name <%= $PLASTER_PARAM_ModuleName %>
```

### Uninstalling <%= $PLASTER_PARAM_ModuleName %>

To uninstall <%= $PLASTER_PARAM_ModuleName %>:

``` PowerShell
PS> Uninstall-Module -Name <%= $PLASTER_PARAM_ModuleName %>
```