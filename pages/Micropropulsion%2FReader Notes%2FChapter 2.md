## Cold Gas Systems
id:: 6466ff58-7b9e-4334-aff8-923a4ed95b76
	- In cold gas systems, the propellant is stored at high pressure (usually in its liquid phase to allow for higher density and therefore reduced volume, but in principle it can also be stored in the gaseous phase) and accelerated in a nozzle without any additional heating or energy input. If the propellant is stored as a liquid, it is vaporized before reaching the nozzle.
	  ls-type:: annotation
	  hl-page:: 14
	  hl-color:: yellow
	- In micro-thrusters typically the pressure regulator is not present due to mass and volume limitations (in particular when the propellant is stored in the gaseous phase), and the only required power is to activate the valve and keep it open when needed.
	  hl-page:: 14
	  ls-type:: annotation
	  hl-color:: yellow
	- In absence of the pressure regulator, the gaseous propellant storage pressure in the tank continuously decreases while propellant is extracted from it (blow-down operation)
	  hl-page:: 14
	  ls-type:: annotation
	  hl-color:: yellow
	- Blowdown operation is the process of releasing pressurized gas from a tank in a rocket in order to feed propellant to the engine. During blowdown operation, there is no active control over the gas pressure, which decreases steadily as the propellant is consumed.
	- [[GPT Generated Flashcards]]
		- What is the propellant storage method for cold gas systems? #card
		  id:: 3f66f96d-db64-43ec-9de0-12eae08ff838
			- High pressure.
		- In cold gas systems, can the propellant be stored in both the liquid or gaseous phase? #card
		  id:: 9904e406-7e8b-496e-9008-e51a2d510c5d
			- Yes.
		- Are pressure regulators typically present in micro-thrusters? #card
		  id:: 7a1c4243-6f49-4d99-ac65-85dd22f37b79
			- No.
		- What is the only required power source in cold gas micro-thrusters? #card
		  id:: ff673e41-d542-4ac3-b92e-7879bf8ccce3
			- To activate the valve and keep it open when needed.
		- What happens to the storage pressure in the absence of a pressure regulator? #card
		  id:: eaf0ba6d-d833-494e-92f8-608ecee43cea
			- It continuously decreases.
		- What is blowdown operation? #card
		  id:: 4ac1db51-5940-4318-96f0-e2f580fc2b93
			- Releasing pressurized gas from a tank in a rocket to feed propellant to the engine.
		- What happens to gas pressure during blowdown operation? #card
		  id:: bee8750b-ed8d-4371-97c6-910fd250b691
			- It decreases steadily as the propellant is consumed.
	- If the extraction of propellant is not too fast, it can be assumed that the blow-down process is isothermal and, therefore, the pressure $p_T$ and mass $M_T$ of propellant in the tank change according to the following relationship: \(\frac{p_T}{M_T}=\) constant
	  hl-page:: 15
	  ls-type:: annotation
	  hl-color:: yellow
	- given the continuous reduction of tank pressure in non-regulated systems, and remembering from equation (1.12) that the thrust is proportional to the propellant inlet pressure, it can be inferred that the thrust level provided by these systems is not constant and continuously decreasing with time during operation in orbit.
	  ls-type:: annotation
	  hl-page:: 15
	  hl-color:: yellow
	- Typical propellants for cold gas micro-thrusters are Isobutane, refrigerants (such as R236fa or R134a), Sulfur Dioxide, Sulfur Hexafluoride, but also more common gases such as Nitrogen, Argon, Xenon.
	  ls-type:: annotation
	  hl-page:: 15
	  hl-color:: yellow
	- [[GPT Generated Flashcards]]
		- What can be assumed about the blow-down process if the extraction of propellant is not too fast? #card
		  id:: 41337971-da35-46f2-914b-e025e9873ac1
			- It can be assumed to be isothermal.
		- What is the relationship between the pressure and mass of propellant in the tank during an isothermal process? #card
		  id:: e7a1ef92-bf1f-4040-a378-6701a39f956d
			- \(\frac{p_T}{M_T}=\) constant
		- How does the thrust level of non-pressure-regulated systems change with time during operation in orbit? #card
		  id:: e1d22f1b-8668-41e4-8414-bdfae3984a1b
			- The thrust level is not constant and decreases continuously.
		- What are some typical propellants for cold gas micro-thrusters? #card
		  id:: 8d0592cf-98b1-414a-852b-af598a1c9c61
			- Isobutane, Nitrogen,
			  Refrigerants (R236fa, R134a), 
			  Sulfur Dioxide, Sulfur Hexafluoride,
			  Argon, and Xenon.
## Mono-Propellant Systems
	- In mono-propellant systems, the propellant is typically stored in its liquid phase and pressurized by a pressurant gas which is usually stored separately, with a pressure regulator between the two tanks in order to ensure for constant nozzle inlet pressure and, therefore, constant thrust. By opening the thrust valve, the propellant is then flown into the decomposition chamber, where it chemically decomposes into simpler molecules generating heat and, therefore, entering the nozzle inlet at high temperature. Decomposition is usually facilitated by a catalyst, but also requires in most cases pre-heating of the propellant which, in turn, requires a non-negligible amount of satellite power.
	  hl-page:: 16
	  ls-type:: annotation
	  hl-color:: red
		- [[GPT Generated Flashcards]]
		- How are mono-propellant systems pressurized? #card
		  id:: 1db328d6-20a0-4108-84ac-b2b493a48f0e
			- Through a separate pressurant gas, mediated by a pressure regulator.
		- What happens when the thrust valve is opened in a mono-propellant system? #card
		  id:: d5a2d2db-586e-4e2f-9b94-d1646f4cc2ad
			- Propellant flows into the decomposition chamber.
		- What is decomposition in mono-propellant systems? #card
		  id:: ae4931bc-7a7a-4737-8d24-8fe4a9eb1c6e
			- When the propellant decomposes into simpler molecules, generating heat.
		- What is the purpose of a catalyst in a mono-propellant system? #card
		  id:: d0b66a67-4430-4f82-b2c9-b643d02d7bde
			- To facilitate chemical decomposition of the propellant.
		- What happens to the propellant after decomposition in a mono-propellant system? #card
		  id:: 6850bf59-acb4-4b39-a01e-98f66c8507fd
			- It enters the nozzle inlet at a high temperature.
		- Why is pre-heating the propellant necessary in most cases for monopropellant systems? #card
		  id:: eb2b1761-a6b6-40fe-89a0-99756940d04a
			- To facilitate decomposition.
	- In the case of mono-propellant micro-propulsion systems, “green” propellants are typically used (non-toxic, non-hazardous, easily storable and safe to handle). High-density liquids are usually preferred in order to reduce the required tank volume.
	  ls-type:: annotation
	  hl-page:: 16
	  hl-color:: red
	- Typical propellants are Hydroxyl-Ammonium Nitrate (HAN) and its recently developed, high-performance derivative AF-M315E; Ammonium DiNitramide (ADN) and its derivative LMP-103S. A less typically used green alternative is Hydrogen Peroxide.
	  ls-type:: annotation
	  hl-page:: 16
	  hl-color:: red
	- [[GPT Generated Flashcards]]
		- What are the main characteristics of "green" propellants in mono-propellant micro-propulsion systems? #card
		  id:: 60ee7141-2f70-471b-8605-18d3e90b4d53
			- Non-toxic,
			  non-hazardous,
			  easily storable,
			  safe to handle.
		- Why are high-density liquids preferred in mono-propellant micro-propulsion systems? #card
		  id:: 272a9c6e-ea68-4adc-94c0-ba5e63b588a1
			- To reduce the required tank volume.
		- What are two examples of typical green propellants in mono-propellant micro-propulsion systems? #card
		  id:: 9e2176a6-1ae6-4090-90b0-e77b8906fdfe
			- Hydroxyl-Ammonium Nitrate (HAN),
			  Ammonium DiNitramide (ADN).
		- Which specific high-performance derivative is derived from Hydroxyl-Ammonium Nitrate (HAN)? #card
		  id:: af563b11-df0b-4e51-a0de-0c6ba13abee3
			- AF-M315E.
		- What derivative is derived from Ammonium DiNitramide (ADN)? #card
		  id:: 9f0f81f3-3b72-480e-a0a5-95d426a5b95c
			- LMP-103S.
		- What is a less commonly used green alternative propellant in micro-propulsion systems? #card
		  id:: 08b731e1-9c31-4c9f-84f8-134483195434
			- Hydrogen Peroxide.
## Bi-Propellant Systems
	- In Bi-Propellant systems, instead of one single propellant there are two of them (an oxidizer and a fuel), also in this case stored in their liquid phase and pressurized by a pressurant gas usually stored separately, with a pressure regulator (R) between the two tanks in order to ensure for constant nozzle inlet pressure and, therefore, constant thrust. Two thrust valves are present in this case, through which the propellants flow into the combustion chamber, where a chemical reaction between fuel and oxidizer generates heat and allows them to enter the nozzle inlet at high temperature.
	  hl-page:: 17
	  ls-type:: annotation
	  hl-color:: green
	- Not many bi-propellant systems are currently available at the micro-scale and they are usually characterized by a relatively high trust level compared to other micropropulsion systems, mainly due to down-scaling issues related to the residence time of propellants in the combustion chamber
	  ls-type:: annotation
	  hl-page:: 17
	  hl-color:: green
	- [[GPT Generated Flashcards]]
		- What are the two components of a Bi-Propellant system? #card
		  id:: d3a0256f-c327-4c88-b6fa-90d10a993a6f
			- Oxidizer and fuel.
		- In Bi-Propellant systems, what phase are the propellants stored in? #card
		  id:: ee4169ee-ec8b-4f6d-b8d4-0bfeb15d2e59
			- Liquid phase.
		- How are propellants in a Bi-Propellant system pressurized? #card
		  id:: 8ab17ece-ef8d-48eb-8a12-aa94ddbb1a3c
			- Pressurant gas.
		- What is the purpose of the pressure regulator in a Bi-Propellant system? #card
		  id:: a0f27d84-800c-4868-ae78-a2c39a18f681
			- To ensure constant nozzle inlet pressure and constant thrust.
		- Through what do the propellants reach the combustion chamber in a Bi-Propellant system? #card
		  id:: 93c508c2-c992-449a-969a-97f232a4e28f
			- Through thrust valves.
		- What generates heat in the combustion chamber of a Bi-Propellant system? #card
		  id:: cd2fdc00-5896-4127-8a83-876c751f4d66
			- Chemical reaction between fuel and oxidizer.
		- Are there many Bi-Propellant systems available at the micro-scale? #card
		  id:: 95807b13-3246-473f-a6a3-bd9b078d7e02
			- No.
		- Why is the trust level of micro-scale Bi-Propellant systems high compared to other micropropulsion systems? #card
		  id:: 0c66e77f-b5b4-4372-a0c0-b20c17525d30
			- Due to down-scaling issues related to the residence time of propellants in the combustion chamber.
	- the combustion temperature in bi-propellant systems is normally significantly higher than mono-propellant systems, which allows for higher specific impulse but also causes more significant thermal issues.
	  hl-page:: 17
	  ls-type:: annotation
	  hl-color:: green
	- Bi-propellant systems use Nitrous Oxide+Propene and liquid water (which is then converted to Hydrolox through electrolysis) as propellants
	  hl-page:: 18
	  ls-type:: annotation
	  hl-color:: green
	- [[GPT Generated Flashcards]]
		- What is the main difference between combustion temperatures in bi-propellant and mono-propellant systems? #card
		  id:: 4778acf9-0289-4bed-823d-2816e3db12f2
			- Bi-propellant systems have significantly higher combustion temperatures.
		- What is the advantage of higher combustion temperatures in bi-propellant systems? #card
		  id:: d43d7a43-d68e-497e-a1c1-60d180a3f8fe
			- Higher specific impulse.
		- Which propellants are used in bi-propellant systems? #card
		  id:: 32b760b9-6ed1-4792-8026-7a7c6d23a518
			- Nitrous Oxide + Propene,
			  Liquid water converted to Hydrolox through electrolysis.
	- HYDROS micro-thruster (Figure 9), produced by the company Tethers Unlimited. In this system, the propellant is stored as liquid water and electrolysis is used to convert water into hydrogen and oxygen which are the actual fuel and oxidizer flown in the combustion chamber
	  ls-type:: annotation
	  hl-page:: 18
	  hl-color:: green
## Solid Propellant Systems
	- Solid propellant systems are basically the same as bi-propellant ones, with the only difference that propellants are stored in solid phase in the same grain, and require energy from an igniter to start their combustion.
	  ls-type:: annotation
	  hl-page:: 18
	  hl-color:: blue
	- they suffer from the fact that combustion of a single grain, once initiated, can not be stopped and will continue until the propellants are completely consumed.
	  ls-type:: annotation
	  hl-page:: 18
	  hl-color:: blue
	- Solid Propellant micropropulsion systems have not been extensively developed yet for small satellites due to the typical limitations on pyrotechnic devices present in the requirements for this class of satellites. These limitations may include safety concerns, the compact size needed for the propulsion system, and the overall complexity associated with pyrotechnic devices.
	  hl-page:: 18
	  ls-type:: annotation
	  hl-color:: blue
	- some systems characterized by significantly high thrust levels(in the range 10-100 N) have been proposed for specific applications, such as de-orbiting at the satellite end of life.
	  ls-type:: annotation
	  hl-page:: 18
	  hl-color:: blue
	- [[GPT Generated Flashcards]]
		- What is the main difference between solid propellant systems and bi-propellant systems? #card
		  id:: cbc8eb5e-98cb-4016-b270-fd19be7acbf6
			- Solid propellants are stored in the same grain and require an igniter to start combustion.
		- What is the main disadvantage of solid propellant systems? #card
		  id:: 45167efb-2a14-46fa-9594-efe4dc5d66f1
			- They cannot be stopped and combustion continues until the propellants are completely consumed.
		- Why have solid propellant systems not been extensively developed for small satellites? #card
		  id:: 4c7935d0-2a7e-4999-ad1a-6f6c1ba97f62
			- They have limitations on pyrotechnic devices present in the requirements for this class of satellites like: safety concerns, the compact size needed, and overall complexity.
		- What thrust range have high-thrust solid propellant systems been proposed for? #card
		  id:: fdf05229-9609-48fe-9a16-526641a27f22
			- 10-100 N.
		- What is one application proposed for high-thrust solid propellant systems? #card
		  id:: 235e4cfe-1ead-41a6-a2ea-05ac17f55174
			- De-orbiting at the satellite end of life.
	- the regression rate r of the solid propellant grain has to be taken into account. In the simplest possible approximation, the regression rate can be estimated as a function of the combustion chamber pressure through the following equation: \(r=a \cdot p_C^n\)
	  ls-type:: annotation
	  hl-page:: 18
	  hl-color:: blue
	- where a is the temperature coefficient and n is the combustion index (normally lower than 1), both characteristic of the specific solid propellant grain.
	  ls-type:: annotation
	  hl-page:: 19
	  hl-color:: blue
	- The mass flow rate can then be calculated as: \(\dot{m}=r \cdot \rho_P \cdot A_b\) where $\rho_P$ is the propellant grain density and $A_b$ is its instantaneous burning surface.
	  hl-page:: 19
	  ls-type:: annotation
	  hl-color:: blue
	- it is clear that the chamber pressure evolution over time, and therefore the thrust evolution over time, are a direct consequence of how the grain burning surface changes over time. By selecting a grain geometry with increasing, decreasing or constant burning surface, it is possible to also obtain increasing, decreasing or constant chamber pressure and thrust.
	  ls-type:: annotation
	  hl-page:: 19
	  hl-color:: blue
	- [[GPT Generated Flashcards]]
		- What does the regression rate of a solid propellant grain depend on? #card
		  id:: 14ac73c7-ce77-4cbf-bf9b-7b9d1cb44de4
			- Combustion chamber pressure.
		- What equation is used to calculate mass flow rate for solid propellant combustion? #card
		  id:: 8496e4eb-f005-4fe2-a210-cbe9a6bb3e27
			- \(\dot{m}=r \cdot \rho_P \cdot A_b\).
		- How can you obtain different types of chamber pressure and thrust evolution over time for solid propellant systems? #card
		  id:: 018d79c3-9a11-4386-9b8f-2fc54e7b7f26
			- By selecting grain geometry with increasing, decreasing, or constant burning surface.
## Micro-Resistojets
	- Resistojets can be seen as an intermediate concept between electrical and chemical propulsion since the propellant is heated electrically (typically by means of a resistance) and accelerated in a convergent-divergent nozzle.
	  hl-page:: 19
	  ls-type:: annotation
	  hl-color:: purple
	- In principle, any propellant can be used, stored in any phase (liquid, solid or gaseous); in practice, however, liquid propellants are the most widely used. An alternative to liquid propellants are the socalled warm gas thrusters, which are basically cold gas systems allowing for additional(usually limited) heating of the gaseous propellant before being accelerated in the nozzle.
	  ls-type:: annotation
	  hl-page:: 19
	  hl-color:: purple
	- resistojets are very similar to cold gas thrusters: the propellant is stored in a tank, pressurized (when in the liquid phase) by a pressurant gas and injected in the heating chamber by opening a thrust valve. 
	  ls-type:: annotation
	  hl-page:: 19
	  hl-color:: purple
	- A pressure regulator is usually not included, meaning that the operation is typically blow-down and the pressure (and thrust) provided by the system are decreasing over its lifetime.
	  ls-type:: annotation
	  hl-page:: 20
	  hl-color:: purple
	- The specific impulse, although higher than cold gas systems due to the higher temperature of the propellant and the nozzle inlet, is still limited due to the limitations in the available heating power.
	  ls-type:: annotation
	  hl-page:: 20
	  hl-color:: purple
	- [[GPT Generated Flashcards]]
		- How are resistojets different from traditional chemical and electric propulsion? #card
		  id:: 7d2a2759-8c1c-4a23-9024-231a4603e218
			- Resistojets heat the propellant electrically.
		- What is a key advantage of resistojets compared to cold gas systems, though they are quite similar? #card
		  id:: 7578cbc1-b4fa-48cc-a54b-7c7f5792bd92
			- Higher specific impulse.
		- What are warm gas thrusters? #card
		  id:: 33fbc76b-c109-433b-9b2b-9f27bbdb30da
			- Cold gas systems allowing for limited heating of the gaseous propellant (so Resistojets).
		- How is propellant stored in resistojets? #card
		  id:: 4bd79e1d-6c5b-4fdf-86ef-b88305fc24d0
			- In a tank, pressurized by a pressurant gas.
		- Which phase of propellant is most commonly used in resistojets? #card
		  id:: b58acf6c-fc3e-4a86-b7ab-b993b0fcbe30
			- Liquid phase.
		- What is the main limitation in resistojet's specific impulse? #card
		  id:: cf0977b0-fc5b-4523-9397-2db825bfa2c1
			- The available heating power.
		- Do resistojets typically operate in blow-down mode? #card
		  id:: 0afa2699-97dc-41b2-9b16-66b90e4b724c
			- Yes, since pressure regulators are usually not included.
	- Since the propellant is accelerated in a nozzle, equation (1.5) for the mass flow rate is still valid; however, for the most common case of a liquid propellant that needs to be vaporized before being accelerated in the nozzle, it has to be combined with the following relationship that characterizes the vaporization and heating of the propellant: \(P_h=\dot{m} \cdot\left[c_{p L} \cdot\left(T_{b o i l}-T_0\right)+L_h+c_{p G} \cdot\left(T_C-T_{\text {boil }}\right)\right]\)
	  hl-page:: 20
	  ls-type:: annotation
	  hl-color:: purple
	  where \(P_h\) is the available heating power, \(T_0\) is the initial propellant temperature, \(T_{\text {boil }}\) is the propellant boiling temperature (which in turn is a function of the heating chamber pressure), \(c_{p L}\) and \(c_{p G}\) are the constant pressure specific heat of respectively the liquid and gaseous propellant phase (both usually functions of the temperature), \(L_h\) is the latent heat of vaporization of the propellant.
	- given a desired temperature at which the propellant has to be heated, the required heating power to achieve that temperature will be a function of the propellant pressure and, therefore, in a system without pressure regulator it will vary over the lifetime of the system.
	  ls-type:: annotation
	  hl-page:: 20
	  hl-color:: purple
	- Propellants used for micro-resistojets are liquid water, R134a refrigerant, and ammonia
	- [[GPT Generated Flashcards]]
		- Does equation 1.5 (relating mass flow rate and chamber/throat conditions) apply to micro-resistojet systems? #card
		  id:: 99e97bd7-c968-44ce-b4ee-05021903d8d5
			- Yes, because the heated propellant is accelerated through a convergent/divergent nozzle.
		- What is the equation for available heating power in micropropulsion? #card
		  id:: a7c56f1a-8fb2-4aa7-9c75-b27cf26bd919
			- \(P_h=\dot{m} \cdot\left[c_{p L} \cdot\left(T_{b o i l}-T_0\right)+L_h+c_{p G} \cdot\left(T_C-T_{\text {boil }}\right)\right]\)
			  
			  where \(P_h\) is the available heating power,
			  \(T_0\) is the initial propellant temperature,
			  \(T_{\text {boil }}\) is the propellant boiling temperature (which in turn is a function of the heating chamber pressure),
			  \(c_{p L}\) and \(c_{p G}\) are the constant pressure specific heat of respectively the liquid and gaseous propellant phase (both usually functions of the temperature),
			  \(L_h\) is the latent heat of vaporization of the propellant.
		- What are \(c_{p L}\) and \(c_{p G}\) in the resistojet available heating power equation? #card
		  id:: 94dc9e2c-1597-468f-adbe-e0ce44dfc450
			- Constant pressure specific heat of the liquid and gaseous propellant phase
		- What does \(L_h\) represent in the resistojet available heating power equation? #card
		  id:: d9a58348-1a06-4496-b4bc-599a8913c40c
			- Latent heat of vaporization of the propellant
		- What factors affect the required heating power for micropropulsion? #card
		  id:: 2ac0d976-1c9f-4f2a-96cb-f3a7a1978d6f
			- Propellant pressure and desired temperature
		- Name three propellants commonly used in micro-resistojets. #card
		  id:: 061b667f-69f0-43dc-80a5-734e78f2b87f
			- Liquid water,
			  R134a refrigerant,
			  Ammonia
	- TU Delft is currently working at a micro-resistojet system for small satellites using liquid water as propellan
	  ls-type:: annotation
	  hl-page:: 20
	  hl-color:: purple
	- The choice of water is not only driven by the fact that it is a safe, easy to handle, cheap propellant, but also by a thorough analysis which has shown that, among all propellants that can be stored as a liquid at ambient temperature and relatively low pressure (no more than 10 bar), water is the fluid which allows for the best combination of specific impulse and tank volume for a given Delta-V requirement, thanks to its relatively low molecular mass and high density, in spite of the high value of its heat of vaporization
	  ls-type:: annotation
	  hl-page:: 20
	  hl-color:: purple
	- [[GPT Generated Flashcards]]
		- What factors make water a suitable propellant for micro-resistojet micropropulsion? #card
		  id:: 67aa57df-67af-4398-8685-b82327605049
			- Safe, easy to handle, cheap, high density, low molecular mass, and liquid at ambient temperature and low pressure.
		- What property of water allows for the best combination of specific impulse and tank volume for a given Delta-V requirement? #card
		  id:: d72e152d-3216-467f-a336-b515ef9dda11
			- Relatively low molecular mass and high density.
		- What is the maximum pressure at which water can be stored as a liquid at ambient temperature? #card
		  id:: 4e1d90b9-f03c-45f7-8522-446b2c655200
			- 10 bar.
	- R134a refrigerant
	  ls-type:: annotation
	  hl-page:: 20
	  hl-color:: purple
	- Ammonia 
	  ls-type:: annotation
	  hl-page:: 20
	  hl-color:: purple
## Ion Thrusters and RF Electric Thrusters
	- In the classical concept, ions are generated by electron bombardment, i.e. by collisions between propellant molecules and electrons injected in the ionization chamber. The ions are then accelerated by two grids between which a potential drop is applied. Since the expelled ions are positively charged, it is important to expel an equal number of negatively charged particles (electrons) in order to keep the spacecraft neutral. This is done by a component called neutralizer, which is basically the same as the component which injects the electrons in the ionization chamber.
	  ls-type:: annotation
	  hl-page:: 21
	  hl-color:: yellow
	- a good propellant for an ion thruster is a fluid with high molecular mass and low ionization potential.
	  ls-type:: annotation
	  hl-page:: 21
	  hl-color:: yellow
	- Most of the current ion thrusters, either at the macro- or the micro-scale, use gaseous Xenon as propellant, which is one of the best available options according to these criteria.
	  ls-type:: annotation
	  hl-page:: 21
	  hl-color:: yellow
	- [[GPT Generated Flashcards]]
		- How are ions generated in a classical ion thruster? #card
		  id:: 4fb51136-8860-4897-9530-afce871f3cd7
			- By electron bombardment.
		- What accelerates ions in the ion thruster? #card
		  id:: 56305e21-bfa8-40e7-8bf2-6d6df4942d57
			- Two grids with a potential drop applied between them.
		- Why is it important to expel an equal amount of negatively charged particles along with the positively charged ions? #card
		  id:: 4d4486ef-a187-458a-83c2-311fcf0da234
			- To keep the spacecraft neutral.
		- What component in an ion thruster expels negatively charged particles? #card
		  id:: 8b2ec774-d9b4-4fc0-bd29-b6db99c4a6d3
			- Neutralizer.
		- What two properties make a propellant good for an ion thruster? #card
		  id:: 14c70ec8-ef7e-45a1-bcb5-3f5831bd9b22
			- High molecular mass and low ionization potential.
		- Which propellant is commonly used in ion thrusters? #card
		  id:: fd716f2c-157c-41b3-86b2-3be4fe03e592
			- Gaseous Xenon.
	- Radio-Frequency electric thrusters are based on exactly the same working principle as ion thrusters, with the only difference that propellant is not ionized by electron bombardment, but by Radio Frequency (RF) power provided by coils wrapped around the ionization chamber, creating an azimuthally oscillating electric field to generate the ions.
	  hl-page:: 21
	  ls-type:: annotation
	  hl-color:: yellow
	- RF thrusters are affected by a number of drawbacks when compared to electron bombardment ion engines: they are usually less efficient and require bulky electronics for the conversion from the power provided by the solar panels(typically DC) to the RF power required by the thruster coils.
	  ls-type:: annotation
	  hl-page:: 22
	  hl-color:: yellow
	- Xenon is still a common propellant choice for miniaturized Radio-Frequency thrusters, but Iodine is also a very typical alternative that allows for higher storage density and smaller tank volumes.
	  ls-type:: annotation
	  hl-page:: 22
	  hl-color:: yellow
	- [[GPT Generated Flashcards]]
		- What is the main difference between Radio-Frequency electric thrusters and ion thrusters? #card
		  id:: 8b660730-4a59-42f7-b263-c2f7a412cc9b
			- Ionization method.
		- How is propellant ionized in Radio-Frequency electric thrusters? #card
		  id:: 2fb058bf-65df-4045-92e4-d8fe3fb3dca7
			- By Radio Frequency power provided by coils.
		- What drawbacks do RF thrusters have compared to electron bombardment ion engines? #card
		  id:: c8ad4bf0-9068-4e32-9100-f6fa6ba337fa
			- Lower efficiency and bulky electronics.
		- What power conversion is required for RF thruster coils? #card
		  id:: 7d532f46-ea42-4437-b837-b737251f0f96
			- From DC to RF power.
		- What are two common propellant choices for miniaturized Radio-Frequency thrusters? #card
		  id:: 7712481d-28ec-4432-8086-ab23f066e89d
			- Xenon and Iodine.
		- Why (two reasons) is Iodine a popular alternative for miniaturized RF thrusters? #card
		  id:: 04c2551f-4969-45c1-b96a-42a5dcea4062
			- Higher storage density and smaller tank volumes.
## Hall Effect Thrusters
	- in Hall Effect thrusters, thrust is generated by first ionizing and then accelerating the propellant. However, in this case, a different acceleration mechanism is used, based on mutually perpendicular electric and magnetic fields applied to the ionization chamber. As in ion thrusters, electrons are injected in the ionization chamber. As a consequence of the Hall effect, they start moving in a spiral trajectory with velocity perpendicular to both the magnetic field B and the electric field E. Ionization of the propellant, as usual, is obtained through collisions between these electrons and the propellant molecules, and propellant ions are then accelerated by the applied electric field. Therefore, no grids are needed in this case to accelerate the propellant, and they are replaced in practice by the applied magnetic field which, in a typical Hall Effect thruster, is radial.
	  ls-type:: annotation
	  hl-page:: 23
	  hl-color:: red
	  hl-stamp:: 1683191745086
	- Hall Effect thrusters are typically characterized by high specific impulse (although slightly lower than ion thrusters), high thrust density and design simplicity. Their main drawback, especially when used at the micro-scale, is the very low efficiency and, consequently, extremely high required input power. They typically use the same type of propellants as ion thrusters, such as Xenon, Krypton, Iodine, Argon.
	  ls-type:: annotation
	  hl-page:: 23
	  hl-color:: red
	- Due to the mentioned down-scaling difficulties and high power requirements caused by the low efficiency, no Hall Effect thrusters are currently available at a scale that can be easily applied to small satellites such as CubeSats.
	  ls-type:: annotation
	  hl-page:: 24
	  hl-color:: red
	- [[GPT Generated Flashcards]]
		- How is thrust generated in Hall Effect thrusters? #card
		  id:: fc939f17-6275-4beb-b360-2e12f5c7204a
			- As in ion thrusters, electrons are injected in the ionization chamber. As a consequence of the Hall effect, they start moving in a spiral trajectory with velocity perpendicular to both the magnetic field B and the electric field E. Ionization of the propellant, as usual, is obtained through collisions between these electrons and the propellant molecules, and propellant ions are then accelerated by the applied electric field.
		- In Hall Effect thrusters, what replaces the grids that are used to accelerate propellant in ion thrusters? #card
		  id:: ecaeb684-47e1-4b15-b08d-1b7f08b5f48a
			- The applied magnetic field.
		- What are three advantages of Hall Effect thrusters? #card
		  id:: 16beecab-15c0-4125-b433-9445a8a90715
			- High specific impulse, high thrust density, and design simplicity.
		- What is the main drawback of Hall Effect thrusters when used at the micro-scale? #card
		  id:: 261f9eb7-3640-4edc-97e0-cdd263c38b44
			- Very low efficiency, leading to extremely high required input power.
		- What type of propellants do Hall Effect thrusters typically use? #card
		  id:: bf093166-bc3f-46f4-9586-247f08d57d99
			- Xenon, Krypton, Iodine, Argon.
		- Are there any Hall Effect thrusters available that can be easily applied to small satellites like CubeSats? #card
		  id:: 19a37eea-934a-4950-8c9c-0baa900aca75
			- No, due to down-scaling difficulties and high power requirements caused by low efficiency.
## Electrospray Thrusters
	- Electrospray thrusters are based on electrostatic acceleration of charged ions from a liquid propellant to produce thrust. The propellant is a conductive liquid and its surface is deformed by a strong electric field into a sharp cone-shaped meniscus called Taylor Cone; when a certain electric potential threshold is reached, ions are extracted from the cone and then accelerated by the same electric field used for their extraction. Both positive and negative ions are accelerated, thus there is no need for an additional neutralizer as in ion thrusters. The propellants used by electrospray thrusters are usually ionic liquids, characterized by a very small vapour pressure that allows for avoiding propellant pressurization. Additionally, ionic liquids do not require heating, have low operating voltage and high conductivity. Typical propellants include liquid metals such as Cesium, Gallium and Indium, or solutions of Formamide, Propylene Carbonate, water, Tri-Ethylene Glycol doped with Sodium Iodide or other ionic salts.
	  ls-type:: annotation
	  hl-page:: 24
	  hl-color:: green
	  hl-stamp:: 1683191850309
	- by combining several emitters in an array, it is possible to obtain higher thrust levels at the cost of a higher required input power.
	  ls-type:: annotation
	  hl-page:: 24
	  hl-color:: green
	- [[GPT Generated Flashcards]]
		- What principle do electrospray thrusters operate on? #card
		  id:: 511801c0-836d-491f-86fc-94f13271ebaa
			- Electrostatic acceleration of charged ions from the surface of a liquid propellant. When a certain electric potential threshold is reached, ions are extracted from the surface and then accelerated by the same electric field used for their extraction.
		- In Electrospray thruster, what is the sharp cone-shaped meniscus formed by the electric field on the propellant surface called? #card
		  id:: 087682ce-366d-458b-8dae-1e3ffde24e23
			- Taylor Cone.
		- Do electrospray thrusters require an additional neutralizer? #card
		  id:: 0d3d8259-c1f3-427a-8a0d-7924b990dc2b
			- No.
		- What type of propellants do electrospray thrusters typically use? #card
		  id:: 322ddd23-fde2-4c4c-b419-3218a112170b
			- Ionic liquids.
		- Why do ionic liquids not require pressurization in electrospray thrusters? #card
		  id:: 38af6f9f-6443-4062-a5df-30cd00bd6416
			- They have a very small vapor pressure.
		- Name three typical liquid metal propellants used in electrospray thrusters. #card
		  id:: 323cbac5-4f52-417a-af91-9fe9d3812cf1
			- Cesium, Gallium, and Indium.
		- Name some less common ionic liquid propellants used in electrospray thrusters. #card
		  id:: 46e5e0fa-179e-4b75-b63a-9a587484b57b
			- Solutions of Formamide,
			  Propylene Carbonate,
			  Water,
			  Tri-Ethylene Glycol doped with Sodium Iodide or other ionic salts.
		- What can be achieved by combining several emitters in an electrospray array? #card
		  id:: 4b5d226e-0c64-4737-8f2c-7b17352f5629
			- Higher thrust levels at the cost of higher required input power.
## Pulsed Plasma Thrusters
	- Pulsed Plasma Thrusters or PPT operate by creating a pulsed, high-current discharge across the exposed surface of a solid propellant (usually Teflon). The arc discharge, usually generated in a pulsed way by a spark plug, ablates the propellant material generating ionized molecules which are then accelerated. The current pulse usually has a duration of a few microseconds and is driven by a capacitor charged and discharged approximately once per second. A spring mechanism ensures that there is always a propellant surface which can be ablated close to the spark plug. The ablated propellant ions flow in a chamber between an anode and a cathode and, being conductive, close the electrical circuit generated by the voltage provided by a Power Processing Unit (PPU), thus allowing current to flow from the anode to the cathode. This current, in turn, produces a self-induced magnetic field, and the propellant ions are accelerated by a Lorentz force perpendicular to both the electric and the magnetic fields.
	  hl-page:: 25
	  ls-type:: annotation
	  hl-color:: blue
	- [[GPT Generated Flashcards]]
		- How do Pulsed Plasma Thrusters (PPT) operate? #card
		  id:: a1a6323e-bce8-457d-9d2d-ef5935183ce4
			- By creating a pulsed, high-current discharge across the exposed surface of a solid propellant, ablating the material and generating ionized molecules that are accelerated.
		- What is the typical solid propellant used in PPTs? #card
		  id:: ed2f4aee-5564-450f-91c1-788f788b1723
			- Teflon.
		- How is the arc discharge in PPTs usually generated? #card
		  id:: 23c6d06f-724c-4980-be22-b463cf4280be
			- By a spark plug.
		- What is the typical duration of a current pulse in PPTs? #card
		  id:: 80d4f0e5-e178-4505-b5fe-43909be9f385
			- A few microseconds.
		- How often does the capacitor charge and discharge in PPTs? #card
		  id:: 332866ee-1d6f-4d3b-ba44-e7b363e161a5
			- Approximately once per second.
		- What device ensures a propellant surface is available for ablation in PPTs? #card
		  id:: 209e054c-ce54-4f6a-9901-d371bf7421f7
			- A spring mechanism.
		- In a PPT, where do the ablated propellant ions flow? #card
		  id:: fce2f3af-ab4a-4852-98f4-c2f98bba1565
			- In a chamber between an anode and a cathode.
		- What happens when the ablated propellant ions close the electrical circuit in a PPT? #card
		  id:: 82e88fba-2717-4483-8bb5-9c8397322d9c
			- Current flows from the anode to the cathode. This current, in turn, produces a self-induced magnetic field.
		- What force accelerates the propellant ions in PPTs? #card
		  id:: 150349ed-a047-434f-a926-dff10b6999b7
			- Lorentz force.
		- What is the Lorentz force? #card
		  id:: a7442d43-9442-439a-be99-4fb94d4c4483
			- The Lorentz force is the force experienced by a charged particle moving through an electric and magnetic field.
	- The main advantages of Pulsed Plasma Thrusters are their ability to provide very small impulse bits for precision maneuvers, simplicity due to the relatively small number of components, possibility of using a wide range of propellants (not only solid but also in the liquid state) and adjusting the thrust level by varying the pulse frequency, fast response time to commands. However, they also suffer from major drawbacks such as rapid erosion of the electrodes, presence of non-ionized macro-particles in the exhaust plume due to non-uniform ablation, relatively high dry mass due to the bulky electronics required for their operation, and very low efficiency (typically in the 10-15% range)
	  ls-type:: annotation
	  hl-page:: 25
	  hl-color:: blue
	- A particular class of PPTs are the so-called Vacuum Arc Thrusters, which are based on exactly the same principle, with the only difference that propellant ablation is obtained by a vacuum arc instead of a spark plug. In this case the ions to be accelerated are ablated directly from the cathode material (which is therefore, as a matter of fact, the propellant itself), allowing for higher efficiency.
	  ls-type:: annotation
	  hl-page:: 26
	  hl-color:: blue
	- [[GPT Generated Flashcards]]
		- What are the main advantages of Pulsed Plasma Thrusters? #card
		  id:: 6eb110ec-9adb-4fc5-a88b-411af4247ca3
			- Small impulse bits for precision,
			  simplicity,
			  wide range of propellants,
			  adjustable thrust level,
			  fast response time.
		- What are the major drawbacks of Pulsed Plasma Thrusters? #card
		  id:: ec1bc003-e2e6-4f58-970f-6e04de08e01e
			- Rapid electrode erosion,
			  presence of non-ionized macro-particles,
			  high dry mass,
			  and low efficiency.
		- What is the typical efficiency range of Pulsed Plasma Thrusters? #card
		  id:: 1b802ebd-39af-4631-ae6b-4200f7541d8e
			- 10-15%
		- What is the key difference between Vacuum Arc Thrusters and Pulsed Plasma Thrusters? #card
		  id:: 83dfb6e0-1188-4384-9419-b4577e980f12
			- Vacuum Arc Thrusters use a vacuum arc for propellant ablation instead of a spark plug.
		- In Vacuum Arc Thrusters, what serves as the propellant? #card
		  id:: 1af4d487-4b59-4d4c-8104-4be531e7d055
			- The cathode material itself.
## Design Parameter Relationships
	- ### Thrust-Specific Impulse
		- All pure electric propulsion options can be found in the region of high specific impulse(typically 500 s or higher) and low thrust (typically a few mN or lower, with the only notable exception of Hall Effect and ion thrusters). Cold gas and resistojets allow for a wider range of thrust levels (from 0.1 mN to 0.1 N) but are typically limited to specific impulse values lower than 100 s. Chemical propulsion options are the only ones which allow for a thrust level higher than 0.1 N, but are confined to a narrow specific impulse range between 200 and 300 s.
		  ls-type:: annotation
		  hl-page:: 27
		  hl-color:: yellow
		- [[GPT Generated Flashcards]]
			- What propulsion options are found in the region of high specific impulse and low thrust? #card
			  id:: d96eecc3-0c58-465c-9f37-f9d0e0f10080
				- Pure electric propulsion options.
			- Which propulsion option has the highest specific impulse? #card
			  id:: 6468af8b-e4da-444e-955b-f77d0336fce7
				- Ion thrusters.
			- Which propulsion option has the lowest specific impulse? #card
			  id:: 6468b02d-9b1a-4f68-bfb8-b919ce7ae635
				- Cold gas systems.
			- What is the typical specific impulse for pure electric propulsion options? #card
			  id:: 575fd057-7f01-44cf-bdb0-bec8016977c0
				- 500 s or higher.
			- What is the typical thrust range for pure electric propulsion options? #card
			  id:: b3eaba4c-32bc-4db3-b1c4-cb193e172301
				- A few mN or lower.
			- What types of propulsion options allow for a wider range of thrust levels? #card
			  id:: cbee9b41-88be-4375-9cd8-8ac5d7922916
				- Cold gas and resistojets.
			- What is the thrust level range for cold gas and resistojets? #card
			  id:: 67550eeb-7768-40f3-b3ba-7f19b9e4e5b3
				- 0.1 mN to 0.1 N.
			- What is the upper limit specific impulse limit for cold gas and resistojets? #card
			  id:: 09e864d5-d517-407c-a638-5511dc3f4309
				- Around 100 s.
			- What type of propulsion allows for thrust levels higher than 0.1 N? #card
			  id:: f9031b5f-0f09-404a-bfba-cd2ce15474a6
				- Chemical propulsion options.
			- What is the specific impulse range for chemical propulsion options? #card
			  id:: a0f1bde5-01c9-4859-b194-6d47b64d65cf
				- 200 to 300 s.
	- ### Thrust-Power
		- As indirectly suggested by equation (1.10) in Chapter 2, the input power of an ion thruster is proportional, at least in a first simplified approximation, to the jet velocity squared v e2 . Looking at equation (1.7), this means that the input power is proportional to the grid voltage V and thus, from equation (1.8), the thrust is proportional to the input power squared
		  ls-type:: annotation
		  hl-page:: 27
		  hl-color:: yellow
		- In a logarithmic thrust-power chart (like the one in Figure 23) this translates into a “10/100” slope: when the power is increased by one order of magnitude (factor 10), the thrust increases by two orders of magnitude (factor 100)
		  ls-type:: annotation
		  hl-page:: 27
		  hl-color:: yellow
		- [[GPT Generated Flashcards]]
			- What is the input power of an ion thruster proportional to in a simplified approximation? #card
			  id:: 4001a8b7-86ff-4776-b31b-2b915611c153
				- Jet velocity squared (\(v_e^2\)).
			- What is the input power proportional to in relation to the grid voltage in ion thrusters? #card
			  id:: 258c315f-a2f3-43bb-a17b-eb7c23a5bc7d
				- Grid voltage (V).
			- In a logarithmic thrust-power chart for ion thrusters, what happens when power is increased by one order of magnitude? #card
			  id:: 95d85b06-6908-4663-a9af-16becf67d681
				- Thrust increases by two orders of magnitude.
	- ### Specific Impulse-Power
		- the specific impulse would be expected to be proportional to the square root of the power or, in other words, a “100/10” slope in the logarithmic chart of Figure 24. However, in the figure, this trend seems to be followed only by electrospray thrusters, with most of the other propulsion types showing very weak or even no clear relationship between specific impulse and power
		  ls-type:: annotation
		  hl-page:: 28
		  hl-color:: yellow
		- it is likely that a certain type of electric propulsion is preferred to always work in a given specific impulse range independently on the amount of input power required. This is probably a consequence of general efficiency considerations given that, in electric propulsion, the thruster efficiency is usually a direct function of the specific impulse and it is typically possible to find a specific impulse value for which efficiency is maximum.
		  ls-type:: annotation
		  hl-page:: 28
		  hl-color:: yellow
		- [[GPT Generated Flashcards]]
			- Which type of thruster is the only one which follows the trend of specific impulse being proportional to the square root of power in the logarithmic chart? #card
			  id:: d387f88e-9083-4fde-90cc-0e01dc6a4d34
				- Electrospray thrusters.
			- In electric propulsion, what is the relationship between thruster efficiency and specific impulse? #card
			  id:: ef6ed51c-215f-4257-a796-b5fbaceb5687
				- The thruster efficiency is usually a direct function of the specific impulse.
			- Is there a specific impulse value for which efficiency is maximum in electric propulsion? #card
			  id:: 33b35527-6be3-4bbe-90f6-5fd9159385cd
				- Yes.
	- ### Thrust-Power Ratio
		- As already anticipated by the thrust-power chart, resistojets offer a significantly higher thrust/power ratio than any other systems
		  ls-type:: annotation
		  hl-page:: 28
		  hl-color:: yellow
		- resistojets are an optimal solution when a thrust in the order of a few mN is required with an available input power in the order of a few W (as it typically happens in CubeSats or other similar small satellites).
		  ls-type:: annotation
		  hl-page:: 28
		  hl-color:: yellow
		- The second best option in terms of thrust/power ratio are Hall Effect thrusters (0.03-0.1 mN/W), but they are typically characterized by a thrust level in the order of 6 mN or higher which, combined to their thrust/power ratio range of values, leads to an input power of 100 W or higher, which is typically not compatible to the requirements of small satellites.
		  ls-type:: annotation
		  hl-page:: 28
		  hl-color:: yellow
		- All other options approximately cover the region below 0.05 mN/W, with just a few exceptions for some specific products.
		  ls-type:: annotation
		  hl-page:: 28
		  hl-color:: yellow
		- [[GPT Generated Flashcards]]
			- What is the primary advantage of resistojets? #card
			  id:: a1ec508a-933a-46d7-8356-66bfeea6ff2b
				- Higher thrust/power ratio.
			- What is the typical required thrust for CubeSats or small satellites? #card
			  id:: c86a7fd3-f252-45ea-8762-510617323b3b
				- A few mN.
			- What is the typical available input power for CubeSats or small satellites? #card
			  id:: c7f1638d-7cf6-4aa0-9664-8d9e53fd6601
				- A few W.
			- What is the second best option in terms of thrust/power ratio for micropropulsion? #card
			  id:: 32225b5e-fda4-4f17-aacd-e51f0237eab5
				- Hall Effect thrusters.
			- What is the typical thrust level of Hall Effect thrusters? #card
			  id:: 6eb931f7-105f-410f-84a9-6ac846722e5f
				- 6 mN or higher.
			- What is the typical input power required for Hall Effect thrusters? #card
			  id:: c94081df-3936-4a4e-97c9-a6f3c194c2f3
				- 100 W or higher.
			- Are Hall Effect thrusters generally compatible with the requirements of small satellites? #card
			  id:: a799617e-4fae-4171-9de5-fa85e7abf1e6
				- No.
			- What is the approximate maximum thrust/power ratio for other options besides resistojets and Hall Effect thrusters? #card
			  id:: 80470e59-0db2-4243-9ea1-1f260112c4d5
				- Below 0.05 mN/W.
	- ### Dry Mass
		- Looking at the dry mass as a function of thrust, a clearly increasing trend (higher dry mass with increasing thrust) can be observed for thrust levels up to 10 mN, while dry mass values tend to stay approximately constant for thrust levels higher than 10 mN. This can be explained by the fact that only cold gas or chemical propulsion systems are present in the thrust range of 10 mN or higher (with the only exception of Hall Effect thrusters). These systems are all based on accelerating the propellant in a nozzle: the thrust is proportional to chamber pressure and nozzle throat area; however, in micro-propulsion systems, the chamber pressure is typically low and the nozzle is normally very small, meaning that changing their values to modify the thrust level does not affect the mass of the whole system in a significant way.
		  hl-page:: 28
		  ls-type:: annotation
		  hl-color:: yellow
		  
		  Conversely, no clear trends can be observed in the dry mass as a function of the specific impulse. A slightly increasing trend seems to be present in the dry mass as a function of the input power, which can be explained by observing that systems requiring a higher power will typically also require more complex and heavier power management and conditioning components.
		- [[GPT Generated Flashcards]]
			- What trend can be observed for dry mass as a function of thrust up to 10 mN? #card
			  id:: 7c4166df-424c-45be-bdde-394671379b1a
				- Dry mass increases with increasing thrust.
			- What happens to dry mass values for thrust levels higher than 10 mN? #card
			  id:: 7800e842-7bae-4d64-9695-9e8cdeb6e5fb
				- They tend to stay approximately constant.
			- What type of propulsion systems are present in the thrust range of 10 mN or higher? #card
			  id:: 57499ec1-adfa-46b0-9c13-1b70386c94c4
				- Cold gas or chemical propulsion systems.
			- What is the only exception of propulsion systems in the thrust range higher than 10 mN? #card
			  id:: 24b751cd-edc5-423c-bc3b-4e088f5aefff
				- Hall Effect thrusters.
			- Why does changing chamber pressure and nozzle throat area in micro-propulsion systems not affect the mass significantly? #card
			  id:: 13b8740a-ee69-4676-948f-bb8857e9fd6b
				- Because in micro-propulsion systems, the chamber pressure is typically low and the nozzle is normally very small.
			- What trend can be observed in dry mass as a function of specific impulse? #card
			  id:: 931b9757-f9f1-4b27-ba21-9c12ce64165e
				- No clear trends.
			- Is there a trend in dry mass as a function of input power? #card
			  id:: de42cce8-c38c-4ad9-b2fd-ea1baace1313
				- Yes, a slightly increasing trend.
			- Why is there a slightly increasing trend in dry mass with higher input power? #card
			  id:: d35e3fd0-537c-4f07-a269-e622fdbf79db
				- Because systems requiring higher power usually require more complex and heavier power management and conditioning components.
			-