https://uploaddeimagens.com.br/imagens/captura_de_tela-png-12892b3e-6550-43d2-8f51-28190485b2fc

Dell Inspiron 5447  Bios A12

Intel Core i7 4510U @2.00GHZ

Intel HD4400

8GB DDR3L 1600MHZ

SSD 256GB Micron

MacOS Mojave 10.14.5 (18F132)

Hardware Specs:

Suportado:

Audio: Realtek  ALC255                        | Ok Via applealc + codecCommander + HDAVerb

Microfone Interno                             | Ok Via applealc + codecCommander + HDAVerb

Video: Intel HD4400                           | Ok Via patch FakePCIID + platform-id

HDMI:                                         | Ok Video e audio

Backlight:                                    | Ok Via kext

Wifi & bluetooth: Artheros AR9565             | Ok Substituído a placa original por Broadcom bcm94352z (NGFF DELL DW 1560)

Rede cabeada: Realtek RTL 8100                | Ok Via kext

TouchScreen                                   | Ok rodando nativo

Teclado e Touchpad                            | Ok funcionando via voodoops2controller

Portas notebook USB 3.0                       | Ok rodando nativo

Não suportado:

Placa Video:Radeon r7 M265     

SD card reader:RTS5179  
                                        


DSDT + SSDT Extraida do Clover e corrigida, patch ACPI 6.2a
Patch usados na DSDT:
Shutdown Fix v2
Haswell LPC
Rename GFX0 to IGPU
Fix_WAK Arg0 v2
Rename B0D3 to HDAU
System_IRQ : usado para ativar alc255

SSDTs Sistema:
SSDT1
SSDT2
SSDT3
SSDT4
SSDT5

SSDTs Extra usadas:
SSDT-DMAC
SSDT-PMCR
SSDT-PNLF

Patch backlight no tutorial Backlight fix.rtf

EDID tela copiar pasta inteira  “DisplayProductID-5f1” em : /System/Library/Displays/Contents/Resources/Overrides

Patch audio na DSDT  com arquivo system_IRQ.txt + cover layout id 28
HDAVerb ativa o CodecCommander para o audio: HDAVerb: /usr/bin
AudioScript : arquivo para corrigir audio dos headphones com chiado e deve ser iniciado com o sistema


Kexts usados

Clover: EFI/CLOVER/kexts/Other

ACPIBatteryManager.kext

AppleALC.kext

CodecCommander.kext

FakePCIID_Intel_HD_Graphics.kext

FakePCIID_Intel_HDMI_Audio.kext

FakePCIID.kext

FakePCIID_XHCIMux.kext

FakeSMC_ACPISensors.kext

FakeSMC_CPUSensors.kext

FakeSMC_GPUSensors.kext

FakeSMC_LPCSensors.kext

FakeSMC_SMMSensors.kext

FakeSMC.kext

Lilu.kext

RealtekRTL8100.kext

VoodooPS2Controller.kext

WhateverGreen.kext

/System/Library/Extensions

BrcmFirmwareRepo.kext

BrcmPatchRAM2.kext

FakeSMC.kext

/Library/Extensions

AppleBacklightFixup

FakePCIID_Broadcom_WiFi

FakePCIID

/usr/bin

hda-verb
