- References and Literature Review notes
	- Reference school reports
		- [[@Analytical Relations for Performance Characterization of CD Micro-nozzles]]
		  collapsed:: true
			- {{embed [[hls__Micropropulsion project_conventional nozzles]]}}
		- [[@Micropropulsion course Numerical analysis of wavy microchannels employed in a Vaporizing Liquid Micro-resistojet thruster]]
		  collapsed:: true
			- {{embed [[hls__Bianchi - Micropropulsion course Numerical analysis of wavy]]}}
		- [[@Simplified Modelling of Aerospike Micro-nozzles]]
		  collapsed:: true
			- Summary:
			  The text discusses the performance of micronozzles under low Reynolds numbers. Three performance parameters, namely thrust efficiency, discharge coefficient, and specific impulse efficiency, are used to study their performance. The theoretical values of these parameters are calculated using the principles of Ideal Rocket Theory. The text also mentions the momentum loss caused by skin friction in the nozzle walls, which reduces the thrust of the propulsion system. The effect of viscous forces on the nozzle quality is estimated using an expression derived by Spisz. The text further discusses the calculation of thrust efficiency and discharge coefficient using different equations. The discharge coefficient is calculated considering the effect of the boundary layer on the nozzle throat area. The values of effective and geometric area ratio for different Reynolds numbers are provided in a table. The discharge coefficient is assumed to be the ratio between effective and geometric area ratio. The text concludes with an equation that represents the best fit for the given values of the ratio between effective and geometric area ratio.
			- {{embed [[hls__Micropropulsion project_aerospike nozzles]]}}
	- Reference Journal Articles
		- [[@Topology Optimization of Heating Chamber of Vaporizing Liquid Microthrusters]]
		  collapsed:: true
			- {{embed [[hls__Silva et al. - TOPOLOGY OPTIMIZATION OF HEATING CHAMBER OF VAPORI]]}}
		- [[@A Comprehensive Model for Control of Vaporizing Liquid Microthrusters]]
		  collapsed:: true
			- The important parameters to be considered in the design trade-off are size, wall temperature, and pressure losses. The wavy microchannel geometry improves convective heat transfer due to boundary layer thinning and the formation of Dean vortices. The Nusselt number is used to indicate the ratio between the heat transferred via convection and the heat transferred via conduction. A higher Nusselt number means having lower wall temperatures, which is critical in Cubesats where available power is often limited. Future work should concentrate on the two sections of the flow that have not been simulated in this work: boiling and vapor.
			  id:: 64a59f7e-d25e-45fe-8227-81c8d3b66335
			- ## Main Equations 
			  The main equations used for modeling heat transfer in the heating chamber are as follows:
			  
			  1. Nozzle model:
			  The mass flow rate at the nozzle, \(\dot{m}_3\), is calculated using the ideal rocket conditions. The mass flow rate equation is given by:
			  \[
			  \dot{m}_3 = \sqrt{\frac{2 \gamma}{R}} \frac{A_t}{A_e} p_1 \sqrt{\frac{\gamma}{R T_1}} \left(1 - \left(\frac{p_0}{p_1}\right)^{\frac{\gamma - 1}{\gamma}}\right)
			  \]
			  where \(\gamma\) is the specific heat ratio, \(R\) is the specific gas constant, \(A_t\) is the throat area, \(A_e\) is the exit area, \(p_1\) is the chamber pressure, \(T_1\) is the chamber temperature, and \(p_0\) is the ambient pressure.
			  
			  2. Vaporization model:
			  The average volume of vapor, \(V_{av}\), is calculated as a function of the thruster temperature and pressure:
			  \[
			  V_{av} = a_T T_n + a_p p_1 + b
			  \]
			  where \(a_T\), \(a_p\), and \(b\) are parameters of the linear regression, and \(T_n\) is the temperature of the chip measured around the nozzle.
			  
			  3. Time derivative of volume:
			  The time derivative of the volume, \(\dot{V}\), is assumed to be a first-order linear system:
			  \[
			  \dot{V} = A(V_{av} - V)
			  \]
			  
			  4. Vaporization rate:
			  The vaporization rate, \(\dot{m}_2\), is calculated as the difference between the liquid flow rate, \(\dot{m}_1\), and the time derivative of volume multiplied by the liquid density, \(\rho_l\):
			  \[
			  \dot{m}_2 = \dot{m}_1 - \dot{V} \rho_l
			  \]
			  
			  5. Pressure model:
			  The pressure inside the chamber, \(p\), is calculated using the ideal gas law:
			  \[
			  p = \frac{1}{\alpha_2} \left(\frac{m R_s}{V} - \beta_2\right)
			  \]
			  where \(\alpha_2\) and \(\beta_2\) are coefficients obtained from a linear approximation.
			  
			  6. Chip temperature model:
			  The temperature of the thruster, \(T\), is modeled as a linear first-order system with the applied power, \(P\), as the input. The Laplace transfer function of the power-temperature system is given by:
			  \[
			  \frac{T(s)}{P(s)} = \frac{K}{s + \frac{1}{\tau}}
			  \]
			  where \(\tau\) and \(K\) are experimentally estimated parameters.
			  
			  7. Resistance model:
			  The change in resistance, \(R\), due to temperature changes is described by the equation:
			  \[
			  R = \alpha R_0 (T - T_0) + R_0
			  \]
			  where \(\alpha\) is the temperature coefficient of resistance, \(R_0\) is the resistance measured at temperature \(T_0\), and \(T\) is the current temperature.
			- ## Main assumptions 
			  The model makes several assumptions and uses equations to describe heat transfer in the heating chamber. Here are the key assumptions and equations:
			  
			  1. Nozzle Model:
			  The temperature of the gas is assumed to be the saturation temperature.
			  The temperature of the vapor can be calculated based on the pressure using the Antoine equation.
			  The mass flow rate through the nozzle is given by an equation, which can be multiplied by a discharge coefficient to account for non-ideal conditions.
			  
			  2. Vaporization Model:
			  The average volume of vapor is expressed as a function of the temperature and pressure.
			  The time derivative of the volume is assumed to follow a first-order linear system.
			  The vaporization rate is calculated based on the mass flow rate of the liquid and the rate of change of volume.
			  
			  3. Pressure Model:
			  The ideal gas law is used to relate pressure, temperature, volume, and mass of gas.
			  The term "p/T" is approximated by a linear relation, resulting in a simplified equation for pressure.
			  
			  4. Chip Temperature Model:
			  The temperature of the thruster is modeled as a linear first-order system with the applied power as the input.
			  The Laplace transfer function is used to describe the power-temperature relationship.
			  The change in resistance due to temperature changes is described by an equation involving the resistance at a reference temperature and a temperature coefficient.
			  
			  These assumptions and equations provide a framework for understanding heat transfer in the heating chamber of the model.
			- {{embed [[hls__Silva et al. - 2019 - A Comprehensive Model for Control of Vaporizing Li]]}}
		- [[@State Space Modeling of Fluid Flow for Thrust Control in MEMS-Based Micropropulsion]]
		  collapsed:: true
			- {{embed [[hls__Ref4]]}}
		- [[@Vaporizing Liquid Microthrusters with integrated heaters and temperature measurement]]
		  collapsed:: true
			- {{embed [[hls__Silva et al. - 2017 - Vaporizing Liquid Microthrusters with integrated h]]}}
	- Supplementary Materials
		- [[@Simplified Equations for Saturated Steam Properties for Simulation Purpose]]
- Assignment
	- Tasks
		- Carefully analyse the models proposed in the previous Micropropulsion projects for the heating
		  chamber and the micro-nozzle, and perform a short literature study to define which other
		  simplified analytical models are available to characterize heat transfer and micro-nozzle
		  performance in a device with similar geometry and size as the VLM thruster
		- Write a set of simplified equations to model the full performance of a VLM thruster with
		  serpentine channels, based on suitable modelling assumptions
		- Use these simplified equations to propose a new-generation design for the VLM thruster,
		  focusing in particular on the dimensioning of all thruster features (inlet section, micro-channels,
		  nozzle) and the consequent expected performance of the thruster
	- Research questions
		- What is a suitable set of simplified equations and assumptions for modelling the heating
		  chamber and the micro-nozzle of a VLM micro-resistojet?
		- What is the most promising design for the new generation of VLM micro-resistojet thrusters
		  to be manufactured and tested by TU Delft?