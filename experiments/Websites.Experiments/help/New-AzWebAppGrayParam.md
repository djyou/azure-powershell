---
external help file: AzureRM.Websites.Experiments-help.xml
online version: 
schema: 2.0.0
---

# New-AzWebAppGrayParam

## SYNOPSIS
Create an Azure Website using Azure App Service. 

## SYNTAX

```
New-AzWebAppGrayParam [[-WebAppName] <String>] [[-ResourceGroupName] <String>] [[-AppServicePlan] <String>]
 [-Auto] [-AddRemote] [[-GitRepositoryPath] <String>] [-WhatIf] [-Confirm] -Location <String>
 [<CommonParameters>]
```

## DESCRIPTION
Create an Azure Website using Azure App Service. This cmdlet uses the 'Gray Parameter' experience, which will prompt the user with default 
values for parameters that are not provided.  Using -Auto indicates that further prompting for defaults should not occur.

## EXAMPLES

### Example 1
```
PS C:\> New-AzWebAppGrayParam -Location "East US"
```

Create a web application with detailed prompts for parameter values that are not provided, including simple defaults.

## PARAMETERS

### -AddRemote
Add a remote github repository to the given github repo.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppServicePlan
The AppService Plan to use for thsi website.  If not provided, the website will create an app service plan, or join an existing free AppService plan.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Plan

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Auto
Skip parameter prompting for remaining parameters.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GitRepositoryPath
The path to a github repository containingg the application for the website.  A remote for pushign to the website will be added to this repository.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Location
{{Fill Location Description}}

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
The name of the resource group to create the website in.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Group

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebAppName
The name of the website.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs. The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

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

### Microsoft.Azure.Management.WebSites.Models.Site
Details about the created website, including its URL.

## NOTES

## RELATED LINKS
