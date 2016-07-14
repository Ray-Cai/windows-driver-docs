---
Description: Installing Core System Components for an Audio Adapter
MS-HAID: 'audio.installing\_core\_system\_components\_for\_an\_audio\_adapter'
MSHAttr: 'PreferredLib:/library/windows/hardware'
title: Installing Core System Components for an Audio Adapter
---

# Installing Core System Components for an Audio Adapter


## <span id="installing_core_system_components_for_an_audio_adapter"></span><span id="INSTALLING_CORE_SYSTEM_COMPONENTS_FOR_AN_AUDIO_ADAPTER"></span>


This section includes the following topics about installing the core system components for a port-class audio adapter:

[Installing in Windows 2000 and Later](installing-in-windows-2000-and-later.md)

The [**INF DDInstall section**](devinst.inf_ddinstall_section) for each hardware ID specified in the manufacture's **MODEL** section should specify the inclusion of the **KS.Registration** section in Ks.inf and the **WDMAUDIO.Registration** section in Wdmaudio.inf. The Ks.inf file installs the core kernel streaming components. The Wdmaudio.inf file installs the core WDM audio components. Vendors should not modify or replace these system INF files.

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[audio\audio]:%20Installing%20Core%20System%20Components%20for%20an%20Audio%20Adapter%20%20RELEASE:%20%287/14/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")


