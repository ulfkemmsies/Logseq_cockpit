public:: true
id:: d87cb3e3-b6b9-458b-8f91-7187b1c68b36

- Title
	- Integrating Analytical Models for Vaporizing Liquid Micropropulsion Systems: Towards Next-Generation Design and Flow Behavior Characterization
- Abstract
	- This paper presents a comprehensive approach to designing the next generation of vaporizing liquid micropropulsion systems. The study proposes a framework that integrates existing analytical models for key components of the system and characterizes the flow behavior within the system. By leveraging the strengths of these models and gaining insights into the complex fluid dynamics, heat transfer, and combustion processes, the proposed approach aims to overcome design challenges and achieve more accurate predictions and efficient designs. The framework holds significant potential for advancing the field of micropropulsion systems, enabling enhanced efficiency, reliability, and maneuverability for small satellites in space missions.
- Introduction
	- This paper presents a comprehensive approach to designing the next generation of vaporizing liquid micropropulsion systems by combining existing analytical models and characterizing the flow behavior. Micropropulsion systems play a crucial role in various space missions, enabling precise control and maneuverability of small satellites. However, the design and optimization of these systems remain challenging due to the complex interplay of fluid dynamics, heat transfer, and combustion processes.
	  
	  TU Delft has been one of the centers of research around Vaporizing Liquid Microthrusters, with several papers published in the past few years considering different aspects of VLMs. However, each model depends on assumptions that limit its predictive power experimentally, and often focus on single elements of the VLM, like the flow in the heating chamber microchannels, the nozzle's performance, or control of the propellant injector to ensure constant thrust. There is a gap in the literature for an integrated model which characterizes the entire VLM's behavior based on a few inputs, mainly related to sizing the system.
	  
	  To address these challenges, this study proposes a novel framework that integrates multiple analytical models to enhance the understanding and performance of vaporizing liquid micropropulsion systems. By leveraging existing models, we aim to capitalize on their strengths and overcome their limitations, ultimately leading to more accurate predictions and efficient designs.
	  
	  The first step involves a comprehensive review and selection of relevant analytical models for key components of the micropropulsion system, including the inlet, combustion chamber, and nozzle. Each model is carefully evaluated based on its applicability, accuracy, and computational efficiency. Subsequently, these models are integrated into a unified framework, allowing for a holistic analysis of the system's behavior.
	  
	  By combining existing analytical models and characterizing flow behavior, we can overcome the limitations of individual models and achieve a more comprehensive understanding of system performance. This, in turn, will facilitate the design of next-generation micropropulsion systems that offer enhanced efficiency, reliability, and maneuverability for small satellites in space missions.
- Literature Review and Modeling
	- The given source material was composed of previous student-led investigations on the topic and professional research by TUD researchers.
	- Model overview
		- The general structure of the VLM is taken from [[@A Comprehensive Model for Control of Vaporizing Liquid Microthrusters]] and is shown in Figure X:. Water is pressurized to mimic the conditions of a blow-down propellant feed and fed into the inlet of the heating chamber. A resistive heater is used to heat the walls of the microchannels of the chamber, and the water is assumed to lose pressure due to the mechanics of wavy microchannels before boiling. The resulting vapor is accelerated through the remaining channel length toward the micronozzle. The nozzle is a standard axisymmetric choked convergent-divergent type.
	- Assumptions
		- The assumptions for the system under consideration are as follows:
		  
		  \begin{enumerate}
		      \item Water enters the system at the inlet under pressure and at a standard temperature of 22°C. The corresponding density of the water is 997.8 kg/m3.
		      
		      \item Inside the heating chamber, water flows and experiences a decrease in pressure due to convective effects caused by wavy flow.
		      
		      \item The vapor phase of the water remains at the same temperature and pressure as it undergoes boiling until it reaches the nozzle. There is no additional heat transfer from the walls of the system to the vapor phase during this process.
		      
		      \item The nozzle is assumed to have axisymmetric choked flow, meaning that the flow rate is at its maximum and no further increase is possible. Additionally, there is no heat transfer occurring between the walls of the nozzle and the gas.
		      
		      \item The heaters in the system uniformly heat the entire volume of liquid and vapor mixture (VLM), ensuring that all the walls of the heating chamber and nozzle are at the same temperature, denoted as Tw.
		      
		      \item Inside the heating chamber, a constant heat flux is maintained, while the wall temperature along the entire nozzle remains constant.
		  \end{enumerate}
		- Water enters pressurized at the inlet at standard temperature (22 C), the corresponding density is 997.8 kg/m3.
		- Water flows inside the heating chamber, losing pressure through convective effects due to wavy
		- Vapor remains at same temperature and pressure from boiling until nozzle largely without extra heat transfer from the walls
		- Nozzle is axisymmetric choked flow and no heat transfer between nozzle walls and gas occurs
		- Heaters heat the entire VLM equally, so that all the walls of the heating chamber and nozzle are at the same temperature $T_w$.
		- Constant heat flux inside the heating chamber and constant wall temperature along the entire nozzle
	- Ideal Rocket Theory and General Equations
		- Ideal Gas Relation
		  
		  The ideal gas theory is a simplified model that describes the behavior of gases under certain conditions. It assumes that gas particles are point masses with no volume, and that they move randomly and independently. The theory states that the pressure, density, and temperature of an ideal gas are related by the equation:
		  
		  \[ P = \rho \cdot R_s \cdot T \]
		  
		  where \(P\) is the pressure, \(\rho\) is the density, \(R_s\) is the ideal gas constant, and \(T\) is the temperature in Kelvin.
		  
		  It is important to note that this theory assumes incompressibility, and therefore cannot be used once the Mach number \( Ma > 0.3\), which means anywhere in the nozzle, since choked flow at the throat is assumed.
		- Speed of sound
		  
		  The speed of sound refers to the rate at which sound waves propagate through a medium. It is influenced by various factors, including the properties of the medium and the temperature. In an ideal gas, the speed of sound can be determined using the equation:
		  
		  \[
		  a = \sqrt{\gamma \cdot R \cdot T}
		  \]
		  
		  where:
		  \(a\) represents the speed of sound,
		  \(\gamma\) denotes the adiabatic index (also known as the heat capacity ratio),
		  \(R\) represents the specific gas constant, and
		  \(T\) denotes the temperature of the medium.
		  
		  It is important to note that this equation assumes an ideal gas behavior and neglects other factors that may affect the speed of sound, such as humidity or pressure.
		- Kinematic viscosity
		  
		  Kinematic viscosity is a measure of a fluid's resistance to flow under the influence of gravity. It is defined as the ratio of dynamic viscosity to density. The equation for kinematic viscosity (\(\nu\)) is given by:
		  
		  \[\nu = \frac{\mu}{\rho}\]
		  
		  where \(\mu\) represents the dynamic viscosity and \(\rho\) represents the density of the fluid.
	- Sizing
		- Inlet
		  The main model inputs for the circular inlet are the chosen mass flow $\dot{m}_{1}$ and the inlet radius $R_{in}$, which will the determine the pressure of the water.
		- Heating Chamber
		  This chamber consists of wavy microchannels with 3 heated sides (the top wall consists of the next layer in the assembly) and a fixed geometry taken from [[@Micropropulsion course Numerical analysis of wavy microchannels employed in a Vaporizing Liquid Micro-resistojet thruster]] as shown in Figure X. In order to simplify the modeling process, the standard unit was used unaltered, and this geometry is repeated $n_{elem}$ times along the length of the chamber to form a single channel. Along the width of the VLM, $n_{chan}$ channels are used to form the complete heating chamber.
		  
		  The centerline $L_C = 1.00714$ mm and length $L = 0.64$ mm of one such element have been previously determined, and need only be multiplied by the number of elements to be calculated for the whole chamber.
		  
		  The other main sizing variable for the heating chamber is the chamber depth $H$, which will determine the total area of the heated walls $A_{heat}$ when multiplied by the integrated wall length according to $$(2.01062 \ mm \cdot H + 0.213126 \ mm^{2} ) \cdot n_{elem} \cdot n_{chan}$$. The total volume of the chamber $V_{tot}$ is similarly calculated using \( (0.213126 \ mm^{2} \cdot H ) \cdot n_{elem} \cdot n_{chan}\).
		  
		  Finally, the hydraulic diameter of this same cross-section is calculated with \(D_h=\frac{4 A}{p}\), where $A$ is the cross-sectional area and $p$ the rectangular perimeter.
		- Nozzle
		  The micronozzle has three main sizing input variables: the throat radius $R_t$, the exit radius $R_e$, and the nozzle length $L_n$. The diverging section of the nozzle is assumed to expand outward from the throat without any curvature, so that the length along the nozzle wall can be found with \( x = \sqrt{R_{e}^2 + L_{n}^2} \), and the nozzle exit half-angle with \( \alpha = \tan^{-1} \left( \frac{R_{e}}{L_n} \right) \).
	- Heating Chamber Liquid Phase
		- The assumptions of the model used in this phase, in the original paper [[@Micropropulsion course Numerical analysis of wavy microchannels employed in a Vaporizing Liquid Micro-resistojet thruster]], are as follows:
		  • Incompressible flow
		  • Steady state (this was verified with transient simulations)
		  • Negligible radiative and natural convective heat transfer
		  • Negligible viscous dissipation
		  • Laminar flow
		  • Constant fluid properties
		  This is due to the extremely low Reynolds numbers found in that investigation, and in order to keep the validity of the model intact, we must design our liquid flow phase according to those low Reynolds numbers. Additionally, constant heat flux from the walls was assumed, although in that model, the heat flux was chosen to ensure the flow would stay liquid, which is not the case in this more comprehensive model.
		- The essence of this phase of the model is characterizing the loss in pressure (which can be seen either as a performance loss or as an increased requirement in the pressure of the propellant tank) due to friction and the interaction of the fluid with the waviness of the channel walls. Once the pressure at boiling is found, the boiling temperature follows, and the rest of the conditions can be calculated. This is done using the following equations and quantities, and the exact simulation procedure will be discussed in a later chapter.
			- Dynamic Viscosity
			  
			  Dynamic viscosity is a measure of a fluid's resistance to flow under an applied force or stress. It quantifies the internal friction within a fluid as it flows, determining how easily the fluid deforms or shears. In simpler terms, dynamic viscosity describes how "thick" or "sticky" a fluid is, with higher viscosity indicating a thicker or more resistant fluid, and lower viscosity indicating a thinner or more easily flowing fluid. It is typically measured in units of pascal-seconds (Pa·s) or poise (P).
			  
			  Because dynamic viscosity is dependent on the temperature of a liquid, a fitted equation was found that interpolates the experimental values reported on EngineeringToolbox for water.
			  
			  The equation for dynamic viscosity (\(\mu\)) and temperature (\(T\)) for water is:
			  
			  \[
			  \mu = a \cdot T^6 + b \cdot T^5 + c \cdot T^4 + d \cdot T^3 + e \cdot T^2 + f \cdot T + g
			  \]
			  
			  where:
			  \[
			  a = 5.26010734 \times 10^{-14}
			  \]
			  \[
			  b = -1.44312831 \times 10^{-10}
			  \]
			  \[
			  c = 1.63771197 \times 10^{-7}
			  \]
			  \[
			  d = -9.84335889 \times 10^{-5}
			  \]
			  \[
			  e = 3.30686535 \times 10^{-2}
			  \]
			  \[
			  f = -5.89414841 \times 10^{0}
			  \]
			  \[
			  g = 4.36419186 \times 10^{2}
			  \]
			- Reynolds number
			  id:: 64b187ff-4ac4-4fb1-b528-64d9ff78d098
			  
			  The Reynolds number is a dimensionless quantity used in fluid mechanics to characterize the flow of a fluid, such as water, through a pipe or any other conduit. It helps determine the type of flow, whether it is laminar or turbulent, based on the fluid's velocity, density, viscosity, and the characteristic length or diameter of the conduit.
			  
			  The Reynolds number is calculated using two different formulas, both of which are equivalent but used in different situations. The first formula is:
			  
			  $$
			  R e=\frac{\dot{m} \cdot D_h}{A \cdot \mu}
			  $$
			  
			  In this formula, \(Re\) represents the Reynolds number, \(\dot{m}\) is the mass flow rate of the fluid, \(D_h\) is the hydraulic diameter of the conduit, \(A\) is the cross-sectional area of the flow region, and \(\mu\) is the dynamic viscosity of the fluid. For circular cross-sections, the hydraulic diameter can just be replaced by the cross-sectional diameter.
			  
			  This equation can alternatively be expressed as 
			  
			  $$R e=\frac{ u \cdot D_h}{v}$$
			  
			  where \(u\) is the flow velocity and \(v\) the kinematic viscosity.
			  
			  The Reynolds number is crucial in determining the flow regime of a fluid. When the Reynolds number is below a certain critical value, the flow is considered laminar, characterized by smooth and orderly movement of fluid layers. On the other hand, when the Reynolds number exceeds the critical value, the flow becomes turbulent, with chaotic and irregular fluid motion.
			- Water Boiling Temperature
			  
			  The equation provided in the function is a polynomial fit that approximates the relationship between water boiling temperature \(\left(T_{boil}\right)\) and pressure \(p\). This polynomial fit is based on empirical data collected from EngineeringToolbox. The equation is given by:
			  $$
			  T_{boil}=-1.98450335 \times 10^{-10} \cdot p^2+2.48821438 \times 10^{-4} \cdot p+ 3.50254608 \times 10^2
			  $$
			  ​
			  This equation is an approximation and might not accurately represent extreme conditions, although the range of 0-100 degrees Celsius was used.
		- Heating Chamber Liquid Phase Performance Metrics
			- Nusselt number
			  id:: 64b187ff-20cf-46c6-a290-4d508fe0c853
			  
			  The Nusselt number is a dimensionless parameter used in heat transfer analysis to quantify the relationship between convective and conductive heat transfer across a boundary or surface.
			  It considers factors such as thermal conductivity, fluid properties, and flow characteristics. For low Reynolds numbers (between 10 and 100), the Nusselt number increases significantly with increasing Reynolds numbers.
			  
			  A higher Nusselt number also means that, given a wall temperature, a shorter channel is needed to reach certain fluid temperature (or vaporization).
			  
			  Studies have shown that wavy microchannels result in higher Nusselt numbers and improved convective heat transfer compared to straight channels of the same size. However, this improvement comes at the cost of increased pressure losses. 
			  
			  The Nusselt number can be calculated using the equation:
			  
			  $$N u=\frac{h \cdot D_h}{k_W}$$
			  
			  where \(h\) is the convective heat transfer coefficient, \(D_h\) is the hydraulic diameter, and \(k_W\) is the thermal conductivity.
			- Thermal conductivity
			  
			  The thermal conductivity of water \(k_w\) is temperature dependent, and therefore an equation fitted on experimental data from EngineeringToolbox was found for fast calculation.
			  
			  $$
			  k_w=a \cdot T_{m}^3+b \cdot T_{m}^2+c \cdot T_{m}+d
			  $$
			  
			  $$
			  \begin{aligned}
			  & a=4.07234630 \times 10^{-5} \\
			  & b=-4.91309248 \times 10^{-2} \\
			  & c=2.01086194 \times 10^1 \\
			  & d=-2.10087790 \times 10^3
			  \end{aligned}
			  $$
			  \(T_{m}\) is the mean temperature of the water.
			- Heat transfer coefficient
id:: 64b187ff-2940-4304-8395-8954d0948db6
			  $$
			  h=\frac{q}{A_{\text {wall heat }} \cdot\left(T_w-T_m\right)}
			  $$
			  
			  where \(T_w\) is the chosen temperature of the three heated walls and \(A_{\text {wall heat }}\) is their area (of the section of the heating chamber needed until vaporization), and \(T_m\) is the mean fluid temperature calculated using 
			  
			  \(T_m=0.5 \cdot\left(T_{\text {in }}+T_{\text {out }}\right)\)
			  
			  In this case, the inlet and outlet temperatures of the water are the initial tank temperature and the boiling temperature.
			  
			  making an average over the whole fluid volume due to the constant wall temperature assumption.
	- Heating Chamber Gaseous Phase
		- The equations to model the gaseous phase inside the heating chamber were taken from the Micropropulsion course reader, and essentially consist of solving the two equation system:
		  
		  $$
		  P_h=\dot{m} \cdot\left[c_{p L} \cdot\left(T_{b o i l}-T_0\right)+L_h+c_{p G} \cdot\left(T_C-T_{b o i l}\right)\right]
		  $$
		  
		  $$
		  \dot{m}=\frac{p_C \cdot A^*}{\sqrt{\frac{R_A}{M_W} \cdot T_C}} \cdot \sqrt{\gamma \cdot\left(\frac{1+\gamma}{2}\right)^{\frac{1+\gamma}{1-\gamma}}}
		  $$
		  
		  where \(P_h\) is the available heating power, \(T_0\) is the initial propellant temperature, \(T_{\text {boil }}\) is the propellant boiling temperature (which in turn is a function of the heating chamber pressure), \(c_{p L}\) and \(c_{p G}\) are the constant pressure specific heat of respectively the liquid and gaseous propellant phase (both usually functions of the temperature), \(L_h\) is the latent heat of vaporization of the propellant.
		  
		  The tank pressure, which is assumed to stay constant over the length of the heating chamber, is an input along with a chosen heating power. Since the boiling temperature is known from the pressure and the initial temperature is set, that leaves the mass flow and final chamber gas temperature to be solved for. This is done using a combination of a grid-search method and optimizer, as during calculations non-unique solutions with comparable error tolerances were found, with the least erroneous option chosen and further optimized.
	- Nozzle
		- Throat Condition
			- Critical Throat Condition ratios [source](https://farside.ph.utexas.edu/teaching/336L/Fluid/node197.html)
			  
			  Starting from the isentropic equations relating stagnation conditions (zero subscript) to local flow Mach number:
			  
			  \begin{aligned}
			  & \frac{p}{p_0}=\left(\frac{T}{T_0}\right)^{\gamma /(\gamma-1)}=\left[1+\frac{1}{2}(\gamma-1) \mathrm{Ma}^2\right]^{-\gamma /(\gamma-1)} \\
			  & \frac{\rho}{\rho_0}=\left(\frac{T}{T_0}\right)^{1 /(\gamma-1)}=\left[1+\frac{1}{2}(\gamma-1) \mathrm{Ma}^2\right]^{-1 /(\gamma-1)} .
			  \end{aligned}
			  
			  Setting \(Ma = 1\) as we are assuming perfectly sonic flow at the throat yields:
			  
			  \begin{aligned}
			  & \frac{T_1}{T_0}=\left(\frac{2}{\gamma+1}\right) \\
			  & \frac{p_1}{p_0}=\left(\frac{2}{\gamma+1}\right)^{\gamma /(\gamma-1)}, \\
			  & \frac{\rho_1}{\rho_0}=\left(\frac{2}{\gamma+1}\right)^{1 /(\gamma-1)} .
			  \end{aligned}
			  
			  These relations between the stagnation conditions in the chamber to those in the throat (1 subscript) are used to characterize throat flow.
			- Steam dynamic viscosity
			  
			  The dynamic viscosity of water steam is temperature and pressure dependent, so experimental values reported on EngineeringToolbox were taken and turned into a lookup table with linear interpolation between data points. The dynamic viscosity values are measured in centipoise \((\mathrm{cP})\), a common unit for viscosity, which is multiplied by \( 10^3\) to get the elsewhere used unit of \( \text{Pa} \cdot \text{s} \).
			  
			  In the following table, not all entries describe the gaseous state, and wherever the gas will have turned back into liquid, the original table value was replaced by -1 to allow for a quick check of state change.
			  
			  \begin{table}[ht]
			  \centering
			  \caption{Dynamic Viscosity Lookup Table}
			  \begin{tabular}{|c|c|c|c|c|c|c|c|}
			  \hline
			  Pressure (Pa) & 6900 & 13800 & 34500 & 68900 & 138000 & 345000 & 690000 \\
			  \hline
			  727.15 & 0.028 & 0.028 & 0.028 & 0.028 & 0.028 & 0.028 & 0.028 \\
			  700.15 & 0.026 & 0.026 & 0.026 & 0.026 & 0.026 & 0.026 & 0.027 \\
			  672.15 & 0.024 & 0.025 & 0.025 & 0.025 & 0.025 & 0.025 & 0.025 \\
			  644.15 & 0.023 & 0.023 & 0.023 & 0.023 & 0.023 & 0.023 & 0.023 \\
			  616.15 & 0.022 & 0.022 & 0.022 & 0.022 & 0.022 & 0.022 & 0.022 \\
			  589.15 & 0.021 & 0.021 & 0.021 & 0.021 & 0.021 & 0.021 & 0.021 \\
			  561.15 & 0.020 & 0.020 & 0.020 & 0.020 & 0.020 & 0.020 & 0.020 \\
			  533.15 & 0.019 & 0.019 & 0.019 & 0.019 & 0.019 & 0.019 & 0.019 \\
			  505.15 & 0.018 & 0.018 & 0.018 & 0.018 & 0.017 & 0.017 & 0.017 \\
			  477.15 & 0.016 & 0.016 & 0.016 & 0.016 & 0.016 & 0.016 & 0.016 \\
			  450.15 & 0.015 & 0.015 & 0.015 & 0.015 & 0.015 & 0.015 & 0.015 \\
			  422.15 & 0.014 & 0.014 & 0.014 & 0.014 & 0.014 & 0.014 & -1 \\
			  394.15 & 0.013 & 0.013 & 0.013 & 0.013 & 0.013 & -1 & -1 \\
			  366.45 & 0.012 & 0.012 & 0.012 & 0.012 & -1 & -1 & -1 \\
			  338.75 & 0.0011 & 0.0011 & -1 & -1 & -1 & -1 & -1 \\
			  \hline
			  \end{tabular}
			  \end{table}
			-
			-
		- Nozzle Flow Characterization
			- Isentropic relations
			  
			  The Mach number at any location in the nozzle is related to its area ratio with the throat area by:
			  $$\frac{A}{A_t}=\frac{1}{\mathrm{Ma}}\left[1+\left(\frac{\gamma-1}{\gamma+1}\right)\left(\mathrm{Ma}^2-1\right)\right]^{(\gamma+1) /[2(\gamma-1)]}$$
			  
			  This equation is used to find the Mach number at the exit given the fixed expansion ratio \(A_e / A_t\) for a given design. This Mach number is further used in the following isentropic relation to calculate the temperature and density at the exit.
			  
			  $$ \frac{\rho_e}{\rho_c}=\left(\frac{T_e}{T_c}\right)^{1 /(\gamma-1)}=\left[1+\frac{1}{2}(\gamma-1) \mathrm{Ma_e}^2\right]^{-1 /(\gamma-1)}$$
			  
			  The pressure at the exit is calculated using the following relationship between the pressure ratio \(p_e / p_c\) and the expansion ratio
			  
			  $$\frac{\mathrm{A}_{\mathrm{e}}}{\mathrm{A}_{\mathrm{t}}}=\frac{\Gamma}{\sqrt{\frac{2 \gamma}{\gamma-1} \cdot\left(\frac{\mathrm{p}_{\mathrm{e}}}{\mathrm{p}_{\mathrm{c}}}\right)^{\left(\frac{2}{\gamma}\right)}\left(1-\left(\frac{\mathrm{p}_{\mathrm{e}}}{\mathrm{p}_{\mathrm{c}}}\right)^{\left(\frac{\gamma-1}{\gamma}\right)}\right)}}$$
			  
			  where \(\Gamma\) is the Vanderkerck-hove function:
			  
			  $$\Gamma=\sqrt{\gamma} \cdot\left(\frac{2}{\gamma+1}\right)^{\left(\frac{\gamma+1}{2(\gamma-1)}\right)}$$
			  
			  It is impossible to analytically solve the relation between the expansion/area ratio and pressure ratio for the pressure ratio, so instead, an inverse solution optimizer was used.
			- The bulk of the equations in this section were taken from [[@Analytical Relations for Performance Characterization of CD Micro-nozzles]] , which discusses the performance of CD micronozzles. The final output of this model is the "true" thrust i.e. the ideal thrust corrected with various loss factors.
			- Divergence loss
			  
			  Divergence losses occur when the exit half angle of a nozzle is greater than 0°, causing the gases ejected from the nozzle to deviate from the direction of thrust. This deviation introduces momentum components that are perpendicular to the thrust vector. However, due to the symmetry of the nozzle, these perpendicular momentum components cancel each other out, resulting in no thrust misalignment. Nevertheless, they still contribute to a loss in thrust because not all of the momentum is effectively utilized to propel the spacecraft forward.
			  
			  To quantify this loss, we use the divergence thrust correction factor, denoted as \(\epsilon_{div}\). This factor is calculated using the equation:
			  
			  \(\epsilon_{div} = 1 - \frac{1 - \cos(\alpha)}{2}\)
			  
			  In this equation, \(\alpha\) represents the exit half angle of the nozzle. The value of \(\epsilon_{div}\) depends solely on the exit half angle and affects both large and small nozzles.
			- Boundary Layer Losses
			  
			  The boundary layer is a thin layer of fluid that forms along the wall of a nozzle due to the effects of viscous flow. This phenomenon causes the flow velocity to decrease near the walls and deflect the main flow. In micro-nozzles, the impact of boundary layer losses is more pronounced due to their low Reynolds number, which leads to higher skin friction coefficients and larger boundary layers.
			  
			  To accurately predict performance losses in micro-nozzles, it is crucial to characterize the boundary layer. One approach is to use a simplified model based on flat plate boundary layer solutions, which can be applied to linear convergent-divergent micro-nozzles.
			  
			  The flat-plate Reynolds number at the exit (\(R e_x\)) is defined as the ratio of the product of the exit velocity (\(u_e\)) and the distance from the nozzle entrance (\(x\)) to the dynamic viscosity (\(\mu\)) of the fluid:
			  
			  \[R e_x=\frac{u_e x}{\mu}\]
			  
			  For incompressible, laminar flow, the skin friction coefficient (\(c_{f x}\)) can be calculated using the following equation:
			  
			  \[c_{f x}=\frac{0.664}{\sqrt{R e_x}}\]
			  
			  The skin friction coefficient is an important parameter that quantifies the frictional forces acting on the fluid within the boundary layer.
			- Correcting for compressibility
			  
			  The Reference Temperature Approach is a method used to correct the skin friction coefficient in supersonic flow. In the previous section, we discussed a method for predicting boundary layer properties assuming incompressible flow. However, this assumption is no longer valid when the flow becomes supersonic.
			  
			  To account for compressibility effects, the compressible skin friction coefficient is calculated using the Reference Temperature Approach. This approach involves using an average temperature across the boundary layer to correct the skin friction coefficient.
			  
			  The equation for the compressible skin friction coefficient is given by:
			  
			  \[c_f=c_{f, i}\left(\frac{T_w / T_0+1}{2}+0.22 \frac{\gamma-1}{2} M^2\right)^{-0.6}\]
			  
			  In this equation, \(c_f\) represents the compressible skin friction coefficient, \(c_{f, i}\) is the skin friction coefficient assuming incompressible flow, \(T_w\) is the wall temperature (which remains constant along the entire VLM), \(T_0\) is the stagnation temperature at the point where the skin friction coefficient is determined, \(\gamma\) is the specific heat ratio, and \(M\) is the Mach number.
			  
			  The stagnation temperature (\(T_0\)) refers to the temperature of the vapor immediately before entering the nozzle, which is the same as the previously calculated chamber temperature. By incorporating the average temperature across the boundary layer, the Reference Temperature Approach provides a more accurate estimation of the skin friction coefficient in supersonic flow conditions.
			- The momentum thickness (\(\theta_x\)) is a measure of the thickness of the boundary layer and can be calculated by multiplying the skin friction coefficient (\(c_{f x}\)) by the distance from the nozzle throat (\(x\)):
			  
			  \[\theta_x=c_{f x} \cdot x\]
			  
			  The displacement thickness (\(\delta^*\)) represents the amount by which the flow is displaced by the boundary layer. It can be calculated using the following equation:
			  
			  \[\delta^*=2.59036 \cdot \theta_x\]
			  
			  To optimize the design of the nozzle, the angle of the divergent section should be carefully chosen to balance the displacement thickness and divergence losses.
			  
			  The true area ratio, or expansion ratio, of the nozzle (\(\left(\frac{A_e}{A_t}\right)_{t r u e}\)) can be determined using the following equation:
			  
			  $$\left(\frac{A_e}{A_t}\right)_{t r u e}=\frac{\left(R_e-\delta^*\right)^2}{R_t^2}$$
			  
			  Here, \(R_t\) represents the throat radius and \(R_e\) denotes the exit radius.
			  
			  It is important to note that the assumptions underlying this boundary layer solution include laminar and attached flow, as well as the assumption that the boundary layer starts developing at the throat and increases in size until reaching the nozzle exit. These assumptions provide a simplified model for analyzing boundary layer losses in micro-nozzles.
			- Momentum Losses
			  
			  The presence of a boundary layer in addition to the modification of effective nozzle geometry leads to momentum losses in the flow. These losses occur as the flow loses momentum within the boundary layer. To account for this, the thrust loss due to momentum can be calculated using the equation:
			  
			  \(\Delta F_{\text {momentum }}=\left(\rho_e \cdot u_e \cdot\left(2 \pi R_e\right) \cdot \theta_e\right) \cdot u_e\)
			- True pressure ratio
			  
			  The true area ratio found earlier leads to a different exit pressure than that predicted by IRT, and this true pressure ratio between the exit pressure \(p_e\) and chamber pressure \(p_c\) can be found, as before, iteratively using the relation between the pressure ratio and expansion ratio.
			- The ideal thrust represents the maximum achievable thrust under ideal conditions. \(F_{ideal}\) can be calculated using the following equation:
			  
			  \[F_{i deal}=\dot{m} \cdot u_{e q}\]
			  
			  where \(u_{eq}\) is the (equivalent) exit pressure. The ambient pressure is assumed to be very small given the VLM's final application in the vacuum of space, and generally, the pressure term can be neglected in micropropulsion systems, which was done here as well. Some expansion and rearrangement using the definition of the exit velocity yields:
			  
			  $$
			  F_{ideal} = \dot{m} \cdot \sqrt{2 \cdot \frac{\gamma}{\gamma-1} \cdot R_s \cdot \mathrm{T}_{\mathrm{c}} \cdot\left(1-\left(\frac{\mathrm{p}_{\mathrm{e}}}{\mathrm{p}_{\mathrm{c}}}\right)^{\left(\frac{\gamma-1}{\gamma}\right)}\right)}
			  $$
			- Discharge coefficient \(C_D\)
			  
			  There is only one missing variable to find the true thrust: the true mass flow. The ratio of the real and ideal mass flow in the throat is called the discharge coefficient.
			  
			  Tang and Fenn (1978) derived an expression to calculate the discharge coefficient for choked axisymmetric nozzles with a circular cross-section. The expression takes into account the effect of the boundary layer in reducing the effective nozzle throat area. The expression by Tang and Fenn was derived for adiabatic flow of cold gases through smooth circular nozzles, which is exactly our case. These effects are more significant for throat Reynolds numbers under 100,000. The equation for the discharge coefficient is given as:
			  
			  $$C_D=1-\left(\frac{\gamma+1}{2}\right)^{3/4}\left(\frac{-2.128}{\gamma+1}+3.266\right) R^{-0.5}+9.428 \frac{(\gamma-1)(\gamma+2)}{(\gamma+1)^{0.5}} R^{-1} =\frac{\dot{m}_{\text {true }}}{\dot{m}_{ideal}}$$
			  
			  where \(C_D\) is the discharge coefficient and \(R\) is the modified throat Reynolds number, which in our case for a circular throat, is just the original throat Reynolds number.
			- True Thrust
			  
			  The resulting aggregate thrust loss is calculated by combining the divergence loss, momentum loss, and corrected exit pressure. The true thrust, estimated using this methodology, is given by:
			  
			  $$F_{\text {true }}=\dot{m}_{true} \cdot \epsilon_{\text {div }} \cdot \sqrt{2 \cdot \frac{\gamma}{\gamma-1} \cdot R_s \cdot \mathrm{T}_{\mathrm{c}} \cdot\left(1-\left(\frac{\mathrm{p}_{\mathrm{e}}}{\mathrm{p}_{\mathrm{c}}}\right)_{\text {true }}^{\frac{\gamma-1}{\gamma}}\right)}-\Delta F_{\text {momentum }}$$
		- Nozzle Performance Evaluation
			- Once the true thrust of the nozzle has been found by characterizing the flow within, several different metrics can be calculated to evaluate the performance of the nozzle. The majority of these equations were taken from [[@Simplified Modelling of Aerospike Micro-nozzles]], which discusses the performance of aerospike micronozzles, although many of the relations were originally derived for CD nozzles and then repurposed for aerospikes, keeping them valid for our case.
			- Thrust efficiency, denoted as \(\eta_F\), is a measure of how effectively a propulsion system converts the input power into thrust. It is defined as the ratio of the measured thrust, \(F_{\text{meas}}\), to the ideal thrust, \(F_{ideal}\). By dividing the measured thrust, \(F_{\text{true}}\), by the ideal thrust, \(F_{ideal}\), we obtain the thrust efficiency, \(\eta_F\):
			  
			  $$\eta_F = \frac{F_{\text{true}}}{F_{ideal}}$$
			  
			  The thrust efficiency provides a quantitative measure of how well the propulsion system is performing in converting the input power into useful thrust. A higher thrust efficiency indicates a more efficient propulsion system, while a lower thrust efficiency suggests that a significant portion of the input power is being wasted or lost in the conversion process.
			- Specific Impulse Efficiency
			  
			  Specific impulse efficiency (\(\eta_{I_{sp}}\)) is a parameter used to evaluate the performance of rocket engines. It quantifies the efficiency of a rocket engine in converting propellant mass flow rate into thrust.
			  
			  The specific impulse (\(I_{sp}\)) is a measure of how effectively a rocket engine utilizes its propellant. It is defined as the thrust generated per unit of propellant mass flow rate. The specific impulse efficiency compares the measured specific impulse (\(I_{sp_{true}}\)) of an engine to the specific impulse (\(I_{sp_{ideal}}\)) that would be achieved by an ideal engine operating under the same conditions.
			  
			  The ideal specific impulse (\(I_{sp_{1D}}\)) is calculated using the thrust (\(F_{1D}\)) generated by the engine, the propellant mass flow rate (\(\dot{m}_{1D}\)), and the standard acceleration due to gravity (\(g_0\)). It represents the maximum specific impulse achievable by an engine with perfect efficiency.
			  
			  $$
			  I_{sp_{ideal}} = \frac{F_{ideal}}{\dot{m}_{ideal} \cdot g_0}
			  $$
			  
			  On the other hand, the measured specific impulse (\(I_{sp_{meas}}\)) is determined experimentally by measuring the thrust (\(F_{meas}\)) and the propellant mass flow rate (\(\dot{m}_{meas}\)) of the engine. It represents the actual specific impulse achieved by the engine in real-world conditions.
			  
			  $$
			  I_{sp_{true}} = \frac{F_{true}}{\dot{m}_{true} \cdot g_0}
			  $$
			  
			  The specific impulse efficiency (\(\eta_{I_{sp}}\)) is then calculated by dividing the measured specific impulse by the ideal specific impulse:
			  
			  $$
			  \eta_{I_{sp}} = \frac{I_{sp_{meas}}}{I_{sp_{ideal}}}
			  $$
			  
			  This efficiency parameter provides insight into how well a rocket engine performs relative to its theoretical maximum performance. A higher specific impulse efficiency indicates a more efficient engine, as it is able to achieve a larger fraction of the ideal specific impulse.
			- Thrust per power
			  
			  The final evaluation variable is the amount of thrust generated for a given input power, expressed as
			  
			  $$\eta_{F/P} = \frac{F_{true}}{P_{input}} \ [\text{mN/W}]$$
- Methodology
	- In order to design a next-generation VLM based on the theory presented in the literature review, a comprehensive simulation of the VLM's performance was created. This calculation was performed for a large number of design parameters within a feasible range, the values for which were sampled using Latin Hypercube Sampling in order to efficiently and comprehensively cover the entire design space. The best designs were evaluated using a multi-objective composite score, equally weighting the main performance indicators of the VLM. The best designs according to this score were then subjected to sensitivity analyses and further parameter sweeps to ascertain individual inputs' effect on the system performance.
	- VLM Performance Simulation
	  In order to design a next-generation VLM based on the theoretical background gleaned from the above sources, a comprehensive characterization of the behavior and performance of the VLM was created. The equations used are detailed in the previous section, and the general order of the procedure is:
	  
	  \begin{enumerate}
	  \item Size the VLM
	  \item Calculate the liquid flow conditions in the heating chamber
	  \item Calculate the gaseous flow conditions in the heating chamber
	  \item Find the throat conditions
	  \item Find the exit flow conditions
	  \item Correct the nozzle flow conditions with error terms and find the true thrust
	  \item Calculate all remaining evaluation parameters
	  \end{enumerate}
	  
	  The full code for the simulation can be found in the GitHub repository for this project.
	  
	  Interspersed in the main calculations are a number of sanity checks, preferably performed as early in the calculations as possible, to exclude any parameter combinations that are not physically realistic. These include:
	  
	  \begin{itemize}
	  \item Ensuring the exit radius is greater than the throat radius
	  \item Keeping the exit Mach number between 1 and 5
	  \item Asserting the positive sign of all non-negative variables
	  \item Ensuring the steam has not turned back into water at the exit due to low temperatures
	  \item Finding the existence of solutions for mass flow and chamber temperature combinations for the input power and pressure
	  \end{itemize}
	- Optimization Procedure
		- **Design and Evaluation Variables:**
		  The design variables include nine key parameters:
		  
		  Chip Temperature
		  Tank Pressure
		  Throat Radius
		  Nozzle Exit Radius
		  Number of Elements (Integer)
		  Number of Channels (Integer)
		  Chamber Depth
		  Input Power
		  Nozzle Length
		  
		  The evaluation parameters are as follows:
		  
		  Specific Impulse Efficiency
		  Thrust Efficiency
		  Nusselt Number
		  Discharge Coefficient
		  Reynolds Number (Chamber)
		  Mass Flow Error
		  Chamber Length
		  Chamber Width
		  Thrust per Power
		  
		  Table X shows the input parameter ranges used for the simulation.
		  
		  \begin{table}[htbp]
		    \centering
		    \caption{Input Ranges for Optimization}
		    \label{tab:input_ranges}
		    \begin{tabular}{|c|c|c|}
		        \hline
		        \textbf{Parameter} & \textbf{Range} & \textbf{Unit} \\
		        \hline
		        Chip Temperature & $(400, 600)$ & K \\
		        Tank Pressure & $(100000, 500000)$ & Pa \\
		        Throat Radius & $(1 \times 10^{-2}, 1 \times 10^{-1})$ & mm \\
		        Nozzle Exit Radius & $(1 \times 10^{-2}, 1 \times 10^{-1})$ & mm \\
		        Number of Elements & $(5, 20)$ & \\
		        Number of Channels & $(5, 15)$ & \\
		        Chamber Depth & $(0.01, 0.1)$ & mm \\
		        Input Power & $(0.5, 10)$ & W \\
		        Nozzle Length & $(0.1, 1)$ & mm \\
		        \hline
		    \end{tabular}
		  \end{table}
		- **Latin Hypercube Sampling (LHS):**
		  Latin Hypercube Sampling is employed to efficiently explore the multidimensional design parameter space. This method ensures a comprehensive yet balanced sampling by dividing each variable's range into equal intervals and selecting a unique value from each interval. The use of LHS reduces the risk of missing critical regions of the design space and provides a representative set of designs for subsequent evaluation.
		- **Multi-Objective Evaluation:**
		  Each design generated by LHS, after calculating all the evaluation parameters, undergoes a multi-objective evaluation. The various objectives are combined using a weighted sum approach into a single score. In order to make the parameters comparable between each other, they were normalized, mapping their range onto the $[0,1]$ domain. Some of these variables are supposed to be minimized, like the chamber length and width, and the mass flow error - these were made negative to reflect their influence on the score.
		  
		  \begin{table}[htbp]
		      \centering
		      \caption{Weight Coefficients for Performance Metrics}
		      \label{tab:weight_coefficients}
		      \begin{tabular}{|c|c|}
		          \hline
		          \textbf{Performance Metric} & \textbf{Weight Coefficient} \\
		          \hline
		          Specific Impulse Efficiency & 0.1 \\
		          Thrust Efficiency & 0.2 \\
		          Nusselt Number & 0.05 \\
		          Discharge Coefficient & 0.2 \\
		          Reynolds Number (Chamber) & 0.025 \\
		          Mass Flow Error & 0.025 \\
		          Chamber Length & 0.1 \\
		          Chamber Width & 0.1 \\
		          Thrust per Power & 0.2 \\
		          \hline
		      \end{tabular}
		  \end{table}
- Results
	- An initial simulation with one million samples and the input parameter ranges reported above was performed, but due to the relationship between mass flow, heating power, pressure and chamber temperature, the vast majority of samples did not yield a physically meaningful result, with another portion having the steam condense at the exit and thus yield an error as well. Out of one million, only around 25 thousand simulations were successfully completed.
	  
	  In all following scatter plots, the top 10 percent in terms of the combined evaluation score as described above are plotted in blue, while the bottom 90 percent are plotted in red.
	- Optimized Design
	  
	  Taking the design with the highest combined evaluation score out of all 25 thousand yielded the following design:
	  
	  \begin{table}[htbp]
	      \centering
	      \caption{Best Design}
	      \label{tab:best_design}
	      \begin{tabular}{|c|c|c|}
	          \hline
	          \textbf{Parameter} & \textbf{Value} & \textbf{Unit} \\
	          \hline
	          Specific Impulse Efficiency & 0.990 & \\
	          Thrust Efficiency & 0.935 & \\
	          Nusselt Number & 0.0009897 & \\
	          Discharge Coefficient & 0.944 & \\
	          Reynolds Number (Chamber) & 3.03 & \\
	          Mass Flow Error & -1.73 & mg/s \\
	          Chamber Length & 3.2 & mm \\
	          Chamber Width & 1.06 & mm \\
	          Thrust per Power & 0.417 & mN \\
	          Mass Flow & $3.14 $ & mg/s \\
	          Chamber Temperature & 510.5 & K \\
	          Combined Evaluation Parameter & 0.654 & \\
	          Input Power & 9.21 & W \\
	          Tank Pressure & 3.275 & bar \\
	          Nozzle Exit Radius & $9.76 \times 10^{-2}$ & mm \\
	          Throat Radius & $3.14 \times 10^{-2}$ & mm \\
	          Number of Elements & 5.00 & \\
	          Number of Channels & 5.00 & \\
	          Chamber Depth & 0.2158 & mm \\
	          Chip Temperature & 537.5 & K \\
	          Nozzle Length & 8.13 & mm \\
	          \hline
	      \end{tabular}
	  \end{table}
	- Sensitivity Analysis
	  
	  An attempt at a sensitivity analysis was made by fixing all input parameters to those of the best design and sweeping a given parameter over its design range, but because of the narrow range of possible solutions for the mass flow and heating power equation system, rarely any feasible solutions were found using this procedure.
	- Recalculation for Mass Flow vs. Power relationship
	  
	  However, an interesting result arose from the initial one million sample run, illustrating the narrow relationship between the mass flow and heating power.
	  
	  INSERT MASS FLOW X POWER GRAPH
	  
	  INSERT TANK PRESSURE X CHAMBER TEMPERATURE GRAPH
	  
	  This revealed the real constraints on physically real solutions for this equation system. These relations were fitted through visual analysis:
	  
	  Pressure x Chamber Temperature relation
	  
	  $$
	  \begin{cases}
	    T_c \geq425 & \text{if } 1 \ \text{bar} < p_c < 1.3 \ \text{bar}\\
	    T_c \geq 1.8 \cdot \log{p_c - 130000} + 446 & \text{if }1.3 \ \text{bar} < p_c < 2.6 \ \text{bar} \\
	   T_c \geq 2.8 \cdot \log{p_c - 260000} + 475 & \text{if } 2.6 \ \text{bar} < p_c < 5 \ \text{bar}
	  \end{cases}
	  $$
	  
	  Mass Flow x Heating Power Relation (in mg/s)
	  
	  $$ 0.342 \cdot P_{heat} - 0.175  \leq \dot{m} \leq 0.3947 \cdot P_{heat} -0.2 $$
	  
	  These constraints were added to the two equation system solver to constrain the search domain for a given calculation. Then, the existence of mass flow and temperature solutions and gaseous exit phase check were added as conditions for the generation of a sample using LHS, raising the successful simulation rate from 2.5 to 50 percent. A new set of one hundred thousand samples was generated to have 50,000 for a new optimization attempt.
	  
	  Of these, X thousand were successfully completed, yielding a new dataset with hopefully a more precise look into the domain of interest.
	- Optimized Design
- Conclusion
- Discussion