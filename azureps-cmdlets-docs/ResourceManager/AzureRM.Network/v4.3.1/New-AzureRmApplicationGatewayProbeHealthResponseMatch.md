---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/New-AzureRmApplicationGatewayProbeHealthResponseMatch.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/New-AzureRmApplicationGatewayProbeHealthResponseMatch.md
gitcommit: https://github.com/Azure/azure-powershell/blob/ae060e9ea34c37f2cde2b7c1e2aacff632b227c2
---

# New-AzureRmApplicationGatewayProbeHealthResponseMatch

## SYNOPSIS
Creates a health probe response match used by Health Probe for an application gateway.

## SYNTAX

```
New-AzureRmApplicationGatewayProbeHealthResponseMatch [-Body <String>]
 [-StatusCode <System.Collections.Generic.List`1[System.String]>] [<CommonParameters>]
```

## DESCRIPTION
**The Add-AzureRmApplicationGatewayProbeHealthResponseMatch** cmdlet creates a health probe response match used by Health Probe for an application gateway.

## EXAMPLES

### Example 1
```
PS C:\>$responsematch = New-AzureRmApplicationGatewayProbeHealthResponseMatch -Body "helloworld" -StatusCode "200-399","503"
```

This command creates a health response match which can be passed to ProbeConfig as a parameter.

## PARAMETERS

### -Body
Body that must be contained in the health response.
Default value is empty

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StatusCode
Allowed ranges of healthy status codes.Default range of healthy status codes is 200 - 399

```yaml
Type: System.Collections.Generic.List`1[System.String]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayProbeHealthResponseMatch

## NOTES

## RELATED LINKS

