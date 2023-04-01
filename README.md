# CM4-IO-POE-4G PCIEx1 to NVME Adapter

This is an NVME (M-key) adapter board for the PCIEx1 slot.

![PCB renderings](doc/preview_pcb.png)

It is build to fit the [Waveshare CM4G-IO-POE-4G-BOX](https://www.waveshare.com/wiki/Compute_Module_4_PoE_4G_Board#Isolation_GPIO.2FI2C).

![adapter in use](doc/IMG_20230401_140919_resized.jpg)

## Building

The PCB is cost-optimized to be produced by services like JLCPCB.

You have to separate the finger board from the PCB and solder it into its slot.
A standoff and screw for mounting the NVME has to be provided.
It is recomended to fix the board to the CM4 board with standoffs, not rely solely on the PCIEx1 connector to hold everything in place.

The adapter seems to work fine on the CM4 board without fitting the passives (capacitors and LED).

## Revisions

 * 0.8.2 finger board improvements, minor size adjustments

 * 0.8.1 working version, gone into small production run


