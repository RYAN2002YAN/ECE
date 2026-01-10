# Module 1 – Lesson 4: Temperature Sensors and Applications  
## 模块1 第4课：温度传感器及其应用


## 🎯 Four Major Types of Thermal Sensors / 四类主要热传感器

| Sensor Type       | Principle | Range | Pros | Cons | Common Applications |
|-------------------|----------|-------|------|------|---------------------|
| **Thermocouple**<br>（热电偶） | Voltage from junction of two dissimilar metals<br>两种不同金属接点产生电压 | Up to **1800°C** | - Wide range<br>- Rugged | - Nonlinear<br>- Drifts over time → needs yearly calibration<br>- Low output voltage | Metal/semiconductor fabrication |
| **RTD**<br>（电阻温度检测器） | Metal resistance ↑ with temperature<br>金属电阻随温度升高而增加（铂最常用） | Up to **800°C** | - Highly accurate & linear<br>- Stable long-term<br>- No annual recalibration | - Requires precision current source<br>- Needs 3- or 4-wire circuit to cancel lead resistance | Pharma, biotech (audit-critical processes) |
| **Thermistor**<br>（热敏电阻） | Semiconductor: resistance ↓ sharply with temp (NTC)<br>半导体：温度↑ → 电阻↓（NTC型） | Up to **200°C** | - High sensitivity<br>- Small size → ideal for phones/computers<br>- Low cost | - Highly nonlinear → needs complex firmware (e.g., Steinhart-Hart) | Consumer electronics, embedded systems |
| **Infrared (IR)**<br>（红外传感器） | Measures emitted IR energy from surface<br>通过物体发射的红外能量测温 | Very high (non-contact) | - Non-contact<br>- Safe for hostile environments | - Requires known **emissivity**<br>- Must fill sensor’s field of view<br>- Cannot measure internal temperature | Firefighting, industrial surface monitoring |

> ⚠️ **Note**: IR sensors are **not integrated into embedded systems** in this course → will not be covered in depth.  
> ⚠️ **注意**：红外传感器通常以手持设备形式存在，**不直接集成到嵌入式系统**，本课程不深入讲解。

---

## 🔍 Key Selection Criteria / 选型关键因素

- **Temperature range needed?**  
  需要多高温度？→ >800°C → only thermocouple.
- **Accuracy & stability critical?**  
  精度/稳定性要求高？→ RTD preferred (pharma/biotech).
- **Space-constrained?**  
  空间受限？→ Thermistor (tiny package).
- **Can you handle nonlinear math in firmware?**  
  能处理非线性算法吗？→ If not, avoid thermistors.
- **Need non-contact?**  
  需要非接触？→ Only IR — but with limitations.

---

## 💡 Practical Tips / 实用提示

- **Thermocouples**: Recalibrate annually due to metallurgical drift.  
  热电偶：因金属老化需每年校准。
- **RTDs**: Use 3- or 4-wire configuration to eliminate lead resistance error.  
  RTD：必须用三线或四线制消除导线电阻影响。
- **Thermistors**: Require lookup tables or Steinhart-Hart equation in code.  
  热敏电阻：需在固件中实现查表法或 Steinhart-Hart 公式。

---

> 🔜 **Next**: Deep dive into **thermistor specifications** (L05–L06).  
> 🔜 **下节课**：深入学习**热敏电阻技术参数**（L05–L06）。
