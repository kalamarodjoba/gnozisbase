7z

avast
настроить

everything

naps2
настроить принтер

sordum.org
отлючить автообновление

chrome

remove cortana
winaero
https://winaero.com/download-uninstall-cortana-for-windows-10/





-----------------------

chrome

переименовать man13

+ ublock origin

запрет на установку расщирений

-----------------------








--------------------------------------------------------------

wmic useraccount where name='user' rename person


wmic useraccount list full 

SID=S-1-5-21-3620556808-2144516947-308136571-1001


wmic computersystem where caption='current_pc_name' rename new_pc_name
or
wmic computersystem where name="%COMPUTERNAME%" call rename name="PCMAN13"

# know hostname (computer name)
hostname

cd C:\Users
rename OldUserFolder NewUserFolder


HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\ProfileList

ProfileImagePath




-----------------


DRIVERS MFP

main site
https://support.hp.com/ua-ru/drivers/selfservice/samsung-proxpress-sl-m3870-laser-multifunction-printer-series/16463018/model/16463022

printer
https://ftp.hp.com/pub/softlib/software13/printers/SS/SL-M3370FD/SamsungUniversalPrintDriver3.exe

scan
https://ftp.hp.com/pub/softlib/software13/printers/SS/SL-M3370FD/UniversalScanDriver_V1.02.19.exe




----------------





### для SSD

1.

TRIM
https://remontka.pro/enable-trim-ssd-windows/


2.
установить пароль для акаунта

добавить ярлики на общие папки. создать расшарить директорию "я"

pagefile.sys
swapfile.sys

powershell

New-ItemProperty -Path “HKLM:\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management” -Name SwapfileControl -Value 0 -PropertyType DWORD -Force

---

Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management]
"SwapfileControl"=dword:00000000

---


disable pagefile.sys

powercfg -h off


windows search
sc stop “wsearch” && sc config “wsearch” start=disabled

superfetch
sc stop "SysMain" && sc config "SysMain" start=disabled


---

Отключите автоматическую дефрагментацию дисков
dfrgui



