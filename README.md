# CM4-IO-POE-4G PCIEx1 to NVME Adapter

This is an NVME (M-key) adapter board for the PCIEx1 slot.

Its PCB is designed with a break-away section for the fingered connector. This is then soldered in a matching slot of the PCB to form a 90 degree connector.

## Revisions

 * 0.9.0 added oscillator for 32.768kHz SUSClk signal

 * 0.8.2 finger board improvements, minor size adjustments

 * 0.8.1 working version, gone into small production run

## Description

PCB of the 0.8.2 version without SUSClk
![PCB renderings](doc/preview_pcb.png)

![PCB renderings](doc/preview_sch.png)

It is designed to fit the [Waveshare CM4G-IO-POE-4G-BOX](https://www.waveshare.com/wiki/Compute_Module_4_PoE_4G_Board#Isolation_GPIO.2FI2C).

![adapter in use](doc/IMG_20230401_140919_resized.jpg)

## Building

The PCB is cost-optimized to be produced by services like JLCPCB.

You have to separate the finger board from the PCB and solder it into its slot.
Make sure the finger board is at right angles to the main PCB when soldering.

An NVME M-key connector, a standoff, and screw for mounting the NVME has to be provided.
It is recommended to fix the board to the CM4 board with standoffs, not rely solely on the PCIEx1 connector to hold everything in place. For doing this, there are two holes matching holes in the baseboard PCB.

The adapter seems to work fine on the CM4 board without fitting the passives (capacitors and LED).

Remember that your kernel needs PCIe support. There is a convenient [docker cross-compile environment by Jeff Geerling](https://github.com/geerlingguy/raspberry-pi-pcie-devices/tree/master/extras/cross-compile).

## Improvement ideas

 * choose gold fingers for production (I went as cheap as possible with HASL)

 * get out of the way for the CAM0 FPC cable


