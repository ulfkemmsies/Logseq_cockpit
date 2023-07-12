id:: 6466ff58-6781-4cf0-bfb6-f8c0b0216572

	- The thrust is simply the force produced by the rocket, which can be calculated using the following equation:
	  hl-page:: 7
	  ls-type:: annotation
	  hl-color:: yellow
	  \(F_T=\dot{m} \cdot v_e+\left(p_e-p_a\right) \cdot A_e=\dot{m} \cdot v_{e g}\)
	- In order to write the thrust equation in a more compact way, an equivalent jet velocity is usually defined, indicated by v eq in equation (1.1), which accounts for both the momentum and pressure terms in the equation.
	  ls-type:: annotation
	  hl-page:: 7
	  hl-color:: yellow
	- For a negligible mass change:
	  \(\Delta P = F \cdot t\)
	  \(\Delta P = m \cdot \Delta V\)
	- The specific impulse is defined as the ratio of the total impulse generated by the rocket (thrust integrated over the burn time), to the total weight of propellant used to generate it.
	  hl-page:: 7
	  ls-type:: annotation
	  hl-color:: yellow
	  \(I_{s p}=\frac{\nu_{e q}}{g_0}\)
	- The Delta-V is the ideal velocity change experienced by the spacecraft in which the propulsion system is installed
	  hl-page:: 7
	  ls-type:: annotation
	  hl-color:: yellow
	  \(\Delta v=v_{eq} \cdot \ln \left(\frac{M_0}{M_0-M_P}\right)\)
	- However, this is only true under a number of assumptions: no external forces acting on the spacecraft (such as gravity or atmospheric drag); equivalent jet velocity constant over time; propellant expelled in a direction exactly opposite to the flight direction. When at least one of these assumptions is not met, the Delta-V calculated by means of the rocket equation is no longer the actual velocity change of the spacecraft
	  ls-type:: annotation
	  hl-page:: 8
	  hl-color:: yellow
	- [[GPT Generated Flashcards]]
		- What is the thrust equation in rocket propulsion? #card
		  id:: 83c22613-1da9-45c5-a79b-63f99573a355
			- \(F_T=\dot{m} \cdot v_e+\left(p_e-p_a\right) \cdot A_e=\dot{m} \cdot v_{e g}\)
		- For a satellite with negligible mass change, the following relation concerning momentum changes holds: #card
		  id:: 6469ddb7-1f29-44f6-ac10-b1a4722f66e4
			- \(\Delta P = F_T \cdot t_b = M_0 \cdot \Delta V\)
		- How is the equivalent jet velocity (v eq) used in the thrust equation? #card
		  id:: ab948c77-e9c8-4d77-9390-a5b6745b9b86
			- It accounts for both the momentum and pressure terms.
		- What equation represents the specific impulse? #card
		  id:: 31c7bfc3-6a0e-4b42-be6a-b458a378189a
			- \(I_{s p}=\frac{\nu_{e q}}{g_0}\)
		- Which velocity change does Delta-V represent? #card
		  id:: 28c10b2e-4ef1-452e-946f-5e12635f8f2b
			- The ideal velocity change experienced by the spacecraft.
		- What is the Delta-V equation? #card
		  id:: ba37d25d-9447-4c0f-88d1-f77e4ecd64f7
			- \(\Delta v=v_{e q} \cdot \ln \left(\frac{M_0}{M_0-M_P}\right)\)
		- Under what conditions is the Delta-V equation not accurate for the actual velocity change of the spacecraft? #card
		  id:: ded5607e-76eb-4b05-bec1-0c4f4ffae54d
			- When external forces act on the spacecraft, the equivalent jet velocity isn't constant, or the propellant isn't expelled in the opposite direction of flight.
	- it is important to find equations for three important parameters: the jet velocity, the mass flow rate and the propellant exhaust pressure. For systems based on thermal expansion of the propellant in a nozzle, simplified equations for these three parameters are provided by the so-called Ideal Rocket Theory. This theory is based on a number of simplifying assumptions for the flow in the nozzle, the most important of which are:
	  hl-page:: 8
	  ls-type:: annotation
	  hl-color:: red
	  hl-stamp:: 1683173847874
	  • The fluid flowing in the nozzle is a perfect, calorically ideal gas of constant homogeneous chemical composition;
	  • Flow is steady, isentropic, mono-dimensional, with purely axial velocity;
	  • No friction or other external forces act on the gas flowing in the nozzle. The nozzle is convergent-divergent, with an inlet section in which the flow is considered under stagnation conditions (negligible velocity), a throat section where the flow is sonic, and the exhaust section where the flow is typically highly supersonic.
	- Under the Ideal Rocket Theory assumptions, it is possible to derive the following equation for the jet velocity:
	  hl-page:: 8
	  ls-type:: annotation
	  hl-color:: red
	  \(v_e=\sqrt{\frac{2 \gamma}{\gamma-1} \cdot \frac{R_A}{M_W} \cdot T_C \cdot\left[1-\left(\frac{p_e}{p_C}\right)^{\frac{\gamma-1}{\gamma}}\right]}\)
	  where \(p_C\) and \(T_C\) are the pressure and temperature at the nozzle inlet (which is the combustion chamber, in chemical engines), \(R_A\) is the universal gas constant (= 8314 J/K*kmol), \(M_W\) and \(\gamma\) are the molecular mass and specific heat ratio of the gas flowing in the nozzle. This equation shows that higher jet velocity (thus, higher specific impulse) can be achieved by selecting a propellant that allows for higher chamber temperature and lower molecular mass of the gas flowing in the nozzle
	- The specific heat ratio of a gas, often denoted by the symbol γ (gamma), is the ratio of its specific heats at constant pressure and constant volume. It is a dimensionless quantity and is an important parameter in thermodynamics. For an ideal gas, the value of γ is constant and is equal to 1.4. However, for real gases, the value of γ can vary slightly with temperature and pressure.
	- For the mass flow rate, the following equation holds:
	  hl-page:: 8
	  ls-type:: annotation
	  hl-color:: red
	  \(\dot{m}=\frac{p_C \cdot A^*}{\sqrt{\frac{R_A}{M_W} \cdot T_C}} \cdot \sqrt{\gamma \cdot\left(\frac{1+\gamma}{2}\right)^{\frac{1+\gamma}{1-\gamma}}}\)
	  where $A^*$ is the nozzle throat area.
	- Finally, the following relationship holds between the area ratio Ae /A* and the pressure ratio p_C /p_e :
	  hl-page:: 8
	  ls-type:: annotation
	  hl-color:: red
	  \(\frac{A_{\varepsilon}}{A^*}=\frac{\sqrt{\gamma \cdot\left(\frac{1+\gamma}{2}\right)^{\frac{1+\gamma}{1-\gamma}}}}{\sqrt{\frac{2 \gamma}{\gamma-1} \cdot\left(\frac{p_{\varepsilon}}{p_C}\right)^{\frac{2}{\gamma}} \cdot\left[1-\left(\frac{p_{\varepsilon}}{p_C}\right)^{\frac{\gamma-1}{\gamma}}\right]}}\)
	- [[GPT Generated Flashcards]]
		- What are the three important parameters in micropropulsion systems? #card
		  id:: 7e2d26df-5e9d-427f-818f-6d3b4f089bba
			- Jet velocity, mass flow rate, and propellant exhaust pressure.
		- What theory provides simplified equations for the three important parameters in micropropulsion systems? #card
		  id:: 52015056-94a4-4963-8135-a1888c93d4ee
			- Ideal Rocket Theory.
		- What are the main assumptions of the Ideal Rocket Theory? #card
		  id:: c276d093-25c7-4706-a07a-f1636e4fed2e
			- The fluid is an ideal gas, flow is steady and isentropic, and no external forces act on the gas.
		- What is the equation for jet velocity under the Ideal Rocket Theory? #card
		  id:: 54dc8495-b751-412c-8b51-2eadb3b1e587
			- \(v_e=\sqrt{\frac{2 \gamma}{\gamma-1} \cdot \frac{R_A}{M_W} \cdot T_C \cdot\left[1-\left(\frac{p_e}{p_C}\right)^{\frac{\gamma-1}{\gamma}}\right]}\)
		- How can higher specific impulse be achieved in micropropulsion systems? #card
		  id:: c239e686-b1a9-48a6-ac04-9893bfab7651
			- By selecting a propellant with higher chamber temperature and lower molecular mass.
		- What is the specific heat ratio of an ideal gas? #card
		  id:: 4608284c-8deb-425b-b7e2-923cbdbb8de0
			- 1.4
		- What is the equation for mass flow rate under the Ideal Rocket Theory? #card
		  id:: 73bdda40-7961-4dda-b292-3ca53298198c
			- \(\dot{m}=\frac{p_C \cdot A^*}{\sqrt{\frac{R_A}{M_W} \cdot T_C}} \cdot \sqrt{\gamma \cdot\left(\frac{1+\gamma}{2}\right)^{\frac{1+\gamma}{1-\gamma}}}\)
		- What is the relationship between area ratio and pressure ratio in the Ideal Rocket Theory? #card
		  id:: 599dcc92-fef7-4fbf-8c01-ca37f42f5194
			- \(\frac{A_{\varepsilon}}{A^*}=\frac{\sqrt{\gamma \cdot\left(\frac{1+\gamma}{2}\right)^{\frac{1+\gamma}{1-\gamma}}}}{\sqrt{\frac{2 \gamma}{\gamma-1} \cdot\left(\frac{p_{\varepsilon}}{p_C}\right)^{\frac{2}{\gamma}} \cdot\left[1-\left(\frac{p_{\varepsilon}}{p_C}\right)^{\frac{\gamma-1}{\gamma}}\right]}}\)
	- A good indication of the parameters that play a major role in influencing the performance can however be obtained looking at the ideal equations for an ion thruster, where an electrostatic field between two grids is used to accelerate charged particles and generate the thrust
	  ls-type:: annotation
	  hl-page:: 9
	  hl-color:: green
	- A simplified equation for the jet velocity of the expelled ions can be written under the assumptions that only single-charged ions are present in the flow and that the kinetic energy acquired by an ion is exactly equal to the energy provided by the electrostatic field by which it is accelerated.
	  ls-type:: annotation
	  hl-page:: 9
	  hl-color:: green
	- The jet velocity can then be calculated as:
	  hl-page:: 9
	  ls-type:: annotation
	  hl-color:: green
	  \(v_e=\sqrt{\frac{2 e N_A V}{M_W}}\)
	  where V is the voltage difference of the electrostatic field between the two grids through which the ions are accelerated
	- The thrust produced by the ion thruster can be then written as:
	  hl-page:: 9
	  ls-type:: annotation
	  hl-color:: green
	  \(F_T=\frac{2 \pi \varepsilon_0}{9} \cdot V^2 \cdot n\left(\frac{D}{L}\right)^2\)
	  where n is the number of holes in the grids, L is the distance between the grids, D is the diameter of each hole in the grid, and \(\varepsilon_0\) is the permittivity of vacuum (= 8.8542∙10 -12 Farad/m)
	- [[GPT Generated Flashcards]]
		- What is the purpose of an ion thruster? #card
		  id:: 0df6d104-6633-4185-adec-e9cf7e4429dd
			- To accelerate charged particles and generate thrust using an electrostatic field.
		- In the simplified ion thruster equation for jet velocity, what are the assumptions made? #card
		  id:: 113fad8b-853c-4546-ab11-197474a6da90
			- Only single-charged ions are present and the kinetic energy of an ion equals the energy provided by the electrostatic field.
		- What is the formula to calculate the jet velocity of expelled ions in an ion thruster? #card
		  id:: 026106f8-1a74-4b6d-ac5f-a58415db80b9
			- \(\frac{1}{2} \cdot \frac{M_W}{N_A} \cdot v_e^2 = e \cdot V\)
		- In the jet velocity formula, what does V represent? #card
		  id:: b57e9050-cb6d-47fe-ac04-b4689c482f96
			- The voltage difference of the electrostatic field between the two grids.
		- What is the formula to calculate the thrust produced by the ion thruster? #card
		  id:: 5ed6451d-a4e0-4c48-879d-af7f17f04f5b
			- \(F_T=\frac{2 \pi \varepsilon_0}{9} \cdot V^2 \cdot n\left(\frac{D}{L}\right)^2\)
		- In the ion thruster thrust formula, what do $n$, $L$, $D$, and \(\varepsilon_0\) represent? #card
		  id:: 7c3ce7a6-b67c-4542-be9d-b48318f7c857
			- n is the number of grid holes, L is the distance between grids, D is each hole's diameter, and \(\varepsilon_0\) is the vacuum permittivity.
	- The specific impulse of an ion thruster can be calculated as:
	  hl-page:: 9
	  ls-type:: annotation
	  hl-color:: green
	  \(I_{s p}=\eta_{ion} \cdot \frac{v_e}{g_0}=\frac{\eta_{i o n}}{g_0} \cdot \sqrt{\frac{2 e N_A V}{M_W}}\)
	  where \(\eta_{ion}\) is the ionization efficiency, which accounts for the fact that not all propellant atoms are ionized and contribute in an effective way to generate thrust, and has a typical value in the order of 0.7-0.9 in most ion thrusters.
	- Finally, the thruster efficiency (ratio of kinetic power in the exhaust jet to input power provided to the thruster by the power plant) can be written as:
	  hl-page:: 9
	  ls-type:: annotation
	  hl-color:: green
	  \(\eta=\frac{\frac{1}{2} \frac{M_W}{N_A} v_e^2}{\frac{1}{2} \frac{M_W}{N_A} v_e^2+e_I+e_L}\)
	  Where \(e_I\) is the ionization potential (energy needed for ionizing one atom of propellant) and \(e_L\) is a term which accounts for all other energy losses in the system.
	- Differently to propulsion systems where the propellant is accelerated in a nozzle, the ideal propellant for an ion thruster is a fluid with high molecular mass and low ionization potential. In this way, less energy is needed to ionize a heavier atom and, thus, to produce a higher mass flow rate of ions.
	  hl-page:: 10
	  ls-type:: annotation
	  hl-color:: green
	- [[GPT Generated Flashcards]]
		- What is the specific impulse formula for an ion thruster? #card
		  id:: 0c508e2e-48a3-4d56-88d2-cca61566977a
			- \(I_{s p}=\eta_{ion} \cdot \frac{v_e}{g_0}=\frac{\eta_{i o n}}{g_0} \cdot \sqrt{\frac{2 e N_A V}{M_W}}\)
		- What does \(\eta_{ion}\) represent in the specific impulse formula for an ion thruster? #card
		  id:: a784cc9b-8350-4f64-ba2a-edfed9ed2ad9
			- Ionization efficiency
		- What are the typical values of ionization efficiency in most ion thrusters? #card
		  id:: b81afdb2-6353-4107-80a6-7b35e92372a4
			- 0.7-0.9
		- What is the formula for thruster efficiency? #card
		  id:: 5d29a7f1-bdb0-4277-86c8-177262856129
			- \(\eta=\frac{\frac{1}{2} \frac{M_W}{N_A} v_e^2}{\frac{1}{2} \frac{M_W}{N_A} v_e^2+e_I+e_L}\)
		- In the thruster efficiency formula, what do \(e_I\) and \(e_L\) represent? #card
		  id:: fbf7421f-5603-4188-a6ed-27bbad6c81c6
			- \(e_I\) is the ionization potential and \(e_L\) accounts for other energy losses in the system.
		- In an ion thruster, what are the ideal propellant characteristics? #card
		  id:: 5b390a4c-49b5-4d65-be6f-c94f5fa3ceef
			- High molecular mass and low ionization potential
	- In systems based on thermal expansion of the propellant in a nozzle, the main down-scaling challenge when trying to reduce the thrust level to the mN range or lower is represented by the efficiency of the nozzle itself.
	  ls-type:: annotation
	  hl-page:: 10
	  hl-color:: blue
	- The “discharge coefficient” is defined here as the ratio of the actual measured (or calculated) mass flow rate to the nominal one obtained by means of the Ideal Rocket Theory; thus, a low discharge coefficient indicates the presence of significant losses in the nozzle flow.
	  ls-type:: annotation
	  hl-page:: 10
	  hl-color:: blue
	- Besides the significant uncertainty in the experimental results, reported by the author to be caused by a combination of uncertainty of measurements and inaccuracy of micro-nozzle manufacturing, the plots in Figure 2 clearly show a dramatic decrease in nozzle performance starting at a throat Reynolds number in the range 500-1000. The reason behind this performance drop is not fully understood yet, but is believed to be related to the thick boundary layer at the nozzle throat caused by the laminar flow, which in turns makes the effective throat area smaller and the mass flow rate lower than the ideal one. This also makes the expansion in the nozzle divergent less effective due to the separation effects, with a worst case in which no expansion at all occurs when the flow separation becomes large enough. It is therefore expected that conventional nozzle shapes would not work properly at a throat Reynolds number lower than 1000, for which different types of nozzle shapes would need to be considered.
	  ls-type:: annotation
	  hl-page:: 11
	  hl-color:: blue
	- [[GPT Generated Flashcards]]
		- What is the main challenge when scaling down thermal expansion propulsion systems to the mN range or lower? #card
		  id:: 16c87e05-27a1-4694-878b-014e61d111d3
			- The efficiency of the nozzle itself.
		- How is the "discharge coefficient" defined in the context of thermal propulsion systems? #card
		  id:: 3ae0854c-deb9-4d7f-98a4-0727e532d2d2
			- The ratio of the actual measured mass flow rate to the nominal one obtained by means of the Ideal Rocket Theory.
		- What is the observed effect on nozzle performance at a throat Reynolds number in the 500-1000 range? #card
		  id:: b698ef3d-9b53-43ea-a193-56c4d1fe4c8a
			- A dramatic decrease in nozzle performance.
		- What is believed to be the reason behind the performance drop in nozzle efficiency at a Reynolds number lower than 1000? #card
		  id:: ff72993a-718f-43a8-85a5-4d822f62fcf7
			- The thick boundary layer at the nozzle throat caused by the laminar flow, which makes the effective throat area smaller and the mass flow rate lower than the ideal one, as well as separation effects.
		- At Reynolds numbers lower than 1000, what should be considered to improve nozzle performance? #card
		  id:: ff378f17-2697-464f-9805-bf495b47c7d6
			- Different types of nozzle shapes.
	- Recent research conducted at TU Delft has shown that for this range of very low throat Reynolds number, aerospike micro-nozzles (i.e., nozzles with the flow expanding around a central solid body, instead of being bounded by external walls) can allow for a performance improvement up to 33% when compared to conventional convergent-divergent ones.
	  hl-page:: 11
	  ls-type:: annotation
	  hl-color:: blue
	- The general scaling rules for micropropulsion systems are:
	  \(F_T=\dot{m} \cdot v_e \propto p_C A^* \propto p_C\left(d^*\right)^2\)
	- In a similar way, for the throat Reynolds number as defined in equation (1.11), it is possible to show that:
	  hl-page:: 11
	  ls-type:: annotation
	  hl-color:: blue
	  \(R e^*=\frac{a \cdot d^*}{\nu} \propto p_c \cdot d^*\)
	  where a is the speed of sound and \(\nu\) the kinematic viscosity of the gas flowing in the nozzle (evaluated at throat conditions in terms of pressure and temperature), and \(d^*\) is the throat diameter.
	- Another set of important down-scaling issues come from the variations of heat transfer mechanisms with size.
	  hl-page:: 11
	  ls-type:: annotation
	  hl-color:: blue
	  Heat transfer by conduction becomes much more effective in micropropulsion systems because, for the same material and the same thermal conductivity, smaller size leads to smaller temperature gradients and, thus, a significantly more uniform temperature in the whole thruster. This may represent an issue especially in thrusters where high temperatures are expected, such as chemical propulsion systems, where a large amount of heat power needs to be released by a smaller volume and, thus, the thermal stresses in the material are amplified.
	- [[GPT Generated Flashcards]]
		- Why does conduction become much more effective in micropropulsion systems? #card
		  id:: 7c8d2c33-a184-4681-a712-5972f0ff76df
			- For the same material and the same thermal conductivity, smaller size leads to smaller temperature gradients and a more uniform temperature.
		- How does smaller size affect temperature gradients in micropropulsion systems? #card
		  id:: 709022ce-57f1-46d6-8279-78d75156cc52
			- Smaller size leads to smaller temperature gradients and a more uniform temperature.
		- In what type of thrusters does the improved heat conduction represent an issue? #card
		  id:: 8e6ca741-9e5f-4a96-b569-882487f5cc7e
			- Chemical propulsion systems.
		- How does the smaller size in micropropulsion systems affect thermal stresses in the material? #card
		  id:: 96ec8294-85a6-427f-a91d-ba135ecd7a95
			- The thermal stresses are amplified because a large amount of heat power needs to be released by a smaller volume.
	- Convective heat transfer between propellant and nozzle also increases, meaning that higher thermal losses can be expected in the nozzle flow.
	  ls-type:: annotation
	  hl-page:: 11
	  hl-color:: blue
	- Other design challenges are generated by the significantly different thermal expansion coefficients of different materials used in the thruster, which may lead to increased risk of leaks and additional thermal stresses.
	  hl-page:: 11
	  ls-type:: annotation
	  hl-color:: blue
	- [[GPT Generated Flashcards]]
		- What performance improvement (in numbers) can aerospike micro-nozzles provide compared to conventional convergent-divergent nozzles? #card
		  id:: 6ed409bf-f4ff-4f9a-bbdc-ee8bbfd56313
			- Up to 33%.
		- The general scaling rules for micropropulsion systems are: #card
		  id:: 16d696a3-1229-44fa-912c-2e03702c1353
			- \(F_T=\dot{m} \cdot v_e \propto p_C A^* \propto p_C\left(d^*\right)^2\)
		- The general Reynold number scaling rules for micropropulsion systems are: #card
		  id:: 6a4f45c1-a3cc-46d0-aee6-ec109bf34e0a
			- \(R e^*=\frac{a \cdot d^*}{\nu} \propto p_c \cdot d^*\)
		- What determines the force produced by a micropropulsion system? #card
		  id:: 8a5ad3fc-bafc-498f-9c19-c66223859c67
			- Throat mass flow rate and exit velocity.
		- What factor affects the throat Reynolds number in micropropulsion systems? #card
		  id:: 5fb62448-03d7-47b8-8b6d-aaff81568110
			- Throat diameter.
		- In micropropulsion systems, how does heat transfer by conduction change with size? #card
		  id:: e4394283-0b87-4595-b085-0785025260a2
			- It becomes more effective, leading to more uniform temperatures.
		- How do high temperatures in the thruster affect chemical propulsion systems in micropropulsion? #card
		  id:: 43b56cff-15d1-4f7c-a8c5-56e7bed58af9
			- They result in increased thermal stresses due to the release of a large amount of heat power by a smaller volume.
		- What happens to convective heat transfer between propellant and nozzle in micropropulsion systems? #card
		  id:: e378959c-8690-46af-9928-ea7f4288096a
			- It increases, leading to higher thermal losses in the nozzle flow.
		- What is a design challenge caused by different thermal expansion coefficients of materials used in thrusters? #card
		  id:: 44a8b715-3f25-480d-9524-0c8d8de0071d
			- Increased risk of leaks and additional thermal stresses.
	- Finally, in propulsion systems where a chemical reaction takes place in the combustion chamber, the effectiveness of the chemical reaction strongly depends on the residence time of the propellants in the chamber and on the so-called characteristic length, a design parameter defined as the ratio of the chamber volume to the nozzle throat area. For a given combination of propellants, there is always a (fixed) optimum range of characteristic length values in order to achieve efficient combustion. Considering that the ratio of combustion chamber area to throat area is not expected to change significantly when going from macro- to micro-scale, this means that the combustion chamber length should be kept constant for any size of the system, which is obviously not practical when all other dimensions are reduced by several orders of magnitude.
	  ls-type:: annotation
	  hl-page:: 12
	  hl-color:: blue
	- For electric micro-propulsion systems, as well as any other micro-propulsion systems that require a non-negligible amount of power for their operation, the most significant downscaling challenge is represented by the power itself as well as, in most of the cases, the power-to-thrust ratio.
	  ls-type:: annotation
	  hl-page:: 12
	  hl-color:: blue
	- [[GPT Generated Flashcards]]
		- In propulsion systems with chemical reactions, what does the effectiveness of the reaction depend on? #card
		  id:: 9b0c34ba-b893-4dea-94dc-6911fec2ce68
			- Residence time of propellants and characteristic length.
		- What is the characteristic length? #card
		  id:: 4d4737ed-e271-4120-a2f5-596c92c55e2b
			- The ratio of combustion chamber volume to nozzle throat area.
		- What happens to the combustion chamber length when scaling down propulsion systems? #card
		  id:: 31aba9c0-1856-41d2-8919-e7793918b59a
			- Keeping it constant is not practical when other dimensions are reduced significantly.
		- What is the most significant downscaling challenge for electric micro-propulsion systems? #card
		  id:: efc2f812-d4dd-41b9-97af-ce89ce99f7d9
			- Power and power-to-thrust ratio.