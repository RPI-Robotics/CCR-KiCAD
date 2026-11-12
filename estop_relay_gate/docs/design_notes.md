### Errata Log 11/11/2026: Logic-Level MOSFET Vgs

* **Issue:** Initial BOM selection specified a standard power MOSFET whose rated $R_{DS(on)}$ required a $10\text{V}$ gate-to-source drive, while the control trace only outputs $5\text{V}$ logic.
* **Impact:** Driving the gate at $5\text{V}$ would prevent full MOSFET activation, significantly increasing resistance and causing excessive thermal dissipation during continuous load switching.
* **Resolution:** Replaced the component during pre-fabrication design review with a logic-level MOSFET fully characterized at $V_{GS} = 4.5\text{V}$, ensuring low conduction loss and safe thermal margins.
