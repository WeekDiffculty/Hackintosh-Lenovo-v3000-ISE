

# Hackintosh-Lenovo-v3000-ISE
    
This repository is for hackintosh on Lenovo v3000.


Change log：12/16/2018

•Update Clover 4796,now use full hotpatch (battery、IRQ、DeviceModify), off course, static DSDT patches is optional.
 Use SMCBatteryManager.kext instead of ACPIBatteryManager.kext.

Change log：11/12/2018

•Update Clover 4746 and use static acpi rename patch(RenameDevices seem to be wrong), fix battery patch(EC0->EC) and upload binpatch.sh for static acpi rename (DSDT.aml SSDT-2-CB-01.aml).

Change log：11/1/2018

•Update EFI, Clover 4717, CX20751_2 audio layout-id ingect via Device Properties, acpi rename patches via RenameDevices, all kext has been update to the newest.

Change log：10/18/2018

•Update EFI to 10.14+,Clover 4706, only use WhateverGreen.kext,all kext has been update to the newest, and other changes.

Change log：5/20/2018

•Update Clover 4480 、new ACPI files (BIOS version:B0CNA0WW)、remove hotpatch of ULAC replace by custom USBInjectAll.kext、drop CPU related tables by length.

Change log：4/22/2018

•Update Clover 4444 and AppleALC 1.2.6,SSDT-ALL.dsl has updated also.Now the battery hotpatch is coming,but not add to the SSDT-ALL as for it's stability.

Change log：4/14/2018

•Merge 2048M Graphics memory and 32M minStolenSize to one patch,now no need IntelGraphicsDVMTFixup.kext.

•Note : this patch just for after install, so it's batter to disable it within install.

Change log：4/02/2018

•Update Clover 4423 and upload full EFI flie,update SSDT-ALL.dsl.

Change log：3/19/2018

•Update New batery patch,only use RECB/WECB method.
 
Change log：3/05/2018

•Update B0D3->HDAU patch.

Change log：2/22/2018

•Add SSDT-ASL0 to the SSDT-ALL.dsl to store the brightless level after reboot.

Change log：2/13/2018

•I have done this SSDT-ALL.aml，now all DSDT patches can be replaced by this except battery patch，I'm not going to add a battery patch to SSDT-ALL at the moment.

•This SSDT-ALL.aml can fix Audio、HD5500 Graphics、USB has injected properly、Brightness、XCPM mode、OS check.

•Note:I still use the RMCF to control these hotpatches,because it will be convenient for me to debug. 
It is best to use it after the installation is completed.
