# OpenBSD-patches
Just patches for my laptop running OpenBSD current, I would add a new patch everytime I found a problem, but all works out of the box.

## Laptop info 

```sh
OpenBSD 7.4 (GENERIC.MP) #1388: Sun Oct  1 00:22:20 MDT 2023
    deraadt@amd64.openbsd.org:/usr/src/sys/arch/amd64/compile/GENERIC.MP
real mem = 2118729728 (2020MB)
avail mem = 2034827264 (1940MB)
random: good seed from bootblocks
mpath0 at root
scsibus0 at mpath0: 256 targets
mainbus0 at root
bios0 at mainbus0: SMBIOS rev. 2.6 @ 0xe8090 (36 entries)
bios0: vendor Packard Bell version "V3.10(DDR3)" date 11/17/2010
bios0: Packard Bell DOT SE
acpi0 at bios0: ACPI 4.0
acpi0: sleep states S0 S3 S4 S5
acpi0: tables DSDT FACP HPET APIC MCFG SLIC BOOT SSDT WDAT
acpi0: wakeup devices UHC1(S3) UHC2(S3) UHC3(S3) UHC4(S3) ECHI(S3) EXP1(S4) EXP2(S0) EXP3(S4) EXP4(S4) AZAL(S4)
acpitimer0 at acpi0: 3579545 Hz, 24 bits
acpihpet0 at acpi0: 14318179 Hz
acpimadt0 at acpi0 addr 0xfee00000: PC-AT compat
cpu0 at mainbus0: apid 0 (boot processor)
cpu0: Intel(R) Atom(TM) CPU N550 @ 1.50GHz, 1496.29 MHz, 06-1c-0a, patch 00000107
cpu0: FPU,VME,DE,PSE,TSC,MSR,PAE,MCE,CX8,APIC,SEP,MTRR,PGE,MCA,CMOV,PAT,CFLUSH,DS,ACPI,MMX,FXSR,SSE,SSE2,SS,HTT,TM,PBE,SSE3,DTES64,MWAIT,DS-CPL,EST,TM2,SSSE3,CX16,xTPR,PDCM,MOVBE,NXE,LONG,LAHF,PERF,SENSOR,MELTDOWN
cpu0: 24KB 64b/line 6-way D-cache, 32KB 64b/line 8-way I-cache, 512KB 64b/line 8-way L2 cache
cpu0: smt 0, core 0, package 0
mtrr: Pentium Pro MTRR support, 7 var ranges, 88 fixed ranges
cpu0: apic clock running at 166MHz
cpu0: mwait min=64, max=64, C-substates=0.2.2.0.2, IBE
cpu1 at mainbus0: apid 1 (application processor)
cpu1: Intel(R) Atom(TM) CPU N550 @ 1.50GHz, 1496.29 MHz, 06-1c-0a, patch 00000107
cpu1: FPU,VME,DE,PSE,TSC,MSR,PAE,MCE,CX8,APIC,SEP,MTRR,PGE,MCA,CMOV,PAT,CFLUSH,DS,ACPI,MMX,FXSR,SSE,SSE2,SS,HTT,TM,PBE,SSE3,DTES64,MWAIT,DS-CPL,EST,TM2,SSSE3,CX16,xTPR,PDCM,MOVBE,NXE,LONG,LAHF,PERF,SENSOR,MELTDOWN
cpu1: 24KB 64b/line 6-way D-cache, 32KB 64b/line 8-way I-cache, 512KB 64b/line 8-way L2 cache
cpu1: smt 1, core 0, package 0
cpu2 at mainbus0: apid 2 (application processor)
cpu2: Intel(R) Atom(TM) CPU N550 @ 1.50GHz, 997.53 MHz, 06-1c-0a, patch 00000107
cpu2: FPU,VME,DE,PSE,TSC,MSR,PAE,MCE,CX8,APIC,SEP,MTRR,PGE,MCA,CMOV,PAT,CFLUSH,DS,ACPI,MMX,FXSR,SSE,SSE2,SS,HTT,TM,PBE,SSE3,DTES64,MWAIT,DS-CPL,EST,TM2,SSSE3,CX16,xTPR,PDCM,MOVBE,NXE,LONG,LAHF,PERF,SENSOR,MELTDOWN
cpu2: 24KB 64b/line 6-way D-cache, 32KB 64b/line 8-way I-cache, 512KB 64b/line 8-way L2 cache
cpu2: smt 0, core 1, package 0
cpu3 at mainbus0: apid 3 (application processor)
cpu3: Intel(R) Atom(TM) CPU N550 @ 1.50GHz, 997.56 MHz, 06-1c-0a, patch 00000107
cpu3: FPU,VME,DE,PSE,TSC,MSR,PAE,MCE,CX8,APIC,SEP,MTRR,PGE,MCA,CMOV,PAT,CFLUSH,DS,ACPI,MMX,FXSR,SSE,SSE2,SS,HTT,TM,PBE,SSE3,DTES64,MWAIT,DS-CPL,EST,TM2,SSSE3,CX16,xTPR,PDCM,MOVBE,NXE,LONG,LAHF,PERF,SENSOR,MELTDOWN
cpu3: 24KB 64b/line 6-way D-cache, 32KB 64b/line 8-way I-cache, 512KB 64b/line 8-way L2 cache
cpu3: smt 1, core 1, package 0
ioapic0 at mainbus0: apid 4 pa 0xfec00000, version 20, 24 pins, remapped
acpimcfg0 at acpi0
acpimcfg0: addr 0xe0000000, bus 0-255
acpiprt0 at acpi0: bus 0 (PCI0)
acpiprt1 at acpi0: bus 1 (EXP1)
acpiprt2 at acpi0: bus 2 (EXP2)
acpiprt3 at acpi0: bus -1 (EXP3)
acpiprt4 at acpi0: bus -1 (EXP4)
acpiec0 at acpi0
acpibtn0 at acpi0: PWRB
acpibtn1 at acpi0: SLPB
acpibtn2 at acpi0: LID0
acpipci0 at acpi0 PCI0: 0x00000010 0x00000011 0x00000000
acpibat0 at acpi0: BAT0 model "13848633228217409" type Lion oem "SANYO "
acpiac0 at acpi0: AC unit offline
acpicmos0 at acpi0
"SYN1B1C" at acpi0 not configured
"PNP0C14" at acpi0 not configured
"PNP0C0B" at acpi0 not configured
acpicpu0 at acpi0: !C3(100@100 mwait.3@0x30), !C2(500@20 mwait.1@0x10), C1(1000@1 mwait.1), PSS
acpicpu1 at acpi0: !C3(100@100 mwait.3@0x30), !C2(500@20 mwait.1@0x10), C1(1000@1 mwait.1), PSS
acpicpu2 at acpi0: !C3(100@100 mwait.3@0x30), !C2(500@20 mwait.1@0x10), C1(1000@1 mwait.1), PSS
acpicpu3 at acpi0: !C3(100@100 mwait.3@0x30), !C2(500@20 mwait.1@0x10), C1(1000@1 mwait.1), PSS
acpipwrres0 at acpi0: FN00, resource for FAN_
acpitz0 at acpi0: critical temperature is 100 degC
acpivideo0 at acpi0: OVGA
acpivout0 at acpivideo0: DD02
cpu0: Enhanced SpeedStep 1496 MHz: speeds: 1500, 1000 MHz
pci0 at mainbus0 bus 0
pchb0 at pci0 dev 0 function 0 "Intel Pineview DMI" rev 0x02
inteldrm0 at pci0 dev 2 function 0 "Intel Pineview Video" rev 0x02
drm0 at inteldrm0
intagp0 at inteldrm0
agp0 at intagp0: aperture at 0x80000000, size 0x10000000
inteldrm0: apic 4 int 16, PINEVIEW, gen 3
"Intel Pineview Video" rev 0x02 at pci0 dev 2 function 1 not configured
azalia0 at pci0 dev 27 function 0 "Intel 82801GB HD Audio" rev 0x02: msi
azalia0: codecs: Realtek ALC272
audio0 at azalia0
ppb0 at pci0 dev 28 function 0 "Intel 82801GB PCIE" rev 0x02: msi
pci1 at ppb0 bus 1
alc0 at pci1 dev 0 function 0 "Attansic Technology L2C" rev 0xc1: msi, address 1c:75:08:3d:4c:82
atphy0 at alc0 phy 0: F2 10/100 PHY, rev. 4
ppb1 at pci0 dev 28 function 1 "Intel 82801GB PCIE" rev 0x02: msi
pci2 at ppb1 bus 2
athn0 at pci2 dev 0 function 0 "Atheros AR9285" rev 0x01: apic 4 int 17
athn0: AR9285 rev 2 (1T1R), ROM rev 14, address 88:9f:fa:2a:79:1a
uhci0 at pci0 dev 29 function 0 "Intel 82801GB USB" rev 0x02: apic 4 int 18
uhci1 at pci0 dev 29 function 1 "Intel 82801GB USB" rev 0x02: apic 4 int 20
uhci2 at pci0 dev 29 function 2 "Intel 82801GB USB" rev 0x02: apic 4 int 21
uhci3 at pci0 dev 29 function 3 "Intel 82801GB USB" rev 0x02: apic 4 int 22
ehci0 at pci0 dev 29 function 7 "Intel 82801GB USB" rev 0x02: apic 4 int 22
usb0 at ehci0: USB revision 2.0
uhub0 at usb0 configuration 1 interface 0 "Intel EHCI root hub" rev 2.00/1.00 addr 1
ppb2 at pci0 dev 30 function 0 "Intel 82801BAM Hub-to-PCI" rev 0xe2
pci3 at ppb2 bus 5
pcib0 at pci0 dev 31 function 0 "Intel NM10 LPC" rev 0x02
ahci0 at pci0 dev 31 function 2 "Intel 82801GR AHCI" rev 0x02: msi, AHCI 1.1
ahci0: port 0: 3.0Gb/s
ahci0: PHY offline on port 1
scsibus1 at ahci0: 32 targets
sd0 at scsibus1 targ 0 lun 0: <ATA, Hitachi HTS54503, PB3O> naa.5000cca61fe02491
sd0: 305245MB, 512 bytes/sector, 625142448 sectors
ichiic0 at pci0 dev 31 function 3 "Intel 82801GB SMBus" rev 0x02: apic 4 int 17
iic0 at ichiic0
spdmem0 at iic0 addr 0x50: 2GB DDR3 SDRAM PC3-10600 SO-DIMM
usb1 at uhci0: USB revision 1.0
uhub1 at usb1 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
usb2 at uhci1: USB revision 1.0
uhub2 at usb2 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
usb3 at uhci2: USB revision 1.0
uhub3 at usb3 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
usb4 at uhci3: USB revision 1.0
uhub4 at usb4 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
isa0 at pcib0
isadma0 at isa0
pckbc0 at isa0 port 0x60/5 irq 1 irq 12
pckbd0 at pckbc0 (kbd slot)
wskbd0 at pckbd0: console keyboard
pms0 at pckbc0 (aux slot)
wsmouse0 at pms0 mux 0
pms0: Synaptics touchpad, firmware 7.2, 0x1c0b1 0xa40000 0x0 0xd04731 0xa0000
pcppi0 at isa0 port 0x61
spkr0 at pcppi0
uvideo0 at uhub0 port 4 configuration 1 interface 0 "Suyin 1.3M WebCam" rev 2.00/2.15 addr 2
video0 at uvideo0
vscsi0 at root
scsibus2 at vscsi0: 256 targets
softraid0 at root
scsibus3 at softraid0: 256 targets
root on sd0a (48eb47ed3189c57f.a) swap on sd0b dump on sd0b
inteldrm0: 1024x600, 32bpp
wsdisplay0 at inteldrm0 mux 1: console (std, vt100 emulation), using wskbd0
wsdisplay0: screen 1-5 added (std, vt100 emulation)
uhub1 detached
uhub2 detached
uhub3 detached
uhub4 detached
video0 detached
uvideo0 detached
uhub0 detached
uhub0 at usb1 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
uhub1 at usb2 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
uhub2 at usb3 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
uhub3 at usb4 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
uhub4 at usb0 configuration 1 interface 0 "Intel EHCI root hub" rev 2.00/1.00 addr 1
uvideo0 at uhub4 port 4 configuration 1 interface 0 "Suyin 1.3M WebCam" rev 2.00/2.15 addr 2
video0 at uvideo0
inteldrm0: no ifp
drm : i915 raw-wakerefs=1 wakelocks=1 on cleanup
uhub0 detached
uhub1 detached
uhub2 detached
uhub3 detached
video0 detached
uvideo0 detached
uhub4 detached
uhub0 at usb1 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
uhub1 at usb2 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
uhub2 at usb3 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
uhub3 at usb4 configuration 1 interface 0 "Intel UHCI root hub" rev 1.00/1.00 addr 1
uhub4 at usb0 configuration 1 interface 0 "Intel EHCI root hub" rev 2.00/1.00 addr 1
uvideo0 at uhub4 port 4 configuration 1 interface 0 "Suyin 1.3M WebCam" rev 2.00/2.15 addr 2
video0 at uvideo0
inteldrm0: no ifp
syncing disks... done
rebooting...
```
