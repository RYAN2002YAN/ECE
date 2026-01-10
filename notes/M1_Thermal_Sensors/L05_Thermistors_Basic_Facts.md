# Module 1 – Lesson 5: Thermistors – Basic Facts  
## 模块1 第5课：热敏电阻基础事实

> 📌 **Status**: ⬜ Not Started | **Video Duration**: ~3.5 min  
> 📌 **状态**：⬜ 未开始 | **视频时长**：约3分30秒

---

## 🎯 Core Characteristics / 核心特性

### 1. What is a Thermistor? / 什么是热敏电阻？
- Made of **sintered semiconductor or metal oxide**.  
  由**烧结半导体或金属氧化物**制成。
- **NTC (Negative Temperature Coefficient)** is most common:  
  **NTC（负温度系数）** 最常见：
  - Resistance **decreases sharply** as temperature ↑.  
    温度升高 → 电阻**急剧下降**。
- Highly **nonlinear** R vs. T curve → material-dependent.  
  电阻-温度关系高度**非线性**，且依赖材料配方。

---

### 2. Key Parameters / 关键参数

| Parameter | Value / Note |
|----------|--------------|
| **Base Resistance (R₂₅)** | Resistance at **25°C** |
| Common R₂₅ Values | **2,252 Ω**, **10,000 Ω (10kΩ)** |
| High-Temp R₂₅ | **30kΩ**, **50kΩ** (for >100°C) |
| **Typical Range** | **-50°C to +70°C** (consumer electronics) |
| **Max Range** | Up to **200°C** (with special packaging) |
| **Accuracy** | **±0.1°C to ±0.2°C** (with good calibration) |

---

### 3. Packaging & Limitations / 封装与限制

- **Materials**: Glass or epoxy encapsulation.  
  **封装材料**：玻璃或环氧树脂。
- **Limitation**: Upper temperature capped by package (usually ≤200°C).  
  **限制**：封装材料限制最高温度（通常 ≤200°C）。

---

## 🔧 Common Applications / 常见应用

| Application | How It’s Used |
|------------|----------------|
| **Smartphones / Laptops** | Overheat protection (shutdown if too hot) |
| **LCD Displays** | Measure internal temp → adjust contrast compensation |
| **Thermostats** | Replaced bimetallic strips for higher accuracy |
| **Lithium Batteries** | Embedded thermistor monitors cell temperature (safety critical) |
| **Fluid Sensing** | Metal-probe thermistors (e.g., 10kΩ) for immersion |

> 💡 **Fun Fact**: You can buy Li-ion batteries with **pre-installed thermistors** on eBay!  
> 💡 **趣闻**：可在 eBay 购买到**预装热敏电阻**的锂电池！

---

## 📦 Physical Forms / 物理形式

- **Through-hole**: e.g., **44008RC** – for PCB assembly  
  通孔插件：如 44008RC，用于电路板焊接
- **Metal Probe**: For fluid/air immersion (like thermocouples)  
  金属探头：用于液体/气体测温
- **IC-like**: e.g., **MCP9700** (actually a linear analog temp sensor, not NTC)  
  IC 封装：如 MCP9700（注：此为线性传感器，非 NTC 热敏电阻）

> ⚠️ Note: MCP9700 is **not a thermistor** – it’s a silicon-based linear sensor. Mentioned here as a packaged alternative.  
> ⚠️ 注意：MCP9700 **不是热敏电阻**，而是硅基线性温度传感器，此处仅作封装形式参考。

---

## 💡 Key Takeaways / 关键要点

- NTC thermistors = **high sensitivity + small size + low cost**.  
  NTC 热敏电阻 = 高灵敏度 + 小体积 + 低成本。
- Best for **narrow-range, high-accuracy** applications (<200°C).  
  适用于**窄温区、高精度**场景（<200°C）。
- **Nonlinearity requires calibration** (Steinhart-Hart equation in firmware).  
  非线性需通过校准处理（固件中使用 Steinhart-Hart 方程）。
- Ubiquitous in **consumer electronics and battery safety**.  
  广泛用于消费电子与电池安全。

---

> 🔜 **Next**: *How Thermistors Work* – deep dive into physics and equations (L06).  
> 🔜 **下节课**：《热敏电阻工作原理》——深入物理机制与数学模型（L06）。
