- Embedded Systems Memory Types
	- Fixed
		- The content of the memory is physically fixed by the structure of the memory element.
		- Examples: core rope memories (wire wound through or around a core, used in Apollo) or antifuse-based PROMs (Programmable Read-Only Memories).
		- Fixed
	- Erasable
		- The contents of the memory is non-volatile, but the contents can be changed. In many cases this involves an erase operation and then a write.
		- Examples: core, plated wire, electrically erasable programmable read only memories (EEPROM), erasable read only memories (EPROM), ferroelectric memories, and flash.
	- Volatile
		- The content of the memory is volatile: these memories do not retain content either after the cycling of power or during "brown out" conditions.
		- Examples: SRAM, DRAM, and SDRAM
	- Programmable Read-Only Memories (PROMs)
		- PROMs are used in digital electronic devices to store permanent data, usually low level programs such as firmware.
		- Each bit contains both a fuse and an antifuse and is programmed by triggering one of the two.
		- Difference between ROM and PROM is that data are written into ROM at manufacturing while PROM are programmed once after manufacturing.
	- [[GPT Generated Flashcards]]
		- What are the four main types of memories? #card
		  card-last-interval:: -1
		  card-repeats:: 1
		  card-ease-factor:: 2.5
		  card-next-schedule:: 2023-04-03T22:00:00.000Z
		  card-last-reviewed:: 2023-04-03T06:12:04.536Z
		  card-last-score:: 1
		  id:: 64296f3e-2d98-4396-ae25-0af899fe68fa
			- Fixed, erasable, volatile, and Programmable Read-Only Memories (PROMs).
		- What is fixed memory? #card
		  card-last-interval:: 4
		  card-repeats:: 1
		  card-ease-factor:: 2.36
		  card-next-schedule:: 2023-04-07T06:13:22.383Z
		  card-last-reviewed:: 2023-04-03T06:13:22.383Z
		  card-last-score:: 3
		  id:: 64296f3e-a2db-4a44-9c1b-8407b2b67b0d
			- Fixed memory refers to the type of memory that cannot be altered by a user once it has been programmed.
		- What is erasable memory? #card
		  id:: 64296f3e-b637-4c5f-a9d6-53b5466816d5
			- Erasable memory allows users to remove or erase data stored in the memory.
		- What is volatile memory? #card
		  id:: 64296f3e-1332-4d04-ac2d-6eefe5ef99bd
			- Volatile memory is temporary and requires power to maintain the data stored in it.
		- What are Programmable Read-Only Memories (PROMs)? #card
		  id:: 64296f3e-977b-4396-bc9b-1989724c964b
			- Programmable Read-Only Memories (PROMs) are integrated circuits that contain preset data that cannot be changed by the user.
		- What is the difference between PROM and ROM? #card
		  id:: 64296f3e-8900-430e-9e2b-e131bb53f49c
			- Data are written into ROM at manufacturing while PROM are programmed once after manufacturing.
	- Erasable Memories
		- PROM, EPROM, EEPROM and flash are the types of ROM.
		- The main difference between PROM and EPROM is that the PROM can be programmed just once whereas EPROM is erasable (=it can be reprogrammed or rewritten).
		- EPROM is erased using Ultra violet rays whereas, EEPROM can be erased using electric signals.
		- | Memory | PROM | EPROM | EEPROM |
		  | :--- | :--- | :--- | :--- |
		  | Meaning | Programmable Read Only Memory| Erasable Programmable Read Only Memory  |  Electrically Erasable Read-Only Memory  |
		  | Programmability | One-time programmable only |  The chip is reprogrammable  | The chip is reprogrammable and Erasing |
		  | Cost | Cheap | Expensive | Expensive |
		  | Packaging |  PROM is encased in  plastic covering.  |  A transparent quartz window cover EPROM.  |  Encased in opaque plastic case  |
		  |  Storage Endurance  |  High (PROM are no affected by radiation)  |  EPROM are guaranteed for 10 yrs however radiation and electric noise can affect the storage stability  | Same as EPROM |
			- [[GPT Generated Flashcards]]
			  Question: How many times can PROM be programmed?
			  Answer: One-time programmable only
			  
			  Question: How does the cost of PROM compare to the other two types of memory?
			  Answer: Cheap
			  
			  Question: What is the packaging for PROM?
			  Answer: Encased in plastic covering
			  
			  Question: How can EPROM be reprogrammed?
			  Answer: The chip is reprogrammable.
			  
			  Question: What is the packaging for EPROM?
			  Answer: A transparent quartz window cover EPROM
			  
			  Question: What factors can affect EPROM storage stability?
			  Answer: Radiation and electric noise
			  
			  Question: What is the storage endurance for EPROM?
			  Answer: Guaranteed for 10 years
			  
			  Question: How is EEPROM different from EPROM for programming and erasing?
			  Answer: The chip is 
			  reprogrammable and erasing
			  
			  Question: What is the packaging for EEPROM?
			  Answer: Encased in opaque plastic case
			  
			  Question: What is the storage endurance for EEPROM compared to EPROM?
			  Answer: The same
	- [[GPT Generated Flashcards]]
		- What are erasable memories? #card
		  id:: 64296f3e-c7f4-4fb9-b40b-a42f62c22a1d
			- Electronic devices that can be erased and reprogrammed multiple times.
		- What are two types of erasable memories? #card
		  id:: 64296f3e-6222-4009-b5b6-4ef97352d8ea
			- EPROM and EEPROM.
		- What does EPROM stand for? #card
		  id:: 64296f3e-899c-4ab1-908d-fe8a19cf561c
			- Erasable Programmable Read Only Memory.
		- What does EEPROM stand for? #card
		  id:: 64296f3e-b8d9-430d-b483-3686198468ac
			- Electrically Erasable Programmable Read Only Memory.
		- How is data erased in EPROM? #card
		  id:: 64296f3e-6351-4730-9bbc-b9a19a9ec3e3
			- By exposing the memory chip to ultraviolet light.
		- How is data erased in EEPROM? #card
		  id:: 64296f3e-ccfc-4bca-ba26-1cd045255c24
			- By applying an electrical voltage to the chip.
		- What is one advantage of EEPROM over EPROM? #card
		  id:: 64296f3e-09f4-4da0-b22e-7921452563fc
			- EEPROM can be erased and reprogrammed without removing the chip from the device.
	- Boot Memories in space
		- In space designs boot memory architecture have been kept unchanged since the early times of ERC32.
		- We have PROMs (mostly 32k) + EEPROMs, all with 8 bit access.
		- In years we have seen an exponentially accelerating increase of installed boot memory size in space missions
		- [[GPT Generated Flashcards]]
			- What has remained unchanged in space designs since the early times of ERC32? #card
			  id:: 64296f3e-f217-4e53-b379-8211f7a34569
				- Boot memory architecture.
			- What are the two types of memory used in space designs? #card
			  id:: 64296f3e-6628-4800-8d5c-491bd7472aa6
				- PROMs and EEPROMs.
			- What is the access size of PROMs and EEPROMs in space designs? #card
			  id:: 64296f3e-f89f-4d61-87c9-f16b9b415734
				- 8 bit.
			- What is the common size of a PROM in space designs? #card
			  id:: 64296f3e-7a52-46df-99fa-49a85f5b9370
				- 32k.
			- What has been happening to the installed boot memory size in space missions over the years? #card
			  id:: 64296f3e-dce3-499e-9e16-736c7d6994a4
				- Exponentially accelerating increase.
	- Flash memories
		- Flash memories are electrically modifiable, non-volatile storage
		- Principle of operation:
			- The data are stored by removing or putting electrons on its floating gate.
			- Charge on floating gate affects the threshold of the memory element.
				- When electrons are present on the floating gate, no current flows through the transistor, indicating a logic-0.
				- When electrons are removed from the floating gate, the transistor starts conducting, indicating a logic-1.
				- This is achieved by applying voltages between the control gate and source or drain.
		- Uses 2 different technologies: NAND and NOR
			- The market is dominated by NAND but NOR has its niche especially in embedded systems
			- NAND Flash cell was designed with a very small size to enable a low cost-per-bit of stored data, and has been used primarily as a high-density data storage medium for consumer devices.
			- NOR Flash cell is bigger, but more robust, but has typically been used for code storage and direct execution in portable electronics devices, such as mobile phones.
			- NAND is accessible in PAGES, while NOR allows RANDOM access.
			- Choosing NAND or NOR Flash depends on the advantage of each technologe:
				- NOR has low standy power, easy code execution, and high read speeds
				- NAND has low cost-per-bit, easy file storage use, low active power, high write speed, and high capacity
			- [[GPT Generated Flashcards]]
				- What type of storage is flash memory? #card
				  id:: 64296f3e-2ecf-4efd-9592-12820da76d8e
					- Electrically modifiable, non-volatile storage.
				- How is data stored in flash memory? #card
				  id:: 64296f3e-17d5-4a4a-b863-e5ef527cc379
					- By removing or putting electrons on its floating gate.
				- What does the charge on the floating gate affect? #card
				  id:: 64296f3e-8662-4acb-87e6-e4943514f421
					- The threshold of the memory element.
				- What does it mean when no current flows through the transistor in flash memory? #card
				  id:: 64296f3e-07c9-4a02-94df-6e6c2bc4e615
					- It indicates a logic-0.
				- What does it mean when the transistor starts conducting in flash memory? #card
				  id:: 64296f3e-fa5c-4549-8119-8c135e81df36
					- It indicates a logic-1.
				- What are the two main technologies used in flash memory? #card
				  id:: 64296f3e-8f9d-42bf-aa2e-326d58efe8f4
					- NAND and NOR.
				- Which flash memory technology is more commonly used? #card
				  id:: 64296f3e-e01c-4621-be9e-b3b8e7a1c005
					- NAND.
				- Where is NOR flash memory typically used? #card
				  id:: 64296f3e-33b9-4e6e-a35a-a9bad4a40cbb
					- In embedded systems, such as mobile phones.
				- What is the primary use of NAND flash memory? #card
				  id:: 64296f3e-6919-43fe-a8f1-17508b0fb9c1
					- High-density data storage for consumer devices.
				- How is data in NAND flash memory accessed? #card
				  id:: 64296f3e-6291-4a40-bc6d-597a099e0d16
					- In pages.
				- How is data in NOR flash memory accessed? #card
				  id:: 64296f3e-9d80-440e-aa83-12711d8db285
					- Random access.
				- What factors determine the choice between NAND and NOR flash memory? #card
				  id:: 64296f3e-3182-4cb0-b7b8-a3e2d62e8689
					- The advantages of each technology.
	- Flash memories vs EEPROM?
		- Flash is just one type of EEPROM.
		- Flash uses NAND-type memory, while EEPROM uses NOR type.
		- Flash is block-wise erasable, while EEPROM is byte-wise erasable.
		- Flash is constantly rewritten, while other EEPROMs are seldom rewritten.
		- Flash is used when large amounts are needed, while EEPROM is used when only small amounts are needed.se of NAND vs. NOR Flash in embedded systems is an important trade off.
		- [[GPT Generated Flashcards]]
			- What type of memory does Flash use? #card
			  id:: 64296f3e-e2d5-4d0b-bb9e-216fbb2df5c5
				- NAND-type.
			- What type of memory does EEPROM use? #card
			  id:: 64296f3e-ac7a-4077-aa48-149105a0e337
				- NOR type.
			- How is Flash memory erased? #card
			  id:: 64296f3e-9fda-4f98-9fbe-ab58d717bfea
				- Block-wise.
			- How is EEPROM memory erased? #card
			  id:: 64296f3e-ab56-437b-9d5e-8b046377432c
				- Byte-wise.
			- How often is Flash memory typically rewritten? #card
			  id:: 64296f3e-a374-4ece-92b3-ab3b1767178c
				- Constantly.
			- How often are EEPROMs (other that Flash) typically rewritten? #card
			  id:: 64296f3e-f3cc-484c-92cd-939ee22ba972
				- Seldom.
			- When is Flash memory typically used? #card
			  id:: 64296f3e-1ddb-42bc-bbdb-f3e888e909e0
				- When large amounts are needed.
			- When is EEPROM memory typically used? #card
			  id:: 64296f3e-f93a-4eb3-9fee-947c1263a69f
				- When small amounts are needed.
		- [[GPT Generated Flashcards]]
			- What type of storage is flash memory? #card
			  id:: 64296f3e-1904-4471-b792-2fbabacc64ed
				- Electrically modifiable, non-volatile storage.
			- How is data stored in flash memory? #card
			  id:: 64296f3e-f9c0-4f5b-8c8a-76733758da7e
				- By removing or putting electrons on its floating gate.
			- What indicates a logic-0 in flash memory? #card
			  id:: 64296f3e-5048-46f5-8a7e-5dfe6358b1d9
				- No current flows through the transistor when electrons are present on the floating gate.
			- What indicates a logic-1 in flash memory? #card
			  id:: 64296f3e-5639-42e2-b6b8-c703cff17814
				- The transistor starts conducting when electrons are removed from the floating gate.
			- What are the two main technologies used in flash memory? #card
			  id:: 64296f3e-d04a-450a-b82a-75ce22440ea2
				- NAND and NOR.
			- What is the primary use of NAND Flash? #card
			  id:: 64296f3e-102d-4844-8fbe-76667cdde829
				- High-density data storage medium for consumer devices.
			- What is the main use of NOR Flash? #card
			  id:: 64296f3e-d80f-4481-9acc-e7b97bc4a601
				- Code storage and direct execution in portable electronics devices.
			- In which access mode is NAND available? #card
			  id:: 64296f3e-fc8a-40b0-ad2d-628749e5445d
				- Pages.
			- How does NOR allow data access? #card
			  id:: 64296f3e-7b99-40b6-89bc-807bc8111bfd
				- Random access.
			- Which technology has low standby power, easy code execution, and high read speeds? #card
			  id:: 64296f3e-7826-4188-98d7-1925be98efc3
				- NOR.
			- What are the advantages of NAND? #card
			  id:: 64296f3e-4b4e-4fb2-adaa-d5618b68f565
				- Low cost-per-bit, easy file storage use, low active power, high write speed, and high capacity.
			- How is Flash memory related to EEPROM? #card
			  card-last-interval:: -1
			  card-repeats:: 1
			  card-ease-factor:: 2.5
			  card-next-schedule:: 2023-04-03T22:00:00.000Z
			  card-last-reviewed:: 2023-04-03T06:12:35.979Z
			  card-last-score:: 1
			  id:: 64296f3e-d9da-41d4-a750-8c386b974299
				- Flash is a type of EEPROM.
			- What type of memory does Flash use? #card
			  id:: 64296f3e-259c-446a-9204-dad153d3f6e0
				- NAND-type.
			- What type of memory does EEPROM use? #card
			  id:: 64296f3e-4069-47e4-a6f6-270cf98e73a9
				- NOR type.
			- How is Flash memory erasable compared to EEPROM? #card
			  id:: 64296f3e-2e4c-4d93-a947-7cabb65ac059
				- Flash is block-wise erasable while EEPROM is byte-wise erasable.
			- When is Flash memory typically used compared to EEPROM? #card
			  id:: 64296f3e-9ac9-4501-b0ac-83e434df9f3c
				- Flash is used when large amounts are needed, while EEPROM is used when only small amounts are needed.
	- Volatile memories
		- Random Access Memory (RAM) are volatile memories: retains the data bits in its memory as long as power is being supplied.
		- RAM is a semiconductor device internal to the integrated chip that stores data or machine code.
		- The Random-Access allows to read/write in the same amount of time irrespective of the physical location of the data inside the memory.
		- There are 2 main types of volatile memories:
		- DRAM (Dynamic Random Access Memory)
			- The Dynamic Random Access Memory is a type of RAM module that stores each bit of data within a separate capacitor. The level of charge on the memory cell capacitor determines whether that particular bit is a logical "1" or "0" (charge present = logical "1" and charge absent \(=\) logical "0").
			- This is an efficient way to store the data in memory because it requires less physical space to store the data.
			- It is also very simple and as a result it can be densely packed on a silicon chip and this makes it very cheap.
			- A particular size of DRAM can hold more amounts of data than a SRAM chip with the same size.
			- The capacitors in DRAM need to be constantly recharged to keep their charge. This is the reason why DRAM requires more power.
		- SRAM (Static Random Access Memory).
			- Single bit is stored in a bi-stable circuit
			- SRAM does not need to be refreshed periodically.
			- SRAMs provide fast access to the data.
			- Almost all the 'on chip' volatile memories in microcontrollers and processors (like caches and register file within the processor core) are made with SRAM allowing high performances and lower power consumption (against a lower density)
			- [[GPT Generated Flashcards]]
				- What does RAM stand for? #card
				  id:: 64296f3e-5ae1-4575-8c0f-05b3a367fd41
					- Random Access Memory.
				- What is a key feature of RAM memory regarding power supply? #card
				  id:: 64296f3e-771d-4fdb-bd52-eba5e8b98b21
					- It is volatile.
				- What is the function of RAM in a computer? #card
				  id:: 64296f3e-614e-4841-9299-16a3c6aeb68b
					- Storing data or machine code.
				- How does Random-Access in RAM work? #card
				  id:: 64296f3e-af60-40ac-8428-f005d7b747a2
					- It allows read/write in the same amount of time irrespective of the data location in memory.
				- What is DRAM? #card
				  card-last-interval:: 4
				  card-repeats:: 1
				  card-ease-factor:: 2.6
				  card-next-schedule:: 2023-04-07T06:06:46.570Z
				  card-last-reviewed:: 2023-04-03T06:06:46.570Z
				  card-last-score:: 5
				  id:: 64296f3e-fc7b-4a0a-8ad5-8fa940a0df6a
					- Dynamic Random Access Memory.
				- How does DRAM store data bits? #card
				  id:: 64296f3e-3c12-48da-a9da-a38d0efbe404
					- In separate capacitors.
				- What is the advantage of DRAM's data storage method? #card
				  id:: 64296f3e-d84f-48ce-a1c6-fbecfbdb3688
					- It requires less physical space.
				- What determines the logical state of a bit in DRAM? #card
				  id:: 64296f3e-4212-4888-83b5-20376c885f54
					- The level of charge on the memory cell capacitor.
				- Why does DRAM require more power than other types of RAM? #card
				  id:: 64296f3e-ca27-445c-92a8-3f90141b500c
					- Capacitors in DRAM need to be constantly recharged.
				- What is SRAM? #card
				  card-last-interval:: -1
				  card-repeats:: 1
				  card-ease-factor:: 2.5
				  card-next-schedule:: 2023-04-03T22:00:00.000Z
				  card-last-reviewed:: 2023-04-03T06:18:37.374Z
				  card-last-score:: 1
				  id:: 64296f3e-16c5-41e6-93a2-db1cfd71094e
					- Static Random Access Memory.
				- How does SRAM store a single bit? #card
				  id:: 64296f3e-b2b6-43ba-b28c-3dc6bd8bbe6a
					- In a bi-stable circuit.
				- Does SRAM need to be refreshed periodically like DRAM? #card
				  id:: 64296f3e-271b-4d0f-9386-b4c4c2b899e0
					- No.
				- What is an advantage of SRAM regarding data access? #card
				  id:: 64296f3e-0218-436b-aee5-fa2e8ec38328
					- It provides fast access to data.
				- What type of RAM is commonly found in microcontrollers and processors? #card
				  id:: 64296f3e-3058-452a-9229-c4ba296cff2e
					- SRAM.
		- SRAM vs. DRAM
			- SRAM are very robust and have low (static) power consumption.
			- SRAM devices can be found in large variety of of capacities and organizations (from very small to rather large).
			- SRAMs typically have very low latency and high performance.
			- SRAM memory can be designed and interfaced very easily compared to other memories
			- DRAM storage capacity is very high (more than 10x SRAM)
			- DRAM is a low cost/bit device
			- Although random access is not fast it can be 'pipelined' to access adjacent blocks in very efficient way.
			- [[GPT Generated Flashcards]]
				- What is a notable advantage of SRAM regarding power consumption? #card
				  card-last-interval:: 4
				  card-repeats:: 1
				  card-ease-factor:: 2.36
				  card-next-schedule:: 2023-04-07T06:03:06.992Z
				  card-last-reviewed:: 2023-04-03T06:03:06.993Z
				  card-last-score:: 3
				  id:: 64296f3e-dea7-42eb-be1c-deef6b512860
					- Low (static) power consumption.
				- What is a key benefit of SRAM for performance? #card
				  id:: 64296f3e-8357-4be9-970b-a0ec90b82bd0
					- Low latency.
				- What is an advantage of SRAM in device design? #card
				  id:: 64296f3e-8e95-4c0c-8cdf-669c103d0903
					- Easy to design and interface.
				- How does DRAM storage capacity compare to SRAM? #card
				  id:: 64296f3e-7302-4a4f-b027-54120acece88
					- More than 10x higher.
				- What is a benefit of DRAM regarding cost? #card
				  id:: 64296f3e-41b8-44a5-a987-b1e224d08c73
					- Low cost per bit.
				- What technique can be used to increase efficiency in DRAM access? #card
				  id:: 64296f3e-73d8-4d17-b34f-5c2e74c4e30a
					- Pipelining.
- Memory mapping
	- Memory mapping is a common technique for interfacing a peripheral to a processor.
	- With memory mapping a set of functions or settings are broken out and mapped to a set of values that are selected by a given address.
	- [[GPT Generated Flashcards]]
		- What is memory mapping? #card
		  id:: 64296f3e-e16b-4e62-8e88-11799f392fcf
			- A technique for interfacing a peripheral to a processor.
		- What happens to functions or settings in memory mapping? #card
		  id:: 64296f3e-fa66-4f72-85ed-65b0cbbf7888
			- They are mapped to a set of values.
		- How are values selected in memory mapping? #card
		  id:: 64296f3e-bbba-4024-af16-aea9938e62f1
			- By a given address.
	- Example: the PORT registers of an ATmega microcontroller (used in Arduino).
		- If in the code you write something like PORTB 0xAA, this will set the 8 IO pins designated to PORTB to the value 0xAA.
		- PORTB is a pointer to a special memory address. This address in memory maps to an IO peripheral that takes the value and outputs it to the IO pins.
- Embedded Systems Communication Protocols
	- UART (Universal Asynchronous Receiver-Transmitter)
		- Serial communication of bits via a single signal, i.e. UART provides parallel-to-serial and serial-to-parallel conversion.
		- Sender and receiver need to agree on the transmission rate.
		- Transmission of a serial packet starts with a start bit, followed by data bits and finalized using a stop bit
		- [[GPT Generated Flashcards]]
			- What does UART provide? #card
			  id:: 64296f3e-109b-4059-b4ed-0a9a124c1cb6
				- Parallel-to-serial and serial-to-parallel conversion.
			- What do sender and receiver need to agree on? #card
			  card-last-interval:: -1
			  card-repeats:: 1
			  card-ease-factor:: 2.5
			  card-next-schedule:: 2023-04-03T22:00:00.000Z
			  card-last-reviewed:: 2023-04-03T06:07:01.870Z
			  card-last-score:: 1
			  id:: 64296f3e-a13f-4e34-b889-8ba13c6b8b9d
				- Transmission rate.
			- What begins the transmission of a serial packet? #card
			  card-last-interval:: -1
			  card-repeats:: 1
			  card-ease-factor:: 2.5
			  card-next-schedule:: 2023-04-03T22:00:00.000Z
			  card-last-reviewed:: 2023-04-03T06:02:57.585Z
			  card-last-score:: 1
			  id:: 64296f3e-33db-4d3c-881d-ab0e3a3c4d7f
				- A start bit.
			- After data bits, how is the transmission finalized? #card
			  id:: 64296f3e-f5e1-45d9-abc6-1fb3a14bce3a
				- Using a stop bit.
	- SPI (Serial Peripheral Interface Bus)
		- SPI is used typically to communicate across short distances.
		- SPI characteristics:
			- 4 logic signals which are synchronised
			- SCLK: Serial Clock (output from master)
			- MOSI: Master Out Slave In (data output from master)
			- MISO: Master In Slave Out (data output from slave)
			- SS: Slave Select (often active low, output from master)
			- [[GPT Generated Flashcards]]
				- What does SCLK stand for? #card
				  id:: 64296f3e-448b-4b58-871c-df245f57ec66
					- Serial Clock
				- What is the function of SCLK? #card
				  id:: 64296f3e-0e31-455e-81c7-810df0ae51ab
					- Output from master
				- What does MOSI represent? #card
				  id:: 64296f3e-5228-4192-99f0-51ea1bc20019
					- Master Out Slave In
				- What is the purpose of MOSI? #card
				  id:: 64296f3d-23c4-4ed2-a839-687e4429f99e
					- Data output from master
				- What does MISO mean? #card
				  id:: 64296f3d-411b-4f6c-a6d6-9d6b226ae834
					- Master In Slave Out
				- What is the role of MISO? #card
				  card-last-interval:: -1
				  card-repeats:: 1
				  card-ease-factor:: 2.5
				  card-next-schedule:: 2023-04-03T22:00:00.000Z
				  card-last-reviewed:: 2023-04-03T06:09:54.681Z
				  card-last-score:: 1
				  id:: 64296f3d-06e8-42b2-8487-87808637ffe7
					- Data output from slave
				- What is the abbreviation for Slave Select? #card
				  id:: 64296f3d-aa0e-4bd8-b39a-a0bb55e35d5c
					- SS
				- What is the function of SS? #card
				  id:: 64296f3d-7e6a-4cc5-a661-ea6ccf781ed6
					- Often active low, output from master
		- SPI supports one single master and multiple slaves
		- always full-duplex: it communicates in both directions simultaneously
		- a speed of several Mbps can be achieved
		- transfer data in 4 to 16 bit serial packets
		- SPI Timing
			- In addition to setting the clock frequency, the master must also configure the clock polarity and phase with respect to the data
			- CPOL determines the polarity of the clock which can be converted
			- CPOL=0 is a clock which idles at 0 , and each cycle consists of a pulse of 1 . That is, the leading edge is a rising edge, and the trailing edge is a falling edge.
			- CPOL=1 is a clock which idles at 1 , and each cycle consists of a pulse of 0 . That is, the leading edge is a falling edge, and the trailing edge is a rising edge.
			- CPHA determines the phase of the data bits relative to the clock pulses.
			- CPHA=0 cycle consists of a half cycle with the clock idle, followed by a half cycle with the clock asserted.
			- CPHA=1 cycle consists of a half cycle with the clock asserted, followed by a half cycle with the clock idle.
		- [[GPT Generated Flashcards]]
			- What is SPI typically used for? #card
			  card-last-interval:: -1
			  card-repeats:: 1
			  card-ease-factor:: 2.5
			  card-next-schedule:: 2023-04-03T22:00:00.000Z
			  card-last-reviewed:: 2023-04-03T06:03:58.600Z
			  card-last-score:: 1
			  id:: 64296f3d-48ba-41fd-8b19-00ec9ab94a3b
				- Communicating across short distances.
			- How many masters does SPI support? #card
			  id:: 64296f3d-16c5-422c-a227-c20c912e4f04
				- One single master.
			- How many slaves can SPI support? #card
			  id:: 64296f3d-c44c-4832-99c7-74f8028866df
				- Multiple slaves.
			- What type of communication does SPI use? #card
			  card-last-interval:: -1
			  card-repeats:: 1
			  card-ease-factor:: 2.5
			  card-next-schedule:: 2023-04-03T22:00:00.000Z
			  card-last-reviewed:: 2023-04-03T06:14:25.543Z
			  card-last-score:: 1
			  id:: 64296f3d-1a54-45ba-99cc-4eff3e2ce53a
				- Full-duplex communication.
			- What speed can SPI achieve? #card
			  card-last-interval:: -1
			  card-repeats:: 1
			  card-ease-factor:: 2.5
			  card-next-schedule:: 2023-04-03T22:00:00.000Z
			  card-last-reviewed:: 2023-04-03T06:15:12.990Z
			  card-last-score:: 1
			  id:: 64296f3d-0386-4065-8807-84c30ca8a6c5
				- Several Mbps.
			- What is the data transfer size in SPI? #card
			  id:: 64296f3d-2eb8-4373-a442-46170d018fd4
				- 4 to 16 bit serial packets.
			- What aspect of SPI controls data transfer order? #card
			  id:: 64296f3d-e275-404a-b754-e4a9b8089273
				- SPI Timing.
		- SPI Pros and Cons
			- SPI Pros
				- SPI Pros: Fully duplex
				- good signal integrity and high speed
				- Higher throughput than I2C. Not limited to any maximum clock speed, enabling potentially high speed
				- Flexibility on the bits transferred: arbitrary choice of message size, content, and purpose and not limited to 8-bit words.
				- Extremely simple hardware interfacing
				- Typically lower power requirements than I2C due to less circuitry (including pull up resistors)
				- Slaves use the master's clock and do not need precision oscillators.
				- Transceivers are not needed - unlike CAN-bus
				- Uses only four pins (or wires) much fewer than parallel interfaces.
				- Signals are unidirectional allowing for easy galvanic isolation
				- Simple software implementation
				- [[GPT Generated Flashcards]]
					- What is an advantage of SPI in terms of signal quality? #card
					  id:: 64296f3d-d44e-4439-af9b-173d87e6c597
						- Good signal integrity.
					- Which has a higher throughput, SPI or I2C? #card
					  id:: 64296f3d-a27e-4a5e-8fd9-d273206285db
						- SPI.
					- What allows SPI to have potentially high speed? #card
					  id:: 64296f3d-3b17-4e33-86c1-8f57bcd5cdc8
						- Not limited to any maximum clock speed.
					- What gives SPI flexibility in data transfer? #card
					  card-last-interval:: -1
					  card-repeats:: 1
					  card-ease-factor:: 2.5
					  card-next-schedule:: 2023-04-03T22:00:00.000Z
					  card-last-reviewed:: 2023-04-03T06:16:33.166Z
					  card-last-score:: 1
					  id:: 64296f3d-d9d1-4e4e-9bf4-e856bb99f0b1
						- Arbitrary choice of message size, content, and purpose.
					- What makes SPI's hardware interfacing simple? #card
					  id:: 64296f3d-77b1-4c23-8c54-1552157679ad
						- Extremely simple hardware interfacing.
					- Why might SPI have lower power requirements than I2C? #card
					  id:: 64296f3d-bf49-4490-919b-12f4a9d47a9c
						- Due to less circuitry (including pull up resistors).
					- How do SPI slaves maintain timing? #card
					  card-last-interval:: 4
					  card-repeats:: 1
					  card-ease-factor:: 2.6
					  card-next-schedule:: 2023-04-07T06:18:19.493Z
					  card-last-reviewed:: 2023-04-03T06:18:19.493Z
					  card-last-score:: 5
					  id:: 64296f3d-de6b-4d7b-bf62-ec66bed7f44e
						- They use the master's clock.
					- Are transceivers required for SPI communication? #card
					  id:: 64296f3d-c31e-4107-bd0a-5b926a06b52c
						- No.
					- How many pins (or wires) does SPI typically use? #card
					  card-last-interval:: 4
					  card-repeats:: 1
					  card-ease-factor:: 2.6
					  card-next-schedule:: 2023-04-07T06:04:20.628Z
					  card-last-reviewed:: 2023-04-03T06:04:20.628Z
					  card-last-score:: 5
					  id:: 64296f3d-dd28-4491-b1d8-b021b9272da2
						- Four.
					- Why is isolation easier with SPI signals? #card
					  id:: 64296f3d-bb9b-4bf0-b3e2-ed711c382dda
						- Signals are unidirectional.
					- Is SPI's software implementation complex or simple? #card
					  id:: 64296f3d-0135-444d-abc3-ccbe2f9d64f7
						- Simple.
			- SPI Cons
				- SPI Cons: Requires more pins on IC packages than I2C
				- No hardware slave acknowledgment
				- Typically supports only one master device
				- No error-checking protocol is defined
				- Only handles short distances compared to RS-232, RS-485, or CAN-bus
				- Many existing variations, making it difficult to find development tools
				- [[GPT Generated Flashcards]]
					- What are the disadvantages of SPI compared to I2C? #card
					  id:: 64296f3d-21f5-418e-a486-aedd0f7160ef
						- Requires more pins on IC packages.
					- Does SPI have hardware slave acknowledgment? #card
					  card-last-interval:: -1
					  card-repeats:: 1
					  card-ease-factor:: 2.5
					  card-next-schedule:: 2023-04-03T22:00:00.000Z
					  card-last-reviewed:: 2023-04-03T06:18:29.854Z
					  card-last-score:: 1
					  id:: 64296f3d-7f4f-4a26-8bbf-56cb8099082c
						- No.
					- How many master devices does SPI typically support? #card
					  id:: 64296f3d-92d2-4073-8a30-229d719004a8
						- One.
					- Does SPI have a defined error-checking protocol? #card
					  id:: 64296f3d-7445-4a17-8875-b8c4858d38b8
						- No.
					- Can SPI handle longer distances compared to RS-232, RS-485, or CAN-bus? #card
					  id:: 64296f3d-1534-45af-90a0-c95661e3fe7b
						- No, it only handles short distances.
					- Is it easy to find development tools for SPI due to its variations? #card
					  id:: 64296f3d-add9-43f9-a305-1708036d3ae6
						- No, it is difficult due to many existing variations.
	- I2C (Inter-Integrated Circuit)
		- I2C is a synchronous communication protocol => an explicit clock signal shared between sender and receiver.
		- In addition to a clock signal, called SCL, an I2C bus has a data signal called SDA.
		- The bus is considered idle when both SCL and SDA lines are high.
		- To initiate communication the bus master sends a start condition. which means driving SDA low while SCL is high.
		- When the bus master has completed its interaction with the slave device, the bus master asserts a STOP condition, pulling the SDA line high while the SCL line is high.
		- [[GPT Generated Flashcards]]
			- Which type of communication protocol is I2C (synchronous/asynchronous)? #card
			  card-last-interval:: 4
			  card-repeats:: 1
			  card-ease-factor:: 2.6
			  card-next-schedule:: 2023-04-07T06:07:38.521Z
			  card-last-reviewed:: 2023-04-03T06:07:38.521Z
			  card-last-score:: 5
			  id:: 64296f3d-7e7f-44ee-9c2a-0e050f7772eb
				- Synchronous.
			- What are the two signal lines in an I2C bus? #card
			  id:: 64296f3d-9ccd-43ce-bd6e-835d5e2c8621
				- SCL and SDA.
			- What causes the bus to be considered idle? #card
			  id:: 64296f3d-7ff1-4681-860f-519da112d634
				- Both SCL and SDA lines being high.
			- How does the bus master initiate communication? #card
			  id:: 64296f3d-38da-4cfa-99af-1e62264f4382
				- By sending a start condition (driving SDA low while SCL is high).
			- What does the bus master assert after completing interaction with the slave device? #card
			  id:: 64296f3d-5904-43fa-a00a-742aa1cc6c6e
				- A STOP condition (pulling the SDA line high while the SCL line is high).
		- I2C Pros and Cons
			- I2C Pros
				- I2C Pros: Flexibility The I2C protocol supports multimaster, multi-slave communication which can add functionalities to the embedded system.
				- Addressing feature It is easy to add components to the bus without any complexity.
				- Simplicity It requires only two bidirectional signal lines to establish communication among multiple devices and the pin count is low as well.
				- Error handling mechanism Error detection and correction relies on ACK/NACK feature (ACK stands for Acknowledgement whereas NACK means No Acknowledgement).
				- Adaptable The I2C protocol is adaptable in the sense that it can work well with both slow ICs and fast ICs.
				- [[GPT Generated Flashcards]]
					- What kind of communication does the I2C protocol support? #card
					  card-last-interval:: -1
					  card-repeats:: 1
					  card-ease-factor:: 2.5
					  card-next-schedule:: 2023-04-03T22:00:00.000Z
					  card-last-reviewed:: 2023-04-03T06:03:45.769Z
					  card-last-score:: 1
					  id:: 64296f3d-df6f-4317-97de-998b85e509f6
						- Multimaster, multi-slave communication.
					- What is the main advantage of the addressing feature in I2C? #card
					  card-last-interval:: -1
					  card-repeats:: 1
					  card-ease-factor:: 2.5
					  card-next-schedule:: 2023-04-03T22:00:00.000Z
					  card-last-reviewed:: 2023-04-03T06:05:39.978Z
					  card-last-score:: 1
					  id:: 64296f3d-89f0-4cf9-9147-9d44fd3a0d14
						- Easy to add components without complexity.
					- How many bidirectional signal lines are required in I2C? #card
					  id:: 64296f3d-8f8c-465c-9965-c721967c95eb
						- Two.
					- What does ACK/NACK stand for in the context of the I2C protocol? #card
					  id:: 64296f3d-ed4c-4506-9165-54afb2db759f
						- Acknowledgement/No Acknowledgement.
					- Can I2C work with both slow and fast ICs? #card
					  id:: 64296f3d-d432-49e0-91cc-3969a784d671
						- Yes.
			- I2C Cons
				- I2C Cons: Conflicts due to chip addressing.
				- Slower speeds I2C protocol uses pull-up resistors rather than the push-pull ones used by its peers. Due to the open-drain design, the speed is limited.
				- Requires more space The pullup resistors on which the protocol is based require quite some space.
				- [[GPT Generated Flashcards]]
					- What causes conflicts in I2C? #card
					  id:: 64296f3d-517f-40cf-b660-e45a4829996f
						- Chip addressing.
					- What type of resistors does I2C protocol use? #card
					  id:: 64296f3d-2f7c-45bf-9694-a60f54a47fda
						- Pull-up resistors.
					- What design limits the speed of I2C protocol? #card
					  id:: 64296f3d-67c8-4b24-ba6e-6354db4f6c8f
						- Open-drain design.
					- DONE Why does the I2C protocol require more space? #card
					  card-last-interval:: -1
					  card-repeats:: 1
					  card-ease-factor:: 2.5
					  card-next-schedule:: 2023-04-03T22:00:00.000Z
					  card-last-reviewed:: 2023-04-03T06:17:08.351Z
					  card-last-score:: 1
					  id:: 64296f3d-3c1b-41a3-9d77-7d237519996c
						- Pull-up resistors.
	- USB (Universal Serial Bus)
		- A USB system consists of a host with one or more downstream ports, and multiple peripherals.
		- USB device communication is based on **pipes** (logical channels).
		- A pipe is a connection from the host controller to a logical entity within a device, called an **endpoint**.
		- There are two types of pipe: **stream** and **message**.
			- A message pipe is bi-directional and is used for **control transfers**. Typically used for short, simple commands to the device, and for status responses from the device.
			- A stream pipe is a uni-directional pipe connected to a unidirectional endpoint that transfers data using:
				- **Isochronous transfer**: real-time data such as audio and video which require fixed bandwidth.
				- **Interrupt transfer**: used when data is sent regularly, for example for status updates.
				- **Bulk transfer**: used to send data where timing is not important, for example to a printer.
		- [[GPT Generated Flashcards]]
			- What are the two main components of a USB system? #card
			  card-last-interval:: -1
			  card-repeats:: 1
			  card-ease-factor:: 2.5
			  card-next-schedule:: 2023-04-03T22:00:00.000Z
			  card-last-reviewed:: 2023-04-03T06:12:30.658Z
			  card-last-score:: 1
			  id:: 64296f3d-3032-445e-a548-e92a6224a9bd
				- Host and peripherals.
			- What is the basis of USB device communication? #card
			  id:: 64296f3d-009b-45b4-9317-d4d5effd0dc5
				- Pipes.
			- What is a pipe in USB communication? #card
			  card-last-interval:: -1
			  card-repeats:: 1
			  card-ease-factor:: 2.5
			  card-next-schedule:: 2023-04-03T22:00:00.000Z
			  card-last-reviewed:: 2023-04-03T06:06:10.192Z
			  card-last-score:: 1
			  id:: 64296f3d-b128-4ebd-a16b-d3b7c9907e18
				- A connection from the host controller to an endpoint within a device.
			- What are the two types of pipes in USB communication? #card
			  id:: 64296f3d-1eda-4e33-82c8-767557133984
				- Stream and message.
			- What is the purpose of a message pipe? #card
			  id:: 64296f3d-8d8a-4d47-8283-f97f5d6a5c7d
				- Control transfers.
			- What is the purpose of a stream pipe? #card
			  id:: 64296f3d-63fe-49e9-8142-fa7f3023d0af
				- Transfer data using isochronous, interrupt, or bulk transfers.
			- What type of transfer is used for real-time data such as audio and video in a USB system? #card
			  id:: 64296f3d-bf11-4647-8823-c1d404164348
				- Isochronous transfer.
			- What type of transfer is used for regular data updates in a USB system? #card
			  id:: 64296f3d-b1cd-498f-9f70-054ecdaaf961
				- Interrupt transfer.
			- What type of transfer is used for data where timing is not important in a USB system? #card
			  id:: 64296f3d-cfdf-4b36-b8e2-d17e6b428c15
				- Bulk transfer.