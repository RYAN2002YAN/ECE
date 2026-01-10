# Module 1 – Lesson 3: Analog and Digital Interfaces  
## 模块1 第3课：模拟与数字接口

## 🎯 Key Concepts / 核心概念

### 1. Why Convert to Digital? / 为何要数字化？
- Most physical quantities (temperature, pressure, etc.) are **continuous (analog)**.  
  大多数物理量（温度、压力等）是**连续变化的（模拟信号）**。
- Microprocessors only understand **digital data** → need ADC.  
  微处理器只能处理**数字信号** → 需要模数转换器（ADC）。

---

### 2. Signal Conditioning / 信号调理
- **Excitation**: Applying power to a sensor so it produces output.  
  **激励**：给传感器供电以产生输出信号。
- **Analog front-end**: Filters and amplifies raw sensor signal.  
  **模拟前端**：对原始信号进行滤波和放大。
- Placed **close to the sensor** to reduce noise and interference.  
  通常**紧靠传感器放置**，以抑制外部干扰。

---

### 3. Analog-to-Digital Conversion (ADC) / 模数转换
- Converts conditioned analog signal → digital code (8/12/16/24 bits).  
  将调理后的模拟信号转换为数字码（8/12/16/24 位）。
- Higher bit depth = higher resolution.  
  位数越高 → 分辨率越高。

---

### 4. Digital Communication Protocols / 数字通信协议
ADC output is often serialized via:
- **I²C** (Inter-Integrated Circuit)  
- **SPI** (Serial Peripheral Interface)  
- **RS-232** (Legacy serial)

> ✅ These allow reliable long-distance transmission with minimal error.  
> ✅ 可实现低误码率的远距离传输。

---

### 5. Integrated Sensors / 集成式传感器
- Some sensors (e.g., **humidity sensors**) include **ADC + signal conditioning on-chip**.  
  某些传感器（如湿度传感器）将**信号调理 + ADC 集成在单芯片内**。
- Output is **directly digital** → easy to connect to microcontroller.  
  输出为**纯数字信号** → 可直接连接微控制器。

---

### 6. The PSoC Microcontroller / PSoC 微控制器
- Used in this course: **Cypress PSoC series**.  
  本课程使用：**Cypress PSoC 系列**。
- Features built-in:
  - ADC
  - Amplifiers
  - Multiplexers
  - Comparators
  - Timers, counters, shift registers
- **Hardware-programmable**: Design circuits that run as real hardware inside the chip.  
  **硬件可编程**：所设计电路以真实硬件形式在芯片内部运行。
- **PSoC Creator**: IDE with schematic capture + code editor.  
  **PSoC Creator**：集成原理图绘制与代码编辑的开发环境。

---

### 7. Practical Tools / 实用工具
- Normally need expensive oscilloscope (e.g., Agilent).  
  通常需要昂贵的台式示波器（如安捷伦）。
- For this course: Use **low-cost USB oscilloscope** connected to laptop.  
  本课程可用**低成本 USB 示波器**（接笔记本电脑）。
- Recommended devices listed in **course syllabus**.  
  推荐型号见课程大纲。

---

> 💡 **Takeaway**:  
> Signal conditioning + ADC + digital interface = robust sensor system.  
> PSoC integrates all these blocks → fewer external components.  
>
> 💡 **要点**：  
> 信号调理 + ADC + 数字接口 = 健壮的传感器系统。  
> PSoC 集成所有模块 → 减少外部元件数量。

> 🔜 **Next**: Hands-on with PSoC Creator and thermistor lab.
