employees:: Simon Van Benten, Ulf Kemmsies
type:: company

- # Responsibilities
	- ## Model development in [[Reliability Engineering]]
		- ### 1. Availability modeling from Renewal Theory (thesis Bendara / Secuos Artis tool)
			- Papers to read
				- ![A_conceptual_interpretation_of_the_renewal_theorem_with_applications_JvN.pdf](../assets/A_conceptual_interpretation_of_the_renewal_theorem_with_applications_JvN_1645798049453_0.pdf)
					- {{embed [[hls__A_conceptual_interpretation_of_the_renewal_theorem_with_applications_JvN_1645798049453_0]]}}
					-
				- ![Bednara_thesis_2008 - Methds for approximating the availability functions.pdf](../assets/Bednara_thesis_2008_-_Methds_for_approximating_the_availability_functions_1645798062058_0.pdf)
					- {{embed [[hls__Bednara_thesis_2008_-_Methds_for_approximating_the_availability_functions_1645798062058_0]]}}
			- #### SecouS
				- {{renderer :linkpreview,https://www.securityofsupply.com/}}
					-
				- {{renderer :linkpreview,https://wiki.artis.la/doku.php}}
					- [[ARTIS]]
						- {{embed [[ARTIS]]}}
			-
		- ### 2. Weibull model for failure + suspension analysis (WeibullR package / Python reliability package as basis?) – automated reporting and web-based access
			- {{renderer :linkpreview,https://reliability.readthedocs.io/en/latest/}}
				- Pareto toolset:
					- Mean Cumulative Function: assess trend in failure arrival times over certain time period?
					- Weibull parameters MRR: obtain eta and beta parameter for Weibull failure distribution based on failure times (including identification of separate failure modes from the data)
					- Pareto charts 80/20: sort e.g. on top 10 number of failures, costs per failure, length of downtime, workload
					- Risk plot: assuming symmetric distribution of failure occurrence with associated costs, draw a simple log-plot with acceptance levels obtained from decision maker
		- ### 3. Proportional hazard model Jardine?
			- ![Proportional_hazards_Jardine.pdf](../assets/Proportional_hazards_Jardine_1645971985398_0.pdf)
				- {{embed [[hls__Proportional_hazards_Jardine_1645971985398_0]]}}
				-
			-
		- ### 4. CRISP DM for reliability engineering & asset management
			- What is CRISP-DM?
				- {{renderer :linkpreview,https://www.datascience-pm.com/crisp-dm-2/}}
					-
			- #### 1. Translate with applicable terms
			- #### 2. Case studies + content material --> Marketing?
		- ### 5. Dynamic simulation from systems theory / business dynamics simulation
			- Possible platforms/languages?
		- ### 6. Process historians time series to simple physical models, e.g.:
			- #### 1. Pump / compressor
			- #### 2. Gearbox
			- #### 3. Generalized models based on available measurement signals, and what to do if certain signals are not available
	-
	- ## Digital marketing
		- ### 1. Specialization guide (Philip Morgan model)
			- {{renderer :linkpreview,https://philipmorganconsulting.com/specialization-decision-guide/}}
				-
			- #### 1. Finalize model
			- #### 2. Map out potential leads
		- ### 2. LinkedIn Sales Navigator:
			- #### 1. Use outcome of specialization guide to map out potential interesting companies
			- #### 2. Generate leads
		- ### 3. Content
			- #### 1. Blog posts
			- #### 2. LinkedIn posts
			- #### 3. Website optimization
	-
	- ## Client work
		- ### 1. APM Terminals:
			- {{renderer :linkpreview,https://www.apmterminals.com/en/about/our-company}}
			- #### 1. Reliability data analyst - 1 day/week?
			- #### 2. Configuration management / document control
			- #### 3. FMECA - risk analysis - maintenance plan
				- {{renderer :linkpreview,https://quality-one.com/fmeca/}}
					-
			- #### 4. IFS data cleaning and management
				- {{renderer :linkpreview,https://www.ifs-certification.com/index.php/en/}}
					-
		- ### 2. Interim maintenance / reliability engineer (through intermediate firms.)
-
- 07:54 meeting notes [[20.05.2022]] :
	- Repairable/ Non-repairable
	- Distros: non-stationary stochastic process/Poisson process
		- NHPP (non-homogeneous)
	- Non-zero repair times
		- Repair times should be << than times between failures
		- Test this assumption
	- Outlier analysis: give good analysis of
	- Breakdown of systems into subsystems
	- Independences of failure: Markov property
		- This is implicit in statistical approaches
	- Probability of meeting MTBF in a given time
	- Control charts
	-
	- Formulating business problem into reliability problem
		- Use flowchart to place problem: Diagonstic tool on website
	-