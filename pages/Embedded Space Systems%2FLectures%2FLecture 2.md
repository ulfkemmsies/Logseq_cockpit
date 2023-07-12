- **Digital Signal Processor (DSP)**
  A DSP is an IC designed to process digital signals. Analog signals are converted to digital via an analog-to-digital converter before being processed in the DSP. Digital signals are then output and may be converted back to analog signals via a digital-to-analog converter.
  DSPs are specialized microprocessors which perform certain actions on the analog signal (such as filter, measure, compress) using algorithms more efficiently and with less power than a general purpose processor and within a strict deadline. DSPs are programmable.
	- **Application of DSPs**
	  DSP are mainly used in audio and speech processing telecommunications; radar, Lidar, sensors; visual processing, image processing.
	  Some DSPs are being used for neural networks processing.
	  In commercial market multi-cores DSPs are available.
	  In space engineering, DSPs are key components in payload data processing.
	- [[GPT Generated Flashcards]]
	  collapsed:: true
		- What is a Digital Signal Processor (DSP)? #card
		  id:: 642bb718-a333-4efc-987a-27532e842db3
			- An Integrated Circuit designed to process digital signals.
		- What must be done to analog signals before processing in a DSP? #card
		  id:: 642bb718-5fde-4d20-97b3-23924d426bbb
			- Conversion to digital using an analog-to-digital converter.
		- What makes DSPs more efficient than general purpose processors for certain actions on analog signals? #card
		  id:: 642bb718-6a92-4b18-9588-bf3299524102
			- Specialized microprocessors, algorithms, and less power consumption.
		- Are DSPs programmable? #card
		  id:: 642bb718-ab5b-470c-90bb-a4c968efb5b0
			- Yes.
- **Application Specific Integrated Circuit (ASIC)**
  Application Specific/Custom design circuits are needed if high speed and low power are the driving requirements.
  Used for special cases: e.g. mixed analog/digital signals.
  However design cost is very high, it can be compensated only by selling large numbers.
  Manufacturing cost can be reduced by using less advanced semiconductor fabrication techniques and/or multi-project wafers (MPW).
  Lack of flexibility (design errors requires a new mask set and new tape-out).
	- **ASIC Development**
	  ![image.png](../assets/image_1680543314421_0.png) 
	  Developing an ASIC is highly time consuming task because CAD and automatized techniques offer a limited help. Only the skills and continuous experience of the designer are key to ensure the all the features needed find their place in complex fabric of the semiconductor chip.
	  Hardware Description Language (HDL) is a key element to ensure compliance between the system requirements and the design implementation.
	  Verilog and VHDL are the most used in order to represent the desired \(\mathrm{HW}\) functionality as a software program. The model is then simulated to confirm the design will work as intended. Any problems can be corrected in the model, and simulation will verify the correction.
	- **VHDL vs Verilog**
	  VHDL is a strongly typed language and more verbose than Verilog.
	  VHDL syntax is non-C-like and extra coding is required to convert from one data type to another.
	  Verilog is probably the easiest to grasp and understand, but VHDL has more features for high level modelling therefore mosre suitabl for advanced users.
	  Another option is ModelSim, a multi-language environment which supports both.
	- **ASIC Floorplan**
	  After the architecture design, a set of functional blocks and the connections between them are specified in the netlist.
	  These functional blocks can be considered as macrocells in the physical design.
	  The task of floorplan is to place the macrocells on a 2-D chip: it determines the size of the design cell (or die), creates the boundary and core area, and creates wire tracks for placement of standard cells. It is also a process of positioning blocks or macros on the die. All this should be done without overlap while also optimizing design objectives such as timing, congestion, and maximum single and total wire length.
	  This is where experience plays a very important role but nowadays due to the complexity of modern chips automated methods are becoming predominant.
	- [[GPT Generated Flashcards]]
	  collapsed:: true
		- What is ASIC development? #card
		  id:: 642bb718-cf56-4ab7-bddb-fb583782321b
			- A time-consuming task of designing a semiconductor chip using CAD and automation techniques.
		- What is the importance of Hardware Description Language (HDL)? #card
		  id:: 642bb718-a087-42a5-9678-fa9a19612ad3
			- It ensures compliance between system requirements and design implementation.
		- Which two HDLs are most commonly used? #card
		  id:: 642bb718-13a9-4d5e-b312-413876fc0e54
			- Verilog and VHDL.
		- What is the purpose of simulating an HDL model? #card
		  id:: 642bb718-c547-451a-83cb-14c66c59ac1a
			- To confirm the design will work as intended and correct any problems.
		- What is a key difference between VHDL and Verilog? #card
		  id:: 642bb718-d692-407d-9a32-c783554addb1
			- VHDL is more verbose and strongly typed, while Verilog is easier to grasp with a C-like syntax.
		- What is ModelSim? #card
		  id:: 642bb718-0dff-4868-b378-07af3cefbe8e
			- A multi-language environment supporting both Verilog and VHDL.
		- What is the role of the ASIC floorplan? #card
		  id:: 642bb718-2a28-4f6e-9a62-84835d6e50c7
			- To place macrocells on a 2-D chip, determine the size of the design cell, create the boundary and core area, and create wire tracks for standard cell placement.
		- What kind of layout is created in the ASIC floorplan? #card
		  id:: 642bb718-aed3-4920-914b-f01efd7a906f
			- A layout of functional blocks and connections between them, specified in the netlist.
		- What is one major factor in successful ASIC floorplanning? #card
		  id:: 642bb718-504c-4167-b912-7718bc6320bf
			- Experience of the designer, although automated methods are becoming more common due to increasing complexity.
	- [[GPT Generated Flashcards]]
	  collapsed:: true
		- What is an Application Specific Integrated Circuit (ASIC)? #card
		  id:: 642bb718-7862-4dbd-a442-f1bc42fd091e
			- A custom design circuit for high speed and low power requirements.
		- When are ASICs typically used? #card
		  id:: 642bb718-c6ce-4b97-9740-d483781d5f73
			- For special cases like mixed analog/digital signals.
		- Why are ASICs costly to design? #card
		  id:: 642bb718-2cc5-499f-9d68-b9b4b33dbc41
			- Due to high design costs and the need to sell large numbers to compensate.
		- How can the manufacturing cost of ASICs be reduced? #card
		  id:: 642bb718-e9bc-4450-85c3-cae07cc278ab
			- Using less advanced fabrication techniques and/or multi-project wafers (MPW).
		- What is an issue in ASICs flexibility? #card
		  id:: 642bb718-ff66-40ef-88fd-b74589363075
			- Design errors require a new mask set and new tape-out.
- **Field Programmable Gate Arrays**
  ![image.png](../assets/image_1680543541053_0.png) 
  FPGAs are the most common of reconfigurable hardware.
  These devices can be programmed "in the field" (after manufacturing)
  FPGAs consists of many interconnected Configurable Logic Block
	- **Configurable Logic Blocks**
	  Each Configurable Logic Block consist of 2 slices.
	  Those slices are further divided in 2 logic elements.
	  
	  Logic elements consist of:
	  4 input lookup Table
	  Full Adder and Mux logic
	  D FlipFlop
	  Configurable Logic blocks
	  I/O Units
	  Interconnections
	- **Lookup Tables**
	  ![image.png](../assets/image_1680543679485_0.png) 
	  A Lookup Table, as the name suggests, is an actual table that generates an output based on the inputs.
	  This table is then stored in a small memory. Inputs \(A\) and \(B\) are the address pins and \(C\) is the data pin.
	  When your address pins are changing, they will be pointing at a different address with different inputs.
	  2 inputs means 4 different combinatorial scenarios. You can increase the number of inputs and modify accordingly the size of the memory needed.
	- **Flip-Flops**
	  Flip-flops are devices with two stable states that can be used to store binary data. The stored data can be changed by applying varying inputs.
	- **Programming an FPGA**
	  Programming an FPGA is called configuration.
	  Programming an FPGA is **not** like programming a microprocessor.
	  We download a **bitstream** (in bits as 1s or 0s) to the FPGA, not a program
	  The bitstream determines the logic functions performed by the Logic Elements, and the interconnecting switches in order to connect the different Logic Elements together to make up your circuit
	  This is done only once at power-on while a microprocessor needs to be fed these program codes continuously for it to function.
	- The **on-board data handling (OBDH)** of a spacecraft is the subsystem which carries, elaborates and stores data between the various electronics units and the ground segment, via the telemetry, tracking and command (TTC) subsystem.
		- The OBDH has many **functions**:
		  Reception and execution of commands from Ground Data collection, formatting and transmission to Ground Time distribution
		  Spacecraft health monitoring
		  Fault detection Isolation and recover (FDIR)
		  Provision of data storage for program and data
		  Execution of command schedules
		  Execution of control algorithms
		  Security
		  Data processing/compression
	- The **Avionics** are the various electronic systems making spacecraft 'cyber physical system'- some of them are 'sensors', some others are actuators.