# 2:1 CMOS Multiplexer Design & Physical Verification

An end-to-end Custom IC design and physical verification project for a **2:1 Transmission-Gate CMOS Multiplexer** implemented in **45nm GPDK technology** using Cadence Virtuoso.

---

## 📌 Executive Summary
- **Circuit Type:** 2:1 Transmission-Gate CMOS Multiplexer
- **Technology Node:** 45nm GPDK
- **Power Supply ($V_{DD}$):** 1.0 V
- **Verification Status:** 
  - ✅ **DRC:** Passed (0 errors)
  - ✅ **LVS:** Matched (Clean extraction, Empty ERC)

---

## 📑 Full Design Report
You can view or download the complete PDF report here:
👉 **[CMOS_MUX21_45nm_Design_Report.pdf](./CMOS_MUX21_45nm_Design_Report_2.pdf)**


---

## 📊 Key Results & Performance

### 1. DC Analysis Characteristics
| Parameter | Value | Description |
| :--- | :--- | :--- |
| **$V_{OH}$ / $V_{OL}$** | 1.0 V / 0.0 V | Full rail-to-rail swing |
| **$V_{IL}$ / $V_{IH}$** | ~481 mV / ~490 mV | High noise margins |
| **Switching Threshold ($V_M$)** | ~486 mV | Balanced transition region (~0.5V) |

### 2. Transient Response & Power
- **Propagation Delay ($t_{pd\_avg}$):** ~23.03 ps
- **Rise Time ($t_{rise}$):** 1.02 ns | **Fall Time ($t_{fall}$):** 544 ps
- **Dynamic Power:** 1.698 µW
- **Static Power:** 500 pW

---

## 🛠 Flow & Tools Used
1. **Schematic & Symbol Creation:** Cadence Virtuoso Schematic Editor
2. **Simulation:** Cadence Spectre (DC Sweep & Transient Analysis)
3. **Layout & Routing:** Cadence Virtuoso Layout Suite (M1/M2 routing with Guard Rings)
4. **Physical Verification:** Cadence PVS / Pegasus (DRC & LVS debugging)
