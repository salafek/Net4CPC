# Net4CPC
Net4CPC is an Ethernet interface for the [Amstrad CPC](https://www.cpcwiki.eu/index.php/CPC) range of computers.</br></br>
![Net4CPC PCB](https://github.com/salafek/Net4CPC/blob/main/pictures/Net4CPC-pcb.png)
## Notes
The interface has a [Mother X4](https://cpcrulez.fr/hardware-interface-mother_x4.htm) compatible connector.</br> 
The network module is based on the [WIZnet's W5100S](https://www.wiznet.io/product-item/w5100s/) embedded ethernet controller and works in indirect parallel bus mode.</br>
In this mode it needs 4 I/O ports:
- #FD20: MR - Common Register MR
- #FD21: IDM_ARH - Upper 8 bits Offset Address Register
- #FD22: IDM_ARL - Lower 8 bits Offset Address Register
- #FD23: IDM_DR - 8 Bits Data Register

The PCB has provision for 2 differrent types of Ethernet modules:
- A chineese [W5100S module](https://www.aliexpress.com/w/wholesale-%22W5100S-Network-Module%22-parallel.html?catId=0&initiative_id=SB_20230206005326&SearchText=%22W5100S%20Network%20Module%22%20parallel&spm=a2g0o.productlist.1000002.0) with an integrated 3.3V regulator.</br> ![W5100S module](https://github.com/salafek/cyboard-for-cpc/blob/main/pictures/w5100s-module.png)
- The original WIZnet's [W5100S](https://github.com/Wiznet/Hardware-Files-of-WIZnet/tree/master/05_Network_Module/WIZ810SMJ) or [W6100](https://github.com/Wiznet/Hardware-Files-of-WIZnet/tree/master/05_Network_Module/WIZ610MJ) modules.</br> <img src="https://github.com/Wiznet/Hardware-Files-of-WIZnet/blob/master/05_Network_Module/WIZ810SMJ/Pictures/WIZ810SMJ_1.png" width="300" height="230"><img src="https://github.com/Wiznet/Hardware-Files-of-WIZnet/blob/master/05_Network_Module/WIZ610MJ/Pictures/WIZ610MJ1.png" width="400" height="300">
## Build info
The schematic and layout were generated with Autodesk EAGLE 9.6.2 free edition</br>
