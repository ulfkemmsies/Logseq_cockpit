file-path:: file://C:/Users/ulfkemmsies/Zotero/storage/H2UXGAD5/Ref4.pdf

- The Navier-Stokes equations have been used in the simulations to model the behavior of the flow 15,16. These equations (equations [3-5]) are used to describe any flow in the continuum regime.
  hl-page:: 2
  ls-type:: annotation
  id:: 64760ef0-7766-467b-8f60-13b183bbe9b9
  hl-color:: yellow
  \(\begin{gathered}\frac{\partial \rho}{\partial t}+\nabla(\rho \vec{u})=0 \\ \rho\left(\frac{\partial \vec{u}}{\partial t}+\vec{u} \cdot \nabla \vec{u}\right)=-\nabla p+\nabla \cdot \tau+f \\ \rho C_v\left(\frac{\partial T}{\partial t}+T \cdot \nabla T\right)=-p \nabla \cdot \vec{u}+\nabla \cdot(k \nabla T)+\tau \cdot \nabla \vec{u}\end{gathered}\)
  where 𝜌 is the density, 𝑡 is the time, 𝒗 is the fluid velocity, 𝑝 is the pressure 𝜏 is the viscous stress tensor, 𝒇 is an external force acting on the control volume, 𝑅 is the specific gas constant, 𝑇 is the temperature, and 𝐶𝑣 is the specific heat at constant volume.
- Assuming the flow unidirectional and the density constant over time
  ls-type:: annotation
  hl-page:: 2
  hl-color:: red
  id:: 64760f42-1ea0-479d-acb9-7925224b2275
- If we define the velocity as the state of the system we can re-write it in the state space form \(\dot{x}=A x+B \bar{u}\) considering the pressure drop as the input \(\bar{u}=\Delta p\) :
  ls-type:: annotation
  hl-page:: 3
  hl-color:: yellow
  id:: 6476100a-908a-4923-85f9-2d66cc2abf32
  $$
  \frac{\partial u}{\partial t}=-\frac{8 \eta}{R^2 \rho} u-\frac{\Delta p}{\rho L}
  $$
- control, we consider a single cylindrical channel connecting the valve to the chamber through which the liquid propellant is fed. The channel is modeled using Navier-Stokes equations considering the flow as incompressible and unsteady as seen in equation, where \(\vec{u}\) is the velocity, \(\rho\) is the density of the fluid, \(p\) is the pressure, and \(\eta\) is the dynamic viscosity of the fluid.
  hl-page:: 2
  ls-type:: annotation
  id:: 64761041-94dc-4815-a142-a46ab3b26604
  hl-color:: red
- Applying the boundary conditions to calculate the constants:
  hl-page:: 2
  ls-type:: annotation
  id:: 647610bb-aeb5-4231-b95f-568d0a72636c
  hl-color:: red
  \(\left\{\begin{array}{l}\left.\frac{\partial u}{\partial r}\right|_{r=0}=0 \\ \left.u\right|_{r=R}=0\end{array}\right.\)