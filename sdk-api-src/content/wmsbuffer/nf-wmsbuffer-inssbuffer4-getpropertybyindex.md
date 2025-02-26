---
UID: NF:wmsbuffer.INSSBuffer4.GetPropertyByIndex
title: INSSBuffer4::GetPropertyByIndex (wmsbuffer.h)
description: The GetPropertyByIndex method retrieves a buffer property, also called a data unit extension, that was set using INSSBuffer3::SetProperty.
old-location: wmformat\inssbuffer4_getpropertybyindex.htm
tech.root: wmformat
ms.assetid: 8812b7c9-610b-4c17-a274-55e043cfb091
ms.date: 12/05/2018
ms.keywords: GetPropertyByIndex, GetPropertyByIndex method [windows Media Format], GetPropertyByIndex method [windows Media Format],INSSBuffer4 interface, INSSBuffer4 interface [windows Media Format],GetPropertyByIndex method, INSSBuffer4.GetPropertyByIndex, INSSBuffer4::GetPropertyByIndex, INSSBuffer4GetPropertyByIndex, wmformat.inssbuffer4_getpropertybyindex, wmsbuffer/INSSBuffer4::GetPropertyByIndex
ms.topic: method
f1_keywords:
- wmsbuffer/INSSBuffer4.GetPropertyByIndex
dev_langs:
- c++
req.header: wmsbuffer.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 9 Series SDK, or later versions of the SDK
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wmvcore.lib; WMStubDRM.lib (if you use DRM)
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Wmvcore.lib
- Wmvcore.dll
- WMStubDRM.lib
- WMStubDRM.dll
api_name:
- INSSBuffer4.GetPropertyByIndex
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# INSSBuffer4::GetPropertyByIndex


## -description



The <b>GetPropertyByIndex</b> method retrieves a buffer property, also called a data unit extension, that was set using <a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nf-wmsbuffer-inssbuffer3-setproperty">INSSBuffer3::SetProperty</a>. This method differs from <a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nf-wmsbuffer-inssbuffer3-getproperty">INSSBuffer3::GetProperty</a> in that, instead of accessing the property by name, it uses an index ranging from zero to one less than the total number of properties associated with the sample.




## -parameters




### -param dwBufferPropertyIndex [in]

<b>DWORD</b> containing the buffer property index. This value will be between zero and one less than the total number of properties associated with the sample. You can retrieve the total number of properties by calling <a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nf-wmsbuffer-inssbuffer4-getpropertycount">INSSBuffer4::GetPropertyCount</a>.


### -param pguidBufferProperty [out]

Pointer to a GUID specifying the type of buffer property.


### -param pvBufferProperty [out]

Void pointer containing the value of the buffer property.


### -param pdwBufferPropertySize [in, out]

Pointer to a <b>DWORD</b> containing the size of the value pointed to by <i>pvBufferProperty</i>. If you set <i>pvBufferProperty</i> to <b>NULL</b>, this value will be set to the required size in bytes of the buffer needed to store the property value.


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an <b>HRESULT</b> error code.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nn-wmsbuffer-inssbuffer4">INSSBuffer4 Interface</a>
 

 

