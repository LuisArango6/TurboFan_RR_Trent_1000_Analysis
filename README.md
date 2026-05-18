# ***TurboFan RR Trent 1000 Analysis***

Thermodynamic analysis of a **Rolls-Royce Trent 1000 turbofan engine** model.  
The project implements a **stage-by-stage cycle simulation** of both the fan and the core, evaluated at:

- Take-off conditions (2600 m ASL)  
- Cruise conditions (11000 m ASL)

The objective is to provide a **clear and structured thermodynamic model in Python**, where each engine component, governing parameters, and resulting performance metrics are explicitly analyzed.

---

##  ***Results***

The model computes and visualizes:

-  Temperature and pressure at each engine station  
-  Net thrust, specific fuel consumption (SFC), and specific range  
-  Performance analysis through:
  - Temperature and pressure profiles across stations  
  - Thrust vs Mach number sweep  
  - Thrust breakdown (momentum + pressure contributions)  
  - Parametric sensitivity analysis:
    - Fan Pressure Ratio (FPR)  
    - Turbine Inlet Temperature (TiT)  
    - Bypass Ratio (BPR)  

---

## ***Methodology***

The analysis is based on:

- Conservation of mass and energy  
- Isentropic relations with efficiency corrections  
- Combustion modeling via fuel–air ratio  
- Nozzle flow analysis (choked and unchoked regimes)  
- Symbolic resolution of shaft balances  

---

##  ***Dependencies***

- **ambiance** — ISA standard atmosphere model  
- **CoolProp** — thermophysical properties of air  
- **sympy** — symbolic equation solving  
- **numpy / matplotlib** — numerical computation and visualization  

---

##  ***Usage***

1. Install dependencies:

```bash
pip install numpy matplotlib sympy CoolProp ambiance
