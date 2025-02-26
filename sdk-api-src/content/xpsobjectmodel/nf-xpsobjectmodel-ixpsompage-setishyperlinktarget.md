---
UID: NF:xpsobjectmodel.IXpsOMPage.SetIsHyperlinkTarget
title: IXpsOMPage::SetIsHyperlinkTarget (xpsobjectmodel.h)
description: Specifies whether the page is the target of a hyperlink.
old-location: xps\ixpsompage_setishyperlinktarget.htm
tech.root: printdocs
ms.assetid: a8096303-5940-4ad1-aa5a-de604efe8c9e
ms.date: 12/05/2018
ms.keywords: IXpsOMPage interface [XPS Documents and Packaging],SetIsHyperlinkTarget method, IXpsOMPage.SetIsHyperlinkTarget, IXpsOMPage::SetIsHyperlinkTarget, SetIsHyperlinkTarget, SetIsHyperlinkTarget method [XPS Documents and Packaging], SetIsHyperlinkTarget method [XPS Documents and Packaging],IXpsOMPage interface, xps.ixpsompage_setishyperlinktarget, xpsobjectmodel/IXpsOMPage::SetIsHyperlinkTarget
f1_keywords:
- xpsobjectmodel/IXpsOMPage.SetIsHyperlinkTarget
dev_langs:
- c++
req.header: xpsobjectmodel.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: XpsObjectModel.idl
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
- COM
api_location:
- xpsobjectmodel.h
api_name:
- IXpsOMPage.SetIsHyperlinkTarget
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IXpsOMPage::SetIsHyperlinkTarget


## -description


Specifies whether the page is the target of a hyperlink.


## -parameters




### -param isHyperlinkTarget [in]

The Boolean value that indicates whether the page is the target of a hyperlink.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt>TRUE</dt>
</dl>
</td>
<td width="60%">
The page is the target of a hyperlink.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>FALSE</dt>
</dl>
</td>
<td width="60%">
The page is not the target of a hyperlink.

</td>
</tr>
</table>
 


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the table that follows. For information about  XPS document API return values that are not listed in this table, see <a href="https://docs.microsoft.com/previous-versions/windows/desktop/dd372955(v=vs.85)">XPS Document Errors</a>.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>XPS_E_MISSING_NAME</b></dt>
</dl>
</td>
<td width="60%">
The page has not been named. The hyperlink target status can only be set if the page has a name.

</td>
</tr>
</table>
 




## -remarks



Only those pages that have this property set to <b>TRUE</b> will be included in the hyperlink targets that are collected by <a href="https://docs.microsoft.com/windows/desktop/api/xpsobjectmodel/nf-xpsobjectmodel-ixpsompagereference-collectlinktargets">IXpsOMPageReference::CollectLinkTargets</a>.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/xpsobjectmodel/nn-xpsobjectmodel-ixpsompage">IXpsOMPage</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/dd372955(v=vs.85)">XPS Document Errors</a>
 

 

