---
title: Direct3D Texture Management
description: Direct3D Texture Management
ms.assetid: d67ce56b-ed76-413f-b09f-e25400f1ac6d
keywords: ["texture management WDK Direct3D", "Direct3D WDK Windows 2000 display , texture management", "texture management WDK Direct3D , about texture management"]
---

# Direct3D Texture Management


## <span id="ddk_direct3d_texture_management_gg"></span><span id="DDK_DIRECT3D_TEXTURE_MANAGEMENT_GG"></span>


Although texture support is optional, most of today's drivers are capable of supporting it. Drivers that support texture mapping must respond to all of the texture-related operation codes in the Microsoft Direct3D DDI. For more information about texture-related operation codes, see [**D3DHAL\_DP2OPERATION**](https://msdn.microsoft.com/library/windows/hardware/ff545678).

Drivers must also validate the texture stage states with the [**D3dValidateTextureStageState**](https://msdn.microsoft.com/library/windows/hardware/ff549064) callback.

The following sections describe how drivers implement support for textures:

[Multiple Textures](multiple-textures.md)

[Paletted Textures](paletted-textures.md)

[Texture Blitting](texture-blitting.md)

[Driver-Managed Textures](driver-managed-textures.md)

[Driver-Managed Resources](driver-managed-resources.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[display\display]:%20Direct3D%20Texture%20Management%20%20RELEASE:%20%282/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




