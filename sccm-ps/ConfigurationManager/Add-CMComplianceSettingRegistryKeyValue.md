---
external help file: AdminUI.PS.Dcm.dll-Help.xml
online version: 
schema: 2.0.0
---

# Add-CMComplianceSettingRegistryKeyValue

## SYNOPSIS
Adds a compliance setting registry key value

## SYNTAX

### EmptyRule (Default)
```
Add-CMComplianceSettingRegistryKeyValue -DataType <SettingDataType> -Hive <RegistryRootKey> [-Is64Bit]
 -KeyName <String> -ValueName <String> [-Description <String>] -InputObject <PSObject> -Name <String> [-NoRule]
 [-PassThru] [-DisableWildcardHandling] [-ForceWildcardHandling] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ExistentialRule
```
Add-CMComplianceSettingRegistryKeyValue -DataType <SettingDataType> [-Existence <ExistenceType>]
 -Hive <RegistryRootKey> [-Is64Bit] -KeyName <String> -ValueName <String> [-Description <String>]
 [-ExistentialRule] -InputObject <PSObject> -Name <String> [-NoncomplianceSeverity <NoncomplianceSeverity>]
 [-RuleDescription <String>] -RuleName <String> [-PassThru] [-DisableWildcardHandling] [-ForceWildcardHandling]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ValueRule
```
Add-CMComplianceSettingRegistryKeyValue -DataType <SettingDataType> -ExpectedValue <String[]>
 [-ExpressionOperator <RuleExpressionOperator>] -Hive <RegistryRootKey> [-Is64Bit] -KeyName <String>
 [-Remediate] -ValueName <String> [-Description <String>] -InputObject <PSObject> -Name <String>
 [-NoncomplianceSeverity <NoncomplianceSeverity>] [-ReportNoncompliance] [-RuleDescription <String>]
 -RuleName <String> [-ValueRule] [-PassThru] [-DisableWildcardHandling] [-ForceWildcardHandling] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
 

## EXAMPLES

> [!NOTE]
> Configuration Manager CmdLets must be run from the Configuration Manager site drive. For more information, see the [getting started documentation](https://docs.microsoft.com/powershell/sccm/overview).


### Example 1
```
PS XYZ:\>  
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

### -DataType
 

```yaml
Type: SettingDataType
Parameter Sets: (All)
Aliases: 
Accepted values: String, Integer

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
 

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

### -DisableWildcardHandling
DisableWildcardHandling treats wildcard characters as literal character values. Cannot be combined with **ForceWildcardHandling**.

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

### -Existence
 

```yaml
Type: ExistenceType
Parameter Sets: ExistentialRule
Aliases: 
Accepted values: MustExist, MustNotExist

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExistentialRule
 

```yaml
Type: SwitchParameter
Parameter Sets: ExistentialRule
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpectedValue
 

```yaml
Type: String[]
Parameter Sets: ValueRule
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExpressionOperator
 

```yaml
Type: RuleExpressionOperator
Parameter Sets: ValueRule
Aliases: 
Accepted values: IsEquals, NotEquals, BeginsWith, NotBeginsWith, EndsWith, NotEndsWith, Contains, NotContains, OneOf, NoneOf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ForceWildcardHandling
ForceWildcardHandling processes wildcard characters and may lead to unexpected behavior (not recommended). Cannot be combined with **DisableWildcardHandling**.

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

### -Hive
 

```yaml
Type: RegistryRootKey
Parameter Sets: (All)
Aliases: RegistryHive
Accepted values: ClassesRoot, CurrentConfig, CurrentUser, LocalMachine, Users

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
 

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Is64Bit
 

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

### -KeyName
 

```yaml
Type: String
Parameter Sets: (All)
Aliases: RegistryKey

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
 

```yaml
Type: String
Parameter Sets: (All)
Aliases: SettingName

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoRule
 

```yaml
Type: SwitchParameter
Parameter Sets: EmptyRule
Aliases: NoRules

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoncomplianceSeverity
 

```yaml
Type: NoncomplianceSeverity
Parameter Sets: ExistentialRule, ValueRule
Aliases: 
Accepted values: None, Informational, Warning, Critical, CriticalWithEvent

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns an object representing the item with which you are working. By default, this cmdlet may not generate any output.

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

### -Remediate
 

```yaml
Type: SwitchParameter
Parameter Sets: ValueRule
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReportNoncompliance
 

```yaml
Type: SwitchParameter
Parameter Sets: ValueRule
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RuleDescription
 

```yaml
Type: String
Parameter Sets: ExistentialRule, ValueRule
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RuleName
 

```yaml
Type: String
Parameter Sets: ExistentialRule, ValueRule
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ValueName
 

```yaml
Type: String
Parameter Sets: (All)
Aliases: RegistryValueName

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ValueRule
 

```yaml
Type: SwitchParameter
Parameter Sets: ValueRule
Aliases: 

Required: True
Position: Named
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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.Management.Automation.PSObject

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

