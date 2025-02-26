---
UID: NF:netfw.INetFwRule.get_InterfaceTypes
title: INetFwRule::get_InterfaceTypes (netfw.h)
description: Specifies the list of interface types for which the rule applies.
old-location: ics\inetfwrule_interfacetypes.htm
tech.root: ics
ms.assetid: 2548875c-3c23-4076-9d3d-82bebf5e7718
ms.date: 12/05/2018
ms.keywords: INetFwRule interface [ICS/ICF],InterfaceTypes property, INetFwRule.InterfaceTypes, INetFwRule.get_InterfaceTypes, INetFwRule::InterfaceTypes, INetFwRule::get_InterfaceTypes, INetFwRule::put_InterfaceTypes, InterfaceTypes property [ICS/ICF], InterfaceTypes property [ICS/ICF],INetFwRule interface, get_InterfaceTypes, ics.inetfwrule_interfacetypes, netfw/INetFwRule::InterfaceTypes, netfw/INetFwRule::get_InterfaceTypes, netfw/INetFwRule::put_InterfaceTypes
f1_keywords:
- netfw/INetFwRule.InterfaceTypes
dev_langs:
- c++
req.header: netfw.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: FirewallAPI.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- FirewallAPI.dll
api_name:
- INetFwRule.InterfaceTypes
- INetFwRule.get_InterfaceTypes
- INetFwRule.put_InterfaceTypes
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# INetFwRule::get_InterfaceTypes


## -description


Specifies the list of interface types for which the rule applies.

This property is read/write.


## -parameters


## -remarks



This property is optional.

Also see the restrictions on changing properties described in the Remarks section of the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/netfw/nn-netfw-inetfwrule">INetFwRule</a> interface page.

Acceptable values for this property are "RemoteAccess", "Wireless", "Lan", and "All". If more than one interface type is specified, the strings must be separated by a comma.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/netfw/nn-netfw-inetfwrule">INetFwRule</a>
 

 

