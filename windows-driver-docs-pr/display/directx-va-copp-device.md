---
title: DirectX VA COPP Device
description: DirectX VA COPP Device
ms.assetid: f9268b38-3317-4c4f-b9c1-e0ad3c88f92e
keywords: ["COPP device WDK DirectX VA", "copy protection WDK COPP , COPP device", "video copy protection WDK COPP , COPP device", "COPP WDK DirectX VA , COPP device", "protected video WDK COPP , COPP device"]
---

# DirectX VA COPP Device


## <span id="ddk_directx_va_copp_device_gg"></span><span id="DDK_DIRECTX_VA_COPP_DEVICE_GG"></span>


This section applies only to Windows Server 2003 SP1 and later, and Windows XP SP2 and later.

The display driver should be implemented so that a DirectX VA COPP device is created for each video session. The COPP device represents an end point to receive COPP commands and status requests. The COPP device also stores the protection settings of its associated physical connector. A physical connector can support multiple content protection types. For example, an S-Video connector can support analog content protection (ACP) in addition to Content Generation Management System for Analog (CGMS-A) protection. For more information, see [Defining the COPP Device Class](defining-the-copp-device-class.md).

Multiple instances of the COPP device are required so that different processes can configure the settings of the graphics adapter's output through COPP. Therefore, you should implement the COPP device class so that each COPP device acts appropriately when multiple video sessions are active on the system.

**Note**   A video session consists of a video stream possibly combined with one or more video substreams. A video session is tied to a particular graphics adapter's output connector. Several video sessions can be active on a system and within a single process.

 

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[display\display]:%20DirectX%20VA%20COPP%20Device%20%20RELEASE:%20%282/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




