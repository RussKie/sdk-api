---
UID: NS:wsdxmldom._WSDXML_NAMESPACE
title: WSDXML_NAMESPACE (wsdxmldom.h)
description: Specifies an XML namespace.
old-location: ncd\wsdxml_namespace_struct.htm
tech.root: WsdApi
ms.assetid: dcf27f38-e628-4b0c-859c-ad12d3ed0924
ms.date: 12/05/2018
ms.keywords: WSDXML_NAMESPACE, WSDXML_NAMESPACE structure, _WSDXML_NAMESPACE, ncd.wsdxml_namespace_struct, wsdxmldom/WSDXML_NAMESPACE
f1_keywords:
- wsdxmldom/WSDXML_NAMESPACE
dev_langs:
- c++
req.header: wsdxmldom.h
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
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- HeaderDef
api_location:
- WsdXmldom.h
api_name:
- WSDXML_NAMESPACE
targetos: Windows
req.typenames: WSDXML_NAMESPACE
req.redist: 
ms.custom: 19H1
---

# WSDXML_NAMESPACE structure


## -description


Specifies an XML namespace.


## -struct-fields




### -field Uri

The URI that identifies the namespace.


### -field PreferredPrefix

The preferred prefix to be used in XML prefix mappings.


### -field Names

Reference to an array of <a href="https://docs.microsoft.com/windows/desktop/api/wsdxmldom/ns-wsdxmldom-wsdxml_name">WSDXML_NAME</a> structures that specify the names in the namespace.


### -field NamesCount

The number of names in the <b>Names</b> array.


### -field Encoding

The encoded reference for the namespace.


## -remarks



<b>WSDXML_NAMESPACE</b> represents the association between a namespace URI and a list of names belonging to that namespace. Additionally, it provides a <b>PreferredPrefix</b> for the namespace, which gives guidance on the default prefix to use for a specified namespace. In the context of WSDAPI, there are two types of namespaces: static namespaces and dynamic namespaces.

Static namespaces are user provided, well known, and assumed to be complete namespaces, in that all names belonging to the namespace should be in names array. When processing a received XML document, any element or attribute in the document that claims to be in a static namespace but has a name not listed in that namespace is treated as an error. Static namespaces are typically generated pre-compile time, by a tool like WSDCodeGen.

Dynamic namespaces are generated by WSDAPI. These are built when new namespaces are seen in XML documents. With dynamic namespaces, no assumptions can be made about whether a specified name actually belongs to the formal namespace or not, so all names are accepted as being part of the namespace. As such, dynamic namespaces expand the <b>Names</b> array as they process new names in a specified document.



