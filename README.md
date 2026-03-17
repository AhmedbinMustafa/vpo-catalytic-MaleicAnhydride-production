<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Maleic%20Anhydride%20Plant%20Design&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=32&desc=Catalytic%20Oxidation%20of%20n-Butane%20via%20VPO%20Catalyst&descAlignY=55&descSize=18"/>

<h3>80 MTPD Maleic Anhydride Production &nbsp;|&nbsp; 99.8% Purity &nbsp;|&nbsp; Full HAZOP & Process Control Design &nbsp;|&nbsp; Multi-Tubular Fixed Bed Reactor</h3>

![](https://img.shields.io/badge/Purity-99.8%25-brightgreen?style=for-the-badge)
![](https://img.shields.io/badge/Capacity-80%20MTPD-blue?style=for-the-badge)
![](https://img.shields.io/badge/Catalyst-VPO-orange?style=for-the-badge)
![](https://img.shields.io/badge/Reactor-Fixed%20Bed-red?style=for-the-badge)
![](https://img.shields.io/badge/University-COMSATS-purple?style=for-the-badge)

</div>

---

**Academic Context:** B.Sc. Chemical Engineering, COMSATS University Islamabad | 2022

---

## 📋 Overview
This repository contains the complete process engineering and plant design for a facility producing 80 metric tonnes per day (MTPD) of Maleic Anhydride (MAN) at 99.8% purity. The process utilizes the vapor-phase partial oxidation of n-Butane over a Vanadium Phosphorous Oxide (VPO) catalyst. This design demonstrates a modern, highly selective alternative to legacy benzene-oxidation pathways, offering superior economic viability and a reduced environmental footprint.

<img width="2488" height="1696" alt="Process_flow_diagram" src="https://github.com/user-attachments/assets/f6e730e5-b5b0-4498-b230-69247cd6169b" />

---

## ⚗️ Process Chemistry & Reaction Kinetics

The core of the process relies on the highly exothermic oxidation of n-Butane.

**Primary Reaction (72.25% Conversion):**
<div align="center">

$$\Large C_4H_{10} + 3.5\ O_2 \rightarrow C_4H_2O_3 + 4\ H_2O$$

</div>

**Secondary Reaction (12.75% Conversion):**
<div align="center">

$$\Large C_4H_{10} + 6.5\ O_2 \rightarrow 4\ CO_2 + 5\ H_2O$$

</div>

The reaction kinetics were modeled to determine the required catalyst weight and reactor volume. The reaction rate ($R$) was evaluated using the following kinetic model:

$$R = \frac{k_1 \cdot P_a^\alpha}{1 + K_2 \cdot P_c}$$

Where the rate constants were determined as $k_1 = 0.0418 \text{ kmol·kg}^{-1}\text{·h}^{-1}\text{·kPa}^{0.54}$ and $K_2 = 3.059 \text{ kPa}^{-1}$. Numerical integration via Polymath yielded a required VPO catalyst weight of 232.33 kg to achieve an 85% overall conversion rate.

---

## 🔥 Reactor Engineering & Thermodynamics

To manage the massive heat generation of the exothermic oxidation ($5.52 \times 10^7$ kJ/h), a **Multi-Tubular Fixed Bed Reactor** was designed.

| Parameter | Value |
|-----------|-------|
| 🌡️ Temperature | $420^\circ C$ |
| 📊 Pressure | 2.7 bar |
| 📦 Reactor Volume | $2.9\ m^3$ |
| ❄️ Heat Extracted | $55.2 \times 10^6$ kJ/h |
| ⚖️ Catalyst Weight | 232.33 kg |

* **Heat Integration:** A molten salt cooling loop (a eutectic mixture of $NaNO_2$ and $NaNO_3$) circulates through the reactor jacket to maintain isothermal conditions.

<img width="2282" height="1856" alt="control loops Reactor" src="https://github.com/user-attachments/assets/952ad713-773a-4962-a25b-b754204c9179" />

---

## 🔬 Separation & Purification Design

The downstream separation train isolates the MAN from water, unreacted butane, and off-gases using flash separation, gas absorption, and binary distillation.

### 1. Absorption Column

| Parameter | Value |
|-----------|-------|
| Stages | 13 sieve trays |
| Pressure | 1 bar |
| Solvent Flow | $2438.77\ kg/h$ |
| Column Diameter | $1.495\ m$ |
| Column Height | $7.8\ m$ |

<img width="2590" height="1632" alt="Absorber" src="https://github.com/user-attachments/assets/5b03b52b-7e70-44c1-81a2-161bf23fa9b2" />

### 2. Binary Distillation Column

The aqueous MAN mixture is dehydrated to achieve the final 99.8% product purity.

* **Relative Volatility ($\alpha$):** Calculated as 22.65 at the feed temperature of $138.8^\circ C$ using Antoine's Equation.
* **Stage Calculation:** The minimum number of theoretical stages ($N_{min} = 3$) was determined using **Fenske's Equation**:

$$N_{min} = \frac{\ln \left( \frac{x_d(1-x_w)}{x_w(1-x_d)} \right)}{\ln(\alpha)} - 1$$

* **Column Sizing:** The **Lewis-Sorel method** was applied to generate the top and bottom operating lines, resulting in 8 ideal stages. Factoring in a 54% molar average column efficiency, the physical column requires 15 actual bubble-cap trays.

<img width="878" height="1248" alt="distillation column loop" src="https://github.com/user-attachments/assets/fc176499-38fd-4347-86c1-718afa733bcb" />

---

## 🛡️ Instrumentation, Control & Safety (HAZOP)

The plant utilizes advanced process control (APC) loops, including feed-backward, ratio, and auctioneering configurations to stabilize critical nodes. A comprehensive HAZOP analysis was conducted to evaluate process deviations (e.g., thermal runaway, pressure buildup) and size appropriate relief valves and interlocks for the high-temperature reactor and distillation sections.

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer"/>

</div>
