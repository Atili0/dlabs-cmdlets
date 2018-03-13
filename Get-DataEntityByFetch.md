# Get-DataEntityByFetch

**PARAMETERS**
Parameter used for this function

- Entity
    > Alias : e
    > Mandatory : true
- Path
    > Alias : p
    > Mandatory : false
- Fetch
    > Alias : f
    > Mandatory : true
- Uncompressed
    > Alias : unc
    > Mandatory : false
- Encrypt
    > Alias : enc
    > Mandatory : false
- KeyWord
    > Alias : k
    > Mandatory : false
    > ValidateLength : admit 16-20

**EXAMPLE**

```xml
$fetch = "<fetch top='50' >" +
  "<entity name='account'>" +
    "<attribute name='name'/>" +
    "<attribute name='accountnumber'/>"+
  "</entity>" +
"</fetch>";


Get-DataEntityByFetch -c $conn -e account -k "dlabs.mscrm.2018" -f $fetch

```
