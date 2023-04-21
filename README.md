# Openwrt-21.02-Xiaomi-Mi-Wifi-3C

Untuk menggunakan FW ini harus sudah terpasang uboot breed (breed-mt7688-reset38.bin) <br>
https://github.com/macancrew/Openwrt-21.02-Xiaomi-Mi-Wifi-3C/blob/main/breed-mt7688-reset38.bin <br><br><b>
Cara pasang breed bisa mengikuti tutorial dari ==> https://github.com/hanwckf/rt-n56u/issues/528</b><br><br>
Saya menggunakan windows 7 yang sudah terpasang python 3.7.3<br>
<pre>
you can easily get Telnet-access to the Mi-3C wifi router by this exploit:
https://github.com/acecilia/OpenWRTInvasion
Video: https://www.youtube.com/watch?v=VxzEvdDWU_s

The easiest way to install Padavan on this router is via BREED.
Download link: https://breed.hackpascal.net/breed-mt7688-reset38.bin

Upload it via Filezilla in a Telnet session into the /tmp-folder of the router.

Then start terminal and install BREED:
telnet 192.168.1.1
Telnet user: root
Password: none (just hit enter)
mtd -e Bootloader -r write /tmp/breed-mt7688-reset38.bin Bootloader

In BREED you can easily install the firmware.
</pre>

Jika sukses pasang uboot breed, lanjut update FW dengan link berikut ini <br>
https://github.com/macancrew/Openwrt-21.02-Xiaomi-Mi-Wifi-3C/blob/main/openwrt_21.02.bin <br>
dan hasilnya akan seperti berikut ini <br><br>
<img src=Image1.jpg> <br><br>
ip : 192.168.1.1<br>
user : root <br>
pass : root
