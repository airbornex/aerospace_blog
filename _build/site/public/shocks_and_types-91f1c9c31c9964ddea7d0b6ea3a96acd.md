# 2.1 Shocks and Their Classification

Shock waves are thin regions within a flow where abrupt and irreversible changes occur in flow properties such as pressure, temperature, density, and velocity. These discontinuities arise in compressible flows when the local Mach number exceeds unity, preventing upstream propagation of information. To accommodate such high-speed disturbances, the flow adjusts through the formation of shock waves, fundamentally governed by the conservation laws of mass, momentum, and energy.

**1 .Normal Shocks**

A **normal shock** is a shock wave that is perpendicular to the direction of the flow. It is the most fundamental form of shock and serves as the basis for one-dimensional shock analysis.

* Occurs in ducted flows or symmetric configurations.
* Always results in a transition from supersonic to subsonic flow.
* Associated with significant increases in pressure and temperature, and a decrease in Mach number.
* Governed by the *normal shock relations*, derived from the conservation equations.

:::{figure} ./images/normal_shock.png
:name: normal-shock
:width: 70%
:align: center
:class: framed

<span class="source-medium">Schlieren images of normal shock wave turbulent boundary layer interactions attached at </span> $M_\infty = 1.28$ <span class="source-medium">,</span> $Re_{x_{shock}} = 1.79 × 10^6$  {cite}`davidson2018influence`
:::

**2. Oblique Shocks**

An **oblique shock** occurs when the shock front is inclined at an angle to the oncoming flow. These arise in external flows over wedges or in internal duct flows where turning occurs.

* Flow deflection occurs across the shock.
* The upstream flow remains supersonic after the shock if the shock is weak and the deflection angle is small.
* The shock can be attached (pointing from the surface) or detached (ahead of blunt bodies).
* Governed by the *θ–β–M relation*, where:

  * θ is the flow deflection angle,
  * β is the shock angle,
  * M is the upstream Mach number.

<!-- \:::{figure} ./images/oblique\_shock\_diagram.png
\:name: oblique-shock
\:width: 70%
\:align: center
\:class: framed

<span class="source-medium">Oblique shock formation on a wedge at supersonic flow conditions.</span>
\::: -->

**3. Bow (Detached) Shocks**

When a blunt body moves at supersonic speeds, the shock wave cannot remain attached to the body. Instead, a **bow shock** or **detached shock** forms ahead of the object.

* Common in blunt-nosed launch vehicles or capsules.
* Results in a strong shock structure with high entropy generation.
* The stagnation point at the body surface experiences the highest pressure and temperature.

**4. Expansion Fans (Not Shocks, but Related)**

While not technically shocks, **Prandtl–Meyer expansion fans** are another form of compressible turning flow.

* Occur when supersonic flow turns around a convex corner.
* Flow accelerates and Mach number increases.
* Entropy remains constant; expansion is isentropic.

**5. Shock–Shock Interactions**

When multiple shock waves intersect, their interaction can result in complex wave structures:

* **Regular reflection**: Oblique shock reflects at a wall forming another oblique shock.
* **Mach reflection**: At higher Mach numbers or deflection angles, a third, stronger shock called a *Mach stem* forms between incident and reflected shocks.
* These phenomena are particularly important in supersonic inlets and high-speed impact dynamics.

**6. Shock Classification by Strength**

Shocks may also be categorized by their *strength*, determined by the pressure ratio or Mach number change across the shock:

* **Weak shocks**: Small change in flow properties; often found in small deflection oblique shocks.
* **Strong shocks**: Large property changes; typically occur near blunt objects or at high Mach numbers.
* **Hypersonic shocks**: Associated with Mach numbers > 5; often lead to dissociation, ionization, and real gas effects.