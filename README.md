# dlabs-cmdlets
## CUSTOM CMDLETS by DLabs.

###### this project was developed by dlabs teams. We are using this command for our ALM process. Please use carefully.

Until now we can push this method:

```
Get-DataEntityByFetch
```

**Microsoft.Xrm.Data.PowerShell**

This site was built using [GitHub Pages](https://github.com/seanmcne/Microsoft.Xrm.Data.PowerShell)

**Microsoft.Xrm.Tooling.CrmConnector.Powershell**

This module comes from Dynamics CRM SDK and it exposes two functions, Get-CrmOrganizations and Get-CrmConnection. See the link for more detail. [Use PowerShell cmdlets for XRM tooling to connect to CRM](https://technet.microsoft.com/en-us/library/dn689040.aspx)

**How the cmdlet dlabs connect to msdyncrm**

CmdLets Dlabs module exposes many functions, you can use Connect-CrmOnlineDiscovery or Connect-CrmOnPremDiscovery to connect to any CRM organization by using Discovery Service. 

We use a $conn global variable. Any other functions which needs to connect to the CRM Organization takes connection parameter. 

**Example**

```powershell
# Online
Connect-CrmOnlineDiscovery -InteractiveMode
# OnPrem
Connect-CrmOnPremDiscovery -InteractiveMode
```

