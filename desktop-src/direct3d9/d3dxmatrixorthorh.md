---
Description: Builds a right-handed orthographic projection matrix.
ms.assetid: 6b9b50d5-0307-4fc7-a28d-8f42d2a21bf0
title: D3DXMatrixOrthoRH function
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# D3DXMatrixOrthoRH function

Builds a right-handed orthographic projection matrix.

## Syntax


```C++
D3DXMATRIX* D3DXMatrixOrthoRH(
  _Inout_ D3DXMATRIX *pOut,
  _In_    FLOAT      w,
  _In_    FLOAT      h,
  _In_    FLOAT      zn,
  _In_    FLOAT      zf
);
```



## Parameters

<dl> <dt>

*pOut* \[in, out\]
</dt> <dd>

Type: **[**D3DXMATRIX**](d3dxmatrix.md)\***

Pointer to the resulting [**D3DXMATRIX**](https://msdn.microsoft.com/en-us/library/Bb204929(v=VS.85).aspx).

</dd> <dt>

*w* \[in\]
</dt> <dd>

Type: **[**FLOAT**](https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx)**

Width of the view volume.

</dd> <dt>

*h* \[in\]
</dt> <dd>

Type: **[**FLOAT**](https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx)**

Height of the view volume.

</dd> <dt>

*zn* \[in\]
</dt> <dd>

Type: **[**FLOAT**](https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx)**

Minimum z-value of the view volume.

</dd> <dt>

*zf* \[in\]
</dt> <dd>

Type: **[**FLOAT**](https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx)**

Maximum z-value of the view volume.

</dd> </dl>

## Return value

Type: **[**D3DXMATRIX**](d3dxmatrix.md)\***

Pointer to the resulting [**D3DXMATRIX**](https://msdn.microsoft.com/en-us/library/Bb204929(v=VS.85).aspx).

## Remarks

All the parameters of the **D3DXMatrixOrthoRH** function are distances in camera space. The parameters describe the dimensions of the view volume.

The return value for this function is the same value returned in the *pOut* parameter. In this way, the **D3DXMatrixOrthoRH** function can be used as a parameter for another function.

This function uses the following formula to compute the returned matrix.


```
2/w  0    0           0
0    2/h  0           0
0    0    1/(zn-zf)   0
0    0    zn/(zn-zf)  1
```



## Requirements



|                    |                                                                                        |
|--------------------|----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3dx9math.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>   |



## See also

<dl> <dt>

[Math Functions](dx9-graphics-reference-d3dx-functions-math.md)
</dt> <dt>

[**D3DXMatrixOrthoLH**](d3dxmatrixortholh.md)
</dt> <dt>

[**D3DXMatrixOrthoOffCenterRH**](d3dxmatrixorthooffcenterrh.md)
</dt> <dt>

[**D3DXMatrixOrthoOffCenterLH**](d3dxmatrixorthooffcenterlh.md)
</dt> </dl>

 

 



