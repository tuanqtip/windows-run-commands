
# Useful Windows Run Commands

This document lists a variety of useful Run commands in Windows for quickly accessing system utilities and settings.

## Frequently Used Commands

| Command         | Description                               |
|-----------------|-------------------------------------------|
| `sysdm.cpl`     | Opens System Properties (System settings) |
| `appwiz.cpl`    | Opens Programs and Features (Add/Remove Programs) |
| `firewall.cpl`  | Opens Windows Firewall settings           |

## Other Useful Commands

| Command             | Description                                       |
|---------------------|---------------------------------------------------|
| `control`           | Opens Control Panel                               |
| `inetcpl.cpl`       | Opens Internet Properties                         |
| `ncpa.cpl`          | Opens Network Connections                         |
| `main.cpl`          | Opens Mouse Properties                            |
| `mmsys.cpl`         | Opens Sound Properties                            |
| `desk.cpl`          | Opens Display Properties                          |
| `timedate.cpl`      | Opens Date and Time settings                      |
| `hdwwiz.cpl`        | Opens Add Hardware Wizard                         |
| `powercfg.cpl`      | Opens Power Options                               |
| `msinfo32`          | Opens System Information                          |
| `taskmgr`           | Opens Task Manager                                |
| `devmgmt.msc`       | Opens Device Manager                              |
| `services.msc`      | Opens Services Manager                            |
| `compmgmt.msc`      | Opens Computer Management                         |
| `gpedit.msc`        | Opens Group Policy Editor (Windows Pro/Enterprise)|
| `secpol.msc`        | Opens Local Security Policy (Windows Pro/Enterprise)|
| `regedit`           | Opens Registry Editor                             |
| `perfmon.msc`       | Opens Performance Monitor                         |
| `eventvwr.msc`      | Opens Event Viewer                                |
| `fsmgmt.msc`        | Opens Shared Folders                              |
| `lusrmgr.msc`       | Opens Local Users and Groups                      |
| `dxdiag`            | Opens DirectX Diagnostic Tool                     |
| `cmd`               | Opens Command Prompt                              |
| `notepad`           | Opens Notepad                                     |
| `calc`              | Opens Calculator                                  |
| `mstsc`             | Opens Remote Desktop Connection                   |
| `cleanmgr`          | Opens Disk Cleanup Utility                        |
| `msconfig`          | Opens System Configuration                        |

These commands can be entered into the Run dialog (Win + R) for quick access to the listed utilities.

## Remove activate windows watermash
Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\svsvc -> Start (4) -> Reset

## kiem tra may tinh:
Disk: Get-PhysicalDisk | Format-List * > C:\temp\PhysicalDiskInfo.txt
RAM: Get-CimInstance -ClassName Win32_PhysicalMemory | Format-List *
CPU: Get-CimInstance -ClassName Win32_Processor | Format-List *
Motherboard: Get-CimInstance -ClassName Win32_BaseBoard | Format-List *
GPU: Get-CimInstance -ClassName Win32_VideoController | Format-List *
Network Adapter: Get-CimInstance -ClassName Win32_NetworkAdapter | Where-Object { $_.PhysicalAdapter -eq $true } | Format-List *
Pin: Get-CimInstance -ClassName Win32_Battery | Format-List *
Storage Controller (Bộ điều khiển lưu trữ): Get-CimInstance -ClassName Win32_SCSIController | Format-List *
BIOS: Get-CimInstance -ClassName Win32_BIOS | Format-List *



