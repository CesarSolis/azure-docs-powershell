---
external help file: Microsoft.Azure.Commands.IotHub.dll-Help.xml
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/IotHub/Commands.IotHub/help/Get-AzureRmIotHubValidSku.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/IotHub/Commands.IotHub/help/Get-AzureRmIotHubValidSku.md
gitcommit: https://github.com/Azure/azure-powershell/blob/04e47f8329ba9e64790c974f9666dbf41de7483f
---

# Get-AzureRmIotHubValidSku

## SYNOPSIS
Gets all valid skus that this IotHub can transition to.

## SYNTAX

```
Get-AzureRmIotHubValidSku [-ResourceGroupName] <String> [-Name] <String> [<CommonParameters>]
```

## DESCRIPTION
Gets all the valid skus that this IotHub can transition to.
An IotHub cannot transition between free and the paid skus and vice versa. 
You will have to delete and recreate the iothub if you want to achieve this.

## EXAMPLES

### Example 1 Get the valid skus
```
PS C:\> Get-AzureRmIotHubValidSku -ResourceGroupName "myresourcegroup" -Name "myiothub"
```

Gets a list of all skus for the IotHub named "myiothub"

## PARAMETERS

### -Name
Name of the IoT hub. 

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Resource Group Name

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### System.Collections.Generic.IList`1[[Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubSkuDescription, Microsoft.Azure.Commands.IotHub, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null]]

## NOTES

## RELATED LINKS

