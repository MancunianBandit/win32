---
Description: Extracts the per-sample principal component analysis (PCA) projection coefficients from an ID3DXPRTCompBuffer compressed data buffer and adds the data to an ID3DXMesh object.
ms.assetid: 0680d626-f07a-43d3-acb9-e8db82b5e933
title: ID3DXPRTCompBuffer::ExtractToMesh method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# ID3DXPRTCompBuffer::ExtractToMesh method

Extracts the per-sample principal component analysis (PCA) projection coefficients from an [**ID3DXPRTCompBuffer**](id3dxprtcompbuffer.md) compressed data buffer and adds the data to an [**ID3DXMesh**](id3dxmesh.md) object.

## Syntax


```C++
HRESULT ExtractToMesh(
  [in] UINT         NumPCA,
  [in] D3DDECLUSAGE Usage,
  [in] UINT         UsageIndexStart,
  [in] LPD3DXMESH   pScene
);
```



## Parameters

<dl> <dt>

*NumPCA* \[in\]
</dt> <dd>

Type: **[**UINT**](https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46)**

Number of PCA coefficients to extract from the buffer.

</dd> <dt>

*Usage* \[in\]
</dt> <dd>

Type: **[**D3DDECLUSAGE**](https://msdn.microsoft.com/VS|directx_sdk|~\d3ddeclusage.htm)**

Vertex usage descriptions of the mesh. See [**D3DDECLUSAGE**](https://msdn.microsoft.com/VS|directx_sdk|~\d3ddeclusage.htm).

</dd> <dt>

*UsageIndexStart* \[in\]
</dt> <dd>

Type: **[**UINT**](https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46)**

Starting index for PCA coefficients to be stored in the mesh.

</dd> <dt>

*pScene* \[in\]
</dt> <dd>

Type: **[**LPD3DXMESH**](id3dxmesh.md)**

Pointer to an [**ID3DXMesh**](id3dxmesh.md) mesh object that will store PCA coefficients.

</dd> </dl>

## Return value

Type: **[**HRESULT**](https://msdn.microsoft.com/windows/desktop/455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

If the method succeeds, the return value is S\_OK. If the method fails, the return value can be one of the following: D3DERR\_INVALIDCALL, E\_OUTOFMEMORY.

## Requirements



|                    |                                                                                        |
|--------------------|----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Mesh.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>   |



## See also

<dl> <dt>

[ID3DXPRTCompBuffer](id3dxprtcompbuffer.md)
</dt> </dl>

 

 



