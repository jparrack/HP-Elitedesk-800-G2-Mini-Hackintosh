# HP-Elitedesk-800-G2-Mini-Hackintosh
Welcome to my git repository for my HP Elitedesk 800 G2 Mini hackintosh. I've posted on [reddit.com/](https://www.reddit.com/r/hackintosh/comments/vavsua/hp_elitedesk_800_g2_mini_wip_on_monterey/) and recieved a bunch of questions regarding how I got mine to work.

## Hackintosh Specs
My model is the 35W version of the 800 G2 Mini.
* CPU: Intel Core i5-6500T (35w TDP)
* GPU: Intel HD Graphics 530
* RAM: 8GB (2133Mhz DDR4)
* Ethernet Card: Intel Mausi
* BIOS revision: Latest version (v02.56)

## BIOS Setup
I recommend you visit the HP website and install the latest version of the BIOS. The settings I used are;
* TPM Embedded Security - Set to hidden
* Intel Software Guard Extension (SGX) - Disabled

* In boot options - USB Storage boot is enabled but PXE, Fast and CD-ROM boot are disabled. It's down to you and your drives for the boot order.
* Secure boot configuration - Set to Legacy Support Enable and Secure Boot Disable
* System Options - Turbo-boost, Multi-processor, VT (VTx), M.2 SSD and Allow PCIe/PCI SERR# Interrupt are left enabled.
* Built in device options - Embedded LAN controller, audio device and internal speakers are enabled. Increase video memory size to 512mb.
* Port options - enable them all
* Optional ROM policy - All legacy
* Power management options - enable all apart from unqiue sleep state blink rates
* Remote managaement options - disable all options here.

## Modifications made
* I disabled some of OpenCore's security for the bootloader to work correctly.
