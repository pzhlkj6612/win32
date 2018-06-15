---
title: IWMPCdrom eject method
description: The eject method ejects the CD or DVD from the drive.
ms.assetid: c0a69252-fd79-452c-bc61-3c3e8bcaaf48
keywords:
- eject method Windows Media Player
- eject method Windows Media Player , IWMPCdrom interface
- IWMPCdrom interface Windows Media Player , eject method
topic_type:
- apiref
api_name:
- IWMPCdrom.eject
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IWMPCdrom::eject method

The **eject** method ejects the CD or DVD from the drive.

## Syntax


```CSharp
public void eject();
```

<span codelanguage="VisualBasic"></span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>VB</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><pre><code>Public Sub eject()
Implements IWMPCdrom.eject</code></pre></td>
</tr>
</tbody>
</table>



## Parameters

This method has no parameters.

## Return value

This method does not return a value.

## Remarks

If the drive door is open, this method closes the door.

To use this method, read access to the library is required. For more information, see [Library Access](library-access.md).

## Examples

The following example uses **eject** to open the door of the CD or DVD drive that has the index of zero in response to the Click event of a button. The **AxWMPLib.AxWindowsMediaPlayer** object is represented by the variable named player.


```CSharp
private void ejectButton_Click(object o, System.EventArgs args)
{
    player.cdromCollection.Item(0).eject();
}
```

<span codelanguage="VisualBasic"></span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>VB</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><pre><code>Public Sub ejectButton_Click(ByVal o As Object, ByVal args As System.EventArgs) Handles ejectButton.Click

    player.cdromCollection.Item(0).eject()

End Sub</code></pre></td>
</tr>
</tbody>
</table>



## Requirements



|                      |                                                                                                                        |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Version<br/>   | Windows Media Player 9 Series or later<br/>                                                                      |
| Namespace<br/> | **WMPLib**<br/>                                                                                                  |
| Assembly<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## See also

<dl> <dt>

[**AxWindowsMediaPlayer.playState (VB and C#)**](axwmplib-axwindowsmediaplayer-playstate--vb-and-c.md)
</dt> <dt>

[**IWMPCdrom Interface (VB and C#)**](iwmpcdrom--vb-and-c.md)
</dt> <dt>

[**IWMPSettings2.mediaAccessRights (VB and C#)**](wmplibiwmpsettings2-iwmpsettings2-mediaaccessrights--vb-and-c.md)
</dt> <dt>

[**IWMPSettings2.requestMediaAccessRights (VB and C#)**](wmplibiwmpsettings2-iwmpsettings2-requestmediaaccessrights--vb-and-c.md)
</dt> </dl>

 

 




