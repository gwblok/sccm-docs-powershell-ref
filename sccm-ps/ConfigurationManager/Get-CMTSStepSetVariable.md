---
description: Gets a TS step set variable.
external help file: AdminUI.PS.Osd-help.xml
Module Name: ConfigurationManager
ms.date: 05/02/2019
schema: 2.0.0
title: Get-CMTSStepSetVariable
---

# Get-CMTSStepSetVariable

## SYNOPSIS
Gets a TS step set variable.

## SYNTAX

### ByValue (Default)
```
Get-CMTSStepSetVariable [-InputObject] <IResultObject> [-StepName <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### ById
```
Get-CMTSStepSetVariable [-TaskSequenceId] <String> [-StepName <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### ByName
```
Get-CMTSStepSetVariable [-TaskSequenceName] <String> [-StepName <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION

> [!NOTE]
> Configuration Manager cmdlets must be run from the Configuration Manager site drive.
> The examples in this article use the site name **XYZ**. For more information, see the
> [getting started](/powershell/sccm/overview) documentation.

## EXAMPLES

### Example 1
``` POwerShell
PS XYZ:\>$TSName = "Task Sequence Name"
PS XYZ:\>$TSSetVarStepName = "New TS Var - Hello"
PS XYZ:\>Get-CMTSStepSetVariable -TaskSequenceName $TSName -StepName $TSSetVarStepName
```
``` Output
PS PS2:\> Get-CMTSStepSetVariable -TaskSequenceName $TSName -StepName $TSSetVarStepName


SmsProviderObjectPath  : SMS_TaskSequence_SetVariableAction
Condition              : 
ContinueOnError        : False
Description            : Testing Vars via PowerShell
DoNotShowVariableValue : False
Enabled                : True
HiddenVariableValue    : 	
                         
Name                   : New TS Var - Hello
SupportedEnvironment   : WinPEandFullOS
Timeout                : 
VariableName           : Hello
VariableValue          : TRUE
```

## PARAMETERS

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

### -InputObject
```yaml
Type: IResultObject
Parameter Sets: ByValue
Aliases: TaskSequence

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -StepName
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

### -TaskSequenceId
```yaml
Type: String
Parameter Sets: ById
Aliases: Id, TaskSequencePackageId

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TaskSequenceName
```yaml
Type: String
Parameter Sets: ByName
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.ConfigurationManagement.ManagementProvider.IResultObject

## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
