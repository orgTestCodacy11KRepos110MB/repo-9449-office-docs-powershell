---
external help file: Microsoft.Rtc.Management.Hosted.dll-help.xml 
online version: https://learn.microsoft.com/powershell/module/skype/get-cstenantdialplan
applicable: Skype for Business Online
title: Get-CsTenantDialPlan
schema: 2.0.0
manager: bulenteg
author: tomkau
ms.author: tomkau
ms.reviewer:
---

# Get-CsTenantDialPlan

## SYNOPSIS
Use the Get-CsTenantDialPlan cmdlet to retrieve a tenant dial plan.

## SYNTAX

### Identity (Default)
```
Get-CsTenantDialPlan [-Tenant <Guid>] [[-Identity] <XdsIdentity>] [-LocalStore] [<CommonParameters>]
```

### Filter
```
Get-CsTenantDialPlan [-Tenant <Guid>] [-Filter <String>] [-LocalStore] [<CommonParameters>]
```

## DESCRIPTION
The Get-CsTenantDialPlan cmdlet returns information about one or more tenant dial plans (also known as a location profiles) in an organization.
Tenant dial plans provide required information to let Enterprise Voice users make telephone calls.
The Conferencing Attendant application also uses tenant dial plans for dial-in conferencing.
A tenant dial plan determines such things as which normalization rules are applied, and whether a prefix must be dialed for external calls.

You can use the Get-CsTenantDialPlan cmdlet to retrieve specific information about the normalization rules of a tenant dial plan.

## EXAMPLES

### -------------------------- Example 1 --------------------------
```
Get-CsTenantDialPlan
```

This example retrieves all existing tenant dial plans.



### -------------------------- Example 2 --------------------------
```
Get-CsTenantDialPlan -Identity Vt1TenantDialPlan2
```

This example retrieves the tenant dial plan that has an identity of Vt1TenantDialplan2.


## PARAMETERS

### -Filter
The Filter parameter allows you to limit the number of results based on filters you specify.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
The Identity parameter is a unique identifier that designates the name of the tenant dial plan to retrieve.

```yaml
Type: XdsIdentity
Parameter Sets: (All)
Aliases: 
Applicable: Skype for Business Online

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LocalStore
PARAMVALUE: SwitchParameter

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tenant
Specifies the globally unique identifier (GUID) of your Skype for Business Online tenant account.
For example: -Tenant "38aad667-af54-4397-aaa7-e94c79ec2308".
You can find your tenant ID by running this command: Get-CsTenant | Select-Object DisplayName, TenantID

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 
Applicable: Skype for Business Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (https://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
