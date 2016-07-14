---
Description: Retrieving Device Setup Information
MS-HAID: 'audio.retrieving\_device\_setup\_information'
MSHAttr: 'PreferredLib:/library/windows/hardware'
title: Retrieving Device Setup Information
---

# Retrieving Device Setup Information


## <span id="retrieving_device_setup_information"></span><span id="RETRIEVING_DEVICE_SETUP_INFORMATION"></span>


To retrieve setup information from the registry, an adapter driver can call the [**PcGetDeviceProperty**](audio.pcgetdeviceproperty) function, and a miniport driver can call the port driver's [**IPort::GetDeviceProperty**](audio.iport_getdeviceproperty) method.

For either of these calls, the caller selects the type of setup information to request by setting the device-property parameter to one of the following DEVICE\_REGISTRY\_PROPERTY enumeration values from header file Wdm.h:

-   **DevicePropertyAddress**

-   **DevicePropertyBootConfiguration**

-   **DevicePropertyBootConfigurationTranslated**

-   **DevicePropertyBusNumber**

-   **DevicePropertyBusTypeGuid**

-   **DevicePropertyClassGuid**

-   **DevicePropertyClassName**

-   **DevicePropertyCompatibleIDs**

-   **DevicePropertyDetachability**

-   **DevicePropertyDeviceDescription**

-   **DevicePropertyDriverKeyName**

-   **DevicePropertyEnumeratorName**

-   **DevicePropertyFriendlyName**

-   **DevicePropertyHardwareID**

-   **DevicePropertyInstallState**

-   **DevicePropertyLegacyBusType**

-   **DevicePropertyLocationInformation**

-   **DevicePropertyManufacturer**

-   **DevicePropertyPhysicalDeviceObjectName**

-   **DevicePropertyUINumber**

For a description of the DeviceProperty*Xxx* values above, see [**IoGetDeviceProperty**](kernel.iogetdeviceproperty).

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[audio\audio]:%20Retrieving%20Device%20Setup%20Information%20%20RELEASE:%20%287/14/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")


