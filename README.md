# OrbitronDDE2RigCtl
This app take satellite frequency from `Orbitron` and send it to `RigCtl` server. In my case this is SDR++.
Mainly used for polar orbiting satellites.

# Installation.
- unpack `OrbitronDDE2RigCtl.zip` where you want. As example `e:\SDR`
- open file `c:\Users\{You profile name}\AppData\Local\VirtualStore\Program Files (x86)\Orbitron\Config\Setup.cfg` or `c:\Program Files (x86)\Orbitron\Config\Setup.cfg` for rare Windows.
- paste this text to begin of file. Change the path to the one where you unzipped the archive.
````
[Drivers]
RigCtl=e:\SDR\OrbitronDDE2RigCtl\DDE2RigCtl.exe
````
save `Setup.cfg`, launch `Orbitron`, go to `Rotor/Radio` tab, select in `Driver` list `RigCtl`

![Orbitron_wUM9xB0biH](https://github.com/user-attachments/assets/8a55d11e-7e51-4e4f-b42b-fa99e103ddd1)


- click the button to the right of the list. Application will start. Default server is `localhost` and port `4532`.
  
![Orbitron_wMciyIQib9](https://github.com/user-attachments/assets/691cecae-72e5-4473-8837-ae6a2a30163e)

- in SDR++ install plugin `Rigctl server`
- Thats all. Now every several seconds active frequency in SDR++ will be changed to downlink of satellite selected in Obitron. With doppler correction.






  Grok asked to mention him in the description :)
