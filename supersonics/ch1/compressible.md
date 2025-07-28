---
title: 1.1 Compressible Flows
description: An introduction to compressible flows, exploring thermodynamic properties like isothermal compressibility and volume expansion in high-speed aerodynamics.
keywords: ['Compressible Flows', 'Supersonic Flows', 'Thermodynamics', 'Isothermal Compressibility', 'Volume Expansion']
tags: ['Shockwaves', 'Compressible Flows', 'High-Speed Flight']
---

# 1.1 Compressible Flows

Supersonic flows are fundamentally compressible. At first glance, one might define compressible flows as those with variable density. While partially true, this definition is incomplete, not all flows with density variations are truly compressible in the aerodynamic sense.

## Thermodynamic Perspective

To understand compressibility, we turn to thermodynamics. The **specific volume** $v$ is expressed as a function of temperature $T$ and pressure $P$:

```{math}
:label: eq-specific-volume
v = v(T, P)
```

Differentiating this expression yields:

```{math}
:label: eq-total-diff
dv = \left( \frac{\partial v}{\partial P} \right)_T dP + \left( \frac{\partial v}{\partial T} \right)_P dT
```

Dividing both sides by $v$, we obtain the fractional change in specific volume:

```{math}
:label: eq-fractional-dv
\frac{dv}{v} = -\kappa_T dP + \beta dT
```

**This introduces two key thermodynamic properties:**

- **Isothermal compressibility** $ \kappa_T $, which quantifies the change in specific volume due to pressure at constant temperature:

  ```{math}
  :label: eq-kappaT
  \kappa_T = -\frac{1}{v} \left( \frac{\partial v}{\partial P} \right)_T
  ```

- **Coefficient of volume expansion** $ \beta $, which quantifies the change in specific volume due to temperature at constant pressure:

  ```{math}
  :label: eq-beta
  \beta = \frac{1}{v} \left( \frac{\partial v}{\partial T} \right)_P
  ```

Equation {eq}`eq-fractional-dv` shows that changes in specific volume (or density) result from both **pressure** and **temperature** variations. In high-speed flows, where density changes are primarily driven by pressure, the flow exhibits significant **compressibility effects**. Conversely, in flows like natural convection, where pressure is nearly constant and density changes stem from temperature variations, the flow is often treated as **incompressible**, despite a non-zero $ \beta $ in {eq}`eq-beta`.

> In high-speed aerodynamics, compressibility is defined by the dominance of pressure-induced density changes, not merely the presence of density variation.


:::{important}
## Exercise: Compressibility in Different Flows

**Background**: The discussion above focuses on air, where compressibility is significant in supersonic flows due to pressure-driven density changes. However, isothermal compressibility and the coefficient of volume expansion are thermodynamic properties applicable to all materials, including liquids.

**Question**: Consider the following scenarios:

1. A supersonic jet flying at Mach 2 at high altitude (air).
2. Water flowing through a high-pressure hydraulic pipe.
3. Lava flowing down the side of a volcano.

**Using the framework of isothermal compressibility and coefficient of volume expansion**:

a) For each case, discuss whether *compressible flow effects* are likely to be significant, and why.

b) For the water and lava flows, density can vary slightly due to pressure or temperature. Are these flows *compressible* in the same sense as supersonic flows? Why or why not?

:::{dropdown} Show Answer
**a)**  
- **Supersonic Jet (Mach 2):**  
  Compressible effects are *very significant*. Large pressure changes around the aircraft cause substantial density variations. Air’s high isothermal compressibility makes these effects dominant, requiring compressible flow theory for analysis.  
- **Water in a High-Pressure Hydraulic Pipe:**  
  Despite high pressures, water’s isothermal compressibility is very low (about 50 times less than air). Density changes due to pressure are *minimal*, so compressible flow effects are negligible, and the flow is typically treated as incompressible.  
- **Lava Flow:**  
  Lava, a molten liquid, has very low compressibility, similar to water. Even with temperature and pressure gradients, density changes are minor, so compressible flow effects are not significant in most practical cases.

**b)**  
For **water and lava**, the flows are *not* compressible in the same sense as supersonic flows.  
- While density may vary slightly due to pressure or temperature, these changes are extremely small compared to those in high-speed gas flows.  
- **Significant compressibility effects (for flow analysis) arise only when pressure-induced density changes are large enough to affect flow behavior.**  
- For most liquids, even under high pressure or temperature, these changes are so small that the incompressible flow assumption is valid.
:::


