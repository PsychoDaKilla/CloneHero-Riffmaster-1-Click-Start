@echo off
sc stop GameInputSvc
ping 127.0.0.1 -n 10 > nul
del C:\WINDOWS\system32\GameInputRedist.dll /s /f /q
ping 127.0.0.1 -n 6 > nul
start "" "C:\Program Files\RB4InstrumentMapper\RB4InstrumentMapper.exe"
ping 127.0.0.1 -n 3 > nul
start "" "C:\Program Files\Clone Hero\Clone Hero.exe"
