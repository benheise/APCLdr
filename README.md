
<h2 align="center">
APCLdr: Payload Loader With Evasion Features
</h2>



### Features:
- no crt functions imported
- indirect syscalls using [HellHall](https://github.com/Maldev-Academy/HellHall)
- api hashing using [CRC32](https://github.com/NUL0x4C/APCLdr/blob/main/APCLdr/Win32.c#L111) hashing algorithm
- payload encryption using rc4 - payload is saved in .rsrc
- Payload injection using APC calls - alertable thread
- Payload execution using APC - alertable thread
- Execution delation using [MsgWaitForMultipleObjects](https://github.com/NUL0x4C/APCLdr/blob/main/APCLdr/APCLdr.c#L66) - edit [this](https://github.com/NUL0x4C/APCLdr/blob/main/APCLdr/Common.h#L6)

<br>

### Usage:
Use [Builder](https://github.com/NUL0x4C/APCLdr/tree/main/Builder) to update the [PayloadFile.pf](https://github.com/NUL0x4C/APCLdr/blob/main/APCLdr/PayloadFile.pf) file, that'll be the encrypted payload to be saved in the .rsrc section of the loader


<br>

### Thanks For:
- https://www.x86matthew.com/view_post?id=writeprocessmemory_apc
- https://github.com/vxunderground/VX-API

<br>


<h4 align="center">
Tested with cobalt strike && Havoc on windows 10
</h4>


