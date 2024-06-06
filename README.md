# All tools for pentest

## Acunetix 24.4 for Linux

### About

Acunetix v24.4.240514098 by Twilight Shadow


Setup:
1) Download Zip File, password is on our post
2) Before installing the tool, add to your hosts file (usually /etc/hosts) at the end:

127.0.0.1  erp.acunetix.com
127.0.0.1  erp.acunetix.com.
::1  erp.acunetix.com
::1  erp.acunetix.com.

192.178.49.174  telemetry.invicti.com
192.178.49.174  telemetry.invicti.com.
2607:f8b0:402a:80a::200e  telemetry.invicti.com
2607:f8b0:402a:80a::200e  telemetry.invicti.com.

3) Now install the tools with sudo : "sudo bash acunetix_xxxxx.sh"
4) Once installed let's stop its service with: "sudo systemctl stop acunetix"
5) Let's replace wvsc file:
  - sudo cp wvsc /home/acunetix/.acunetix/v_240514098/scanner/wvsc
  - sudo chown acunetix:acunetix /home/acunetix/.acunetix/v_240514098/scanner/wvsc
  - sudo chmod +x /home/acunetix/.acunetix/v_240514098/scanner/wvsc

6) Time to add licenses:
  - sudo rm /home/acunetix/.acunetix/data/license/* (Pay attention to copy and paste right, this can damage your entire OS!!!)
  - sudo cp license_info.json /home/acunetix/.acunetix/data/license/
  - sudo cp wa_data.dat /home/acunetix/.acunetix/data/license/
  - sudo chown acunetix:acunetix /home/acunetix/.acunetix/data/license/license_info.json
  - sudo chown acunetix:acunetix /home/acunetix/.acunetix/data/license/wa_data.dat
  - sudo chmod 444 /home/acunetix/.acunetix/data/license/license_info.json
  - sudo chmod 444 /home/acunetix/.acunetix/data/license/wa_data.dat
  - sudo chattr +i /home/acunetix/.acunetix/data/license/license_info.json (Pay attention to copy and paste right, this can damage your entire  OS!!!)
  - sudo chattr +i /home/acunetix/.acunetix/data/license/wa_data.dat

7) Now let's restart acunetix:
  - sudo systemctl start acunetix

8) Now login back to application, and you should be able to use it :)
9) Enjoy!

### Download

[acunetix_24.4.240514098_x64](https://github.com/0xget/hackerone/releases/tag/acunetix_24.4.240514098_x64)


## Netspot Enterprise Technician Unlimited 3.1.0.478

### About

Netspot Enterprise Technician Unlimited 3.1.0.478
visualize your wifi network
https://www.netspotapp.com/

1. install using NetSpot_3.1.0.478.exe
2. replace files with versions in crack folder

### Download

[Netspot Enterprise Technician Unlimited 3.1.0.478 (windows)](https://github.com/0xget/hackerone/releases/tag/netspot_3.1.0.478_win)
