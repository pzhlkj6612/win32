---
Description: A callback function used to notify the host of offline analysis progress.
MS-HAID: vspixengine.IOfflineAnalysisCallback\_OfflineAnalysisProgress\_DWORD\_DOUBLE
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: IOfflineAnalysisCallback::OfflineAnalysisProgress method
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# <span id="vspixengine.iofflineanalysiscallback_offlineanalysisprogress_dword_double"></span>IOfflineAnalysisCallback::OfflineAnalysisProgress method

A callback function used to notify the host of offline analysis progress.

## Syntax


```C++
);
```

## Parameters

*cookie*   
A cookie that uniquely identifies the request, and can be used to signal for it to be cancelled.

*progress*   
The progress percentage.

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Requirements

<table><colgroup><col style="width: 50%" /><col style="width: 50%" /></colgroup><tbody><tr class="odd"><td><p>Header</p></td><td>Vspixengine.h</td></tr></tbody></table>

## <span id="see_also"></span>See also

[**IOfflineAnalysisCallback**](https://msdn.microsoft.com/library/windows/desktop/mt432706)

 

 


