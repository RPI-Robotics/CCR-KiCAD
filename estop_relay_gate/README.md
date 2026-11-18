# Emergency Stop Relay Gate PCB

---

A custom board to take in two active low emergency stop signals and shut off relays instantaneously upon the loss of one emergency stop signals. I'm designing it in KiCAD to remove any risk of vehicle vibrations loosening solder connections.



The board mounts with 4 M2 screw holes on the corners. It is powered by 5V from the central power system, and takes in two inputs from the physical and wireless emergency stops. It outputs into two control lines for solid state relays powering 2 ODrive motor controllers.



**Status:** Version 1 Gerber and Drill files created. Ordering very soon (I hope).

## Schematic

---

![schematic.png](C:\Users\qiuj5\Documents\Robotics\IGVC\CCR-KiCAD\estop_relay_gate\docs\schematic.png)

**Rough breakdown:**

- Circuit takes two active low signals as input which are fed into an AND logic gate.

- AND gate controls an nMOS MOSFET which powers two Normally Open solid state relays.

- Upon the loss of one emergency stop signal, solid state relays shut off and indicator LED's switch.



## PCB Layout

---

![pcb.png](C:\Users\qiuj5\Documents\Robotics\IGVC\CCR-KiCAD\estop_relay_gate\docs\pcb.png)

PCB dimensions are 31mm x 56.5mm.

## ToDo List

---

- [x] Design PCB layout.

- [ ] Order board and parts.

- [ ] Assemble and test.

## Credits

---

Original design by James Qiu for RPI Robotics Club, 2026. 