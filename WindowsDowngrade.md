DOWNGRADE WINDOWS SERVER (DATACENTER TO STANDARD)

Exibir OS name e OS version


`systeminfo | findstr /B /C:"OS Name" /B /C:"OS Version"`
![Screenshot 2024-03-07 at 17 12 51](https://github.com/IgaoWolf/Comands-Windows/assets/81160709/fcbc85c9-92a9-4abf-ae8a-d7f7a937142c)


`Get-ComputerInfo | select WindowsProductName, WindowsVersion, OsHardwareAbstractionLayer`
![Screenshot 2024-03-07 at 17 13 35](https://github.com/IgaoWolf/Comands-Windows/assets/81160709/4610c559-176a-4509-9349-f4dd287117ff)

Abra o regedit e edite os seguintes componentes - 

HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion
![Screenshot 2024-03-07 at 17 15 48](https://github.com/IgaoWolf/Comands-Windows/assets/81160709/5cbaabf5-ba3c-435e-879e-19a03c1d51ac)

EditionID and CompositionEditionID to ServerStandard, ProductName to Windows Server 2022 Standard
Montar a iso do Windows 2022, marque para não efetuar (updates,drives) e Marque a Imagem Windows Server 2022 Standard (Desktop Experience) 

