# MacOS-Monterey-i7-11700k-MSI-z590-Gaming-Carbon
Hackintosh EFI and development for an i7-11700k, MSI z590 Gaming Carbon WiFi:

Specs:
* i7-11700k
* MSI z590 Gaming Carbon WiFi
* Nitro Sapphire RX Vega 56 (Flashed to Vega 64)
* Crucial 500gb SSD SATA
* FENVI T919 WIFI / BT Card
* 32gb Ram (Generic)

Working:
* Everything but onboard WiFi and onboard Ethernet (I have a Fenvi Card so no interest in trying intel wifi but am curious if it works!)
* The USB 3.2 ports, for me, do not support drives or "data" based connections.... rather peripherals like mice, webcams, and keyboards seem to work fine. Note I must connec the USB to Ethernet adapter to a USB 2.0 port for it to work for me.
* I use audio out from a 3.5mm jack on back and this works great.

Not working:
* ETHERNET on motherboard.... the Intel I225V 2.5Gbps LAN controller is too "new" for Apple and is not supported. I did try patching it like suggested here: [Guide](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#add-2) yet none of the options presented worked for me personally so I did a work around with a USB to ethernet adapter that uses a Realtek8111 based chipset. This is the one that works for me: [Uni USB 3.0 to Ethernet Adapter](https://www.amazon.com/uni-Ethernet-Internet-Compatible-Notebook/dp/B087QFQW6F/ref=sr_1_8?keywords=usb+3.0+to+ethernet&qid=1636773294&sr=8-8)
* Regarding performance - I usually get 400 MBPS through the wall and with the kext and the adpater I get ~ 180 MBPS on Monterey (400 on Windows like expected) but I don't really notice a performance deficit. 


To Be Done:
* USB Map, just been busy
* Test USB C port
* Tinker more with I225V patch

