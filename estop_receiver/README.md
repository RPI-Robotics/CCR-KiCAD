# Emergency Stop Receiver

---

A custom board to wirelessly and securely interface with the Emergency Stop remote. Upon interfacing with the remote and confirming connection, the receiver will continuously scan for a heartbeat packet from the remote. If no heartbeat packet is received within 2 seconds, the receiver will trigger the failsafe to trigger the emergency stop. Upon receiving a STOP packet, the same emergency stop will trigger, pulling a high signal down to low within X ms.

This board is split into two different boards made to fabricate together and easily break apart from each other. One board is for LED indicators and the other is the board used to receive and interpret signals. Both are powered by 5V from the central power system.

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