- Real-time Operating System
	- Real-time Operating System Definition: A real-time operating system is an operating system that supports the construction of real-time systems
		- Soft and Hard real-time systems depending on how strict have to be the deadlines which must be met.
	- 3 key requirements:
		- 1) The timing behavior of the OS must be predictable. For each service of the OS, an upper bound on the execution time must be guaranteed.
		- 2) OS must manage the timing and scheduling. OS has to be aware of deadlines and should have a mechanism to take them into account in the scheduling. OS must provide precise time services with a high resolution
		- 3) OS must be fast: in addition to being predictable, the OS must be capable of supporting applications with deadlines that are fractions of a second.
	- Why do we need a RTOS? A desktop OS is not suited because:
		- 1) It is designed to serve general purpose use and therefore offers too many features which are not needed for embedded systems which have very specific scopes.
		- 2) These extra features/services take too much memory space and computation time.
		- 3) The timing uncertainty is too large for mission-critical applications.
	- [[GPT Generated Flashcards]]
		- What is a real-time operating system? #card
		  id:: 64296f3d-d8d6-4869-a39e-7f800a79132e
			- An operating system that supports the construction of real-time systems.
		- What are the two types of real-time systems? #card
		  id:: 64296f3d-43bd-4149-ad67-aafb12bf3ee2
			- Soft and Hard real-time systems.
		- What are the 3 key requirements of a real-time operating system? #card
		  card-last-interval:: -1
		  card-repeats:: 1
		  card-ease-factor:: 2.5
		  card-next-schedule:: 2023-04-03T22:00:00.000Z
		  card-last-reviewed:: 2023-04-03T06:16:53.390Z
		  card-last-score:: 1
		  id:: 64296f3d-9581-45a1-81d4-a0275be7f48c
			- Predictable timing behavior, timing and scheduling management, and fast performance.
		- Why must the execution time of a real-time operating system be guaranteed? #card
		  id:: 64296f3d-13f0-4850-95b2-cecb46640ac3
			- To ensure predictability and meet deadlines.
		- What is the role of an RTOS in scheduling and deadlines? #card
		  id:: 64296f3d-69c9-41a3-98a1-5afbf542364f
			- It must be aware of deadlines and incorporate them into its scheduling mechanism.
		- Why is a high-resolution time service necessary? #card
		  id:: 64296f3d-bacb-4ee7-9c82-765eca244f2a
			- To provide precise time services for real-time applications.
		- Why is a desktop OS not suitable for real-time applications? #card
		  card-last-interval:: 4
		  card-repeats:: 1
		  card-ease-factor:: 2.36
		  card-next-schedule:: 2023-04-07T06:16:42.938Z
		  card-last-reviewed:: 2023-04-03T06:16:42.938Z
		  card-last-score:: 3
		  id:: 64296f3d-04a8-41c2-ae69-18eced79113a
			- It has too many features, takes up memory and computation time, and has large timing uncertainty.
	- One of the key features of a RTOS for embedded systems is its **configurability**: it must be possible to remove not used components since unnecessary overhead is unacceptable.
	- Embedded OS
		- For embedded OS: Device drivers are typically handled directly by tasks instead of drivers that are managed by the operating system.
		- This architecture improves timing predictability as access to devices is also handled by the scheduler
		- If several tasks use the same external device and the associated driver, then the access must be carefully managed (shared critical resource, avoid race-condition)
	- Functions of a RTOS: the most important function of a RTOS is Task management:
		- Execution of quasi-parallel tasks on a processor using processes or threads (lightweight process) by maintaining process states, process queuing, allowing for preemptive tasks (fast context switching) and quick interrupt handling
		- CPU scheduling (guaranteeing deadlines, minimizing process waiting times, fairness in granting resources such as computing power)
		- Inter-task communication (buffering)
		- Support of real-time clocks
		- Task synchronization (critical sections, semaphores, monitors, mutual exclusion)
			- In classical operating systems, synchronization and mutual exclusion is performed via semaphores and monitors.
			- In real-time OS, special semaphores and a deep integration of them into scheduling is necessary (for example priority inheritance protocols).
	- Task States
		- A RTOS task usually has the following main states:
			- Running State: the task's code is currently being executed by the CPU.
			- Ready State: the task is ready to be put into the running state. In the ready state, the task does not consume any CPU cycles.
			- Blocked State: the task is in this state when it waits for the occurrence of some event. In this state, the task does not consume any cPU cycles.
	- [[GPT Generated Flashcards]]
		- What is the main function of a RTOS? #card
		  id:: 64296f3d-72dc-4eac-861d-b4ad12d06a07
			- Task management.
		- What are the core components of task management in a RTOS? #card
		  id:: 64296f3d-d207-477e-a6c3-1dcb8d9e1567
			- Execution of parallel tasks, CPU scheduling, inter-task communication, support of real-time clocks, and task synchronization.
		- In a RTOS, what is the purpose of preemptive tasks? #card
		  card-last-interval:: -1
		  card-repeats:: 1
		  card-ease-factor:: 2.5
		  card-next-schedule:: 2023-04-03T22:00:00.000Z
		  card-last-reviewed:: 2023-04-03T06:19:20.909Z
		  card-last-score:: 1
		  id:: 64296f3d-34aa-426f-8526-1c57c45a584c
			- Fast context switching and quick interrupt handling.
		- How does a RTOS ensure fairness in granting resources? #card
		  id:: 64296f3d-699d-4e15-9814-3f9484147b1e
			- Through CPU scheduling.
		- What is the purpose of inter-task communication in a RTOS? #card
		  id:: 64296f3d-4281-421c-a318-3c85ecabf6f9
			- Buffering.
		- What are the methods used for task synchronization in classical operating systems? #card
		  id:: 64296f3d-aa1d-4e74-99da-985b699fcf25
			- Semaphores and monitors.
		- In a real-time OS, what is necessary for synchronization and mutual exclusion? #card
		  id:: 64296f3d-56c9-4663-ab51-7b8828f9f0a5
			- Special semaphores and deep integration of them into scheduling.
		- What are the main states of a RTOS task? #card
		  id:: 64296f3d-4e3d-408a-979f-7d583afa3a85
			- Running State, Ready State, and Blocked State.
		- In which task state does a RTOS task consume CPU cycles? #card
		  card-last-interval:: -1
		  card-repeats:: 1
		  card-ease-factor:: 2.5
		  card-next-schedule:: 2023-04-03T22:00:00.000Z
		  card-last-reviewed:: 2023-04-03T06:18:14.964Z
		  card-last-score:: 1
		  id:: 64296f3d-032a-4567-b04f-9ea76de2d2b5
			- Running State.
	- Classes of RTOS
		- Class 1: Fast proprietary kernels
			- Examples: FreeRTOS, QNX, eCOS, RT-LINUX, VxWORKS, LynxOS.
			- For hard real-time systems, these kernels are tricky to use because they are designed to be fast, rather than to be predictable in every respect but they have been successfully used in many NASA missions including: Mars 2020, Mars Reconnaissance Orbiter, Curiosity, Sojourner, Spirit, Opportunity, Clementine, Phoenix Mars lander, Deep Impact space probe, Mars Pathfinder and Juno.
		- Class 2: Extensions to Standard OSs
			- Attempt to exploit existing and comfortable main stream operating systems.
			- A real-time kernel runs all real-time tasks.
			- The standard-OS is executed as one task
			- Example: RT-Linux runs the standard Linux kernel (or sub-kernel) as the lowest priority task in a simple real-time operating system.
		- Class 3: Research Systems
			- Research systems try to avoid limitations of existing real-time and embedded operating systems.
			- Examples include L4, seL4, NICTA, ERIKA, SHARK
			- Typical Research questions:
				- How to implement memory protection with low overhead.
				- How to use cache memories in RTOS
				- How to develop a RTOS for on-chip multiprocessors (i.e. hypervisors)
				- How to provide quality of service (QoS) control
		- Example: RTEMS (Real-Time Executive for Multiprocessor Systems)
	- [[GPT Generated Flashcards]]
		- What are the classes of RTOS? #card
		  id:: 64296f3d-2111-4198-a7d2-901a3abc406f
			- Class 1, Class 2, and Class 3.
		- What is the main characteristic of Class 1 RTOS? #card
		  id:: 64296f3d-8cc8-4a6e-a1d4-dd335d01842c
			- Fast proprietary kernels.
		- Can you name some examples of Class 1 RTOS? #card
		  id:: 64296f3d-9e01-4cc5-b6e1-6d06896249f8
			- FreeRTOS, QNX, eCOS, RT-LINUX, VxWORKS, LynxOS.
		- What type of systems find Class 1 RTOS difficult to use? #card
		  id:: 64296f3d-e9bf-431f-9884-360e49c7c8a1
			- Hard real-time systems.
		- What is the main feature of Class 2 RTOS? #card
		  id:: 64296f3d-830b-4fc0-88df-1125c9b189b1
			- Extensions to standard OSs.
		- How does a real-time kernel in Class 2 RTOS work? #card
		  id:: 64296f3d-7b9a-4291-a2ae-a78e796eec4b
			- It runs all real-time tasks.
		- What is an example of a Class 2 RTOS? #card
		  id:: 64296f3d-87a4-4fed-b54c-a3f12612369a
			- RT-Linux.
		- What is the aim of Class 3 RTOS? #card
		  id:: 64296f3d-d44e-4fbd-af34-ced22eef0458
			- To avoid limitations of existing real-time and embedded operating systems.
		- What is an example of a Class 3 RTOS? #card
		  id:: 64296f3d-f7f0-46d9-91dd-7e66d2e16a22
			- RTEMS (Real-Time Executive for Multiprocessor Systems).
	- The RTEMS is an open source Real Time Operating System (RTOS) that supports open standard API such as POSIX.
		- Chosen by ESA since it supports multiple microprocessors developed for use in space including SPARC, ERC32 and LEON, MIPS Mongoose-V, Coldfire, and PowerPC architectures, which are available in space hardened version.
		- Used in all ESA missions since 2006 and also many NASA (e.g. Mars Reconnaissance Orbiter, Dawn Orbiter, Fermi Gamma-ray Space Telescope, James Webb telescope)
		- Recently ported to support Xilinx Zynq UltraScale+ MPSoC.
	- Embedded Systems Architecture Synthesis
		- The scope of an architecture synthesis is to determine a hardware architecture that efficiently executes a given algorithm.
		- Major tasks of architecture synthesis are:
			- allocation (determine the necessary hardware resources)
			- scheduling (determine the timing of individual operations)
			- binding (determine relation between individual operations of the algorithm and hardware resources)
		- Classification of synthesis algorithms
			- heuristics or exact methods
		- Synthesis methods can often be applied independently of granularity of algorithms, e.g. whether operation is a whole complex task or a single operation.
	- Which language to use to specify embedded systems?
		- Requirements are often written in a natural language however this is not the best way to assure completeness and consistency of specifications.
		- We need a specification language, a formal-machine readable language which describes the system at a higher level than a programming language.
		- Specification languages are not directly executed, they describe the what and not the how.
	- [[GPT Generated Flashcards]]
		- What is the purpose of architecture synthesis? #card
		  id:: 64296f3d-8d87-499a-abdf-5d21775614da
			- To determine a hardware architecture that efficiently executes a given algorithm.
		- What are the major tasks of architecture synthesis? #card
		  id:: 64296f3d-7a7b-4acc-a25f-e5e9e8dedb7e
			- Allocation, scheduling, and binding.
		- What are the two classifications of synthesis algorithms? #card
		  id:: 64296f3d-05e3-4de4-a25f-a654fcafaeb2
			- Heuristics and exact methods.
		- Can synthesis methods be applied independently of granularity? #card
		  card-last-interval:: -1
		  card-repeats:: 1
		  card-ease-factor:: 2.5
		  card-next-schedule:: 2023-04-03T22:00:00.000Z
		  card-last-reviewed:: 2023-04-03T06:11:47.038Z
		  card-last-score:: 1
		  id:: 64296f3d-7db3-436d-b68b-df3a891aaa32
			- Yes.
		- Why are natural languages not the best for specifying embedded systems? #card
		  id:: 64296f3d-f4c5-4de7-80bf-d958130c3101
			- They don't assure completeness and consistency of specifications.
		- What is a specification language? #card
		  id:: 64296f3d-09a7-435d-a1b4-4495510bbe45
			- A formal-machine readable language describing the system at a higher level than a programming language.
		- Do specification languages describe the 'what' or the 'how'? #card
		  id:: 64296f3d-fcbe-4510-9dd0-9bd0d1a37d20
			- The 'what'.
	- Embedded System Features
		- Hierarchy: Behavioral hierarchies (system described by states/events) & Structural hierarchies (system described by physical components)
		- Timing behavior.
		- State oriented behavior (easy to implement but needs to be complemented by timing and hierarchy)
		- Event handling: the reactive nature of embedded systems requires the capability to recognize events which might be external or internal.
		- Exception oriented behavior / Exception handling.
		- Component based design: it should be possible to derive the behavior of a system from the behavior of its components
		- Concurrency: embedded systems are typically composed by distributed and concurrent components.
		- Synchronization and communication: management of common resources.
		- Usability of programming languages.
		- Portability and flexibility: requirements should be as independent as possible from specific hardware platform
		- Support for the design of dependable systems.
		- Appropriate model of computation.
		- [[GPT Generated Flashcards]]
			- What are the two types of hierarchies in a system? #card
			  id:: 64296f3d-27fc-4c39-9d7e-3a68dbf6ebaf
				- Behavioral hierarchies and Structural hierarchies.
			- What type of behavior is easy to implement but needs to be complemented by timing and hierarchy? #card
			  id:: 64296f3d-1e00-481d-8351-10dcea63628d
				- State oriented behavior.
			- What is the term for recognizing events that might be external or internal in embedded systems? #card
			  id:: 64296f3d-7c75-4cf8-9281-53bc468ea94f
				- Event handling.
			- What type of behavior deals with exceptions in a system? #card
			  id:: 64296f3d-97f3-4b4f-84ca-82be2bc3967c
				- Exception oriented behavior.
			- What is the design approach that allows deriving the behavior of a system from its components? #card
			  id:: 64296f3d-ad8c-4307-8893-5dc0062be51d
				- Component based design.
			- What is the term used for embedded systems with distributed and concurrent components? #card
			  id:: 64296f3d-3100-4ff3-bfce-62714ffa87cd
				- Concurrency.
			- What are the two main aspects of managing common resources in embedded systems? #card
			  card-last-interval:: -1
			  card-repeats:: 1
			  card-ease-factor:: 2.5
			  card-next-schedule:: 2023-04-03T22:00:00.000Z
			  card-last-reviewed:: 2023-04-03T06:07:21.385Z
			  card-last-score:: 1
			  id:: 64296f3d-d8cb-4fac-8052-9dae778a68ad
				- Synchronization and communication.
			- What factor of programming languages is important for embedded systems development? #card
			  id:: 64296f3d-3d48-491a-aade-fa25aac4a3b0
				- Usability.
			- What two qualities are important in making requirements independent of a specific hardware platform? #card
			  id:: 64296f3d-cd8a-4f8e-adad-2824b3aa6367
				- Portability and flexibility.
			- In embedded systems, which feature supports the design of dependable systems? #card
			  id:: 64296f3d-9eb1-4af8-a516-9ec64c2ceacf
				- Support for the design of dependable systems.
			- Which aspect of embedded systems involves an appropriate model of computation? #card
			  id:: 64296f3d-74ee-48c6-bbef-0a02bb82e7c8
				- Appropriate model of computation.
	- Models of Computation
		- The Von Neumann architecture does not describe fully an embedded system!
		- Models of Computation (MoC) describe the mechanism used to perform computations. It defines how a set of inputs is computed to obtain a certain set of output.
		- Models of computation define:
			- a) Components: organization of computation in different components (Procedures, processes, functions, finite state machine.
			- b) Communication protocols: methods for communication between components.
		- Relations between components can be captured in graphs where computations are represented as processes or tasks.
		  An obvious type of relation between computations is their casual dependence (for example a computation can be only executed after an another computation has been completed).
		- These dependencies are captured in dependence graphs.
			- These simple graphs should evolve in task graph which include also:
				- Timing information
				- input/output
				- Access to resources
				- Periodic scheduling
				- Hierarchical nodes
		- [[GPT Generated Flashcards]]
			- What do Models of Computation (MoC) describe? #card
			  id:: 64296f3d-495c-415c-9f39-dabb3e61d1e1
				- The mechanism used to perform computations.
			- What are the two main aspects defined by Models of Computation? #card
			  card-last-interval:: -1
			  card-repeats:: 1
			  card-ease-factor:: 2.5
			  card-next-schedule:: 2023-04-03T22:00:00.000Z
			  card-last-reviewed:: 2023-04-03T06:18:44.650Z
			  card-last-score:: 1
			  id:: 64296f3d-9ec1-4a37-b7ee-b921c93aedff
				- Components and communication protocols.
			- What are some examples of components in Models of Computation? #card
			  id:: 64296f3d-3b12-4671-ba4f-812feb5d796d
				- Procedures, processes, functions, finite state machines.
			- How can relations between components be represented? #card
			  card-last-interval:: -1
			  card-repeats:: 1
			  card-ease-factor:: 2.5
			  card-next-schedule:: 2023-04-03T22:00:00.000Z
			  card-last-reviewed:: 2023-04-03T06:14:14.015Z
			  card-last-score:: 1
			  id:: 64296f3d-e139-4460-9fec-3d9d3b1e4a18
				- In graphs as processes or tasks.
			- What type of relation between computations is casual dependence? #card
			  id:: 64296f3d-4b33-401c-b394-eb7d694e9944
				- When a computation can only be executed after another computation is completed.
			- What are the graphs called that capture dependencies between computations? #card
			  card-last-interval:: 4
			  card-repeats:: 1
			  card-ease-factor:: 2.6
			  card-next-schedule:: 2023-04-07T06:10:07.399Z
			  card-last-reviewed:: 2023-04-03T06:10:07.399Z
			  card-last-score:: 5
			  id:: 64296f3d-daa6-4854-8f28-55528e5507d9
				- Dependence graphs.
	- Organization of computations
		- Communicating Finite State Machines (CFSMs): based on a finite set of state machines communicating with each other (i/o and transitions between states).
		- Discrete event model: event carry a time stamp and are processed from a event queue sorted by time.
		- Differential equations/polynomials: used for modeling analog circuits and physical systems.
		- Asynchronous message passing: processes communicate by sending messages which can be buffered. The sender does not need to wait for the receiver to be ready. There different implementations for example Dataflow program where the availability of data triggers the possible execution of operations \(\rightarrow\) risk of overflows.
		- Synchronous message passing: processes communicate in a instantaneous actions called rendez-vous. The process which reaches first the point of communication has to wait for the second to complete.
		- Designs starting from non-Von-Neumann models are also called model-based designs where the key idea is to have some abstract mode of the system under design.
	- [[GPT Generated Flashcards]]
		- What is the basis of Communicating Finite State Machines? #card
		  id:: 64296f3d-d26d-496d-82cf-4f2f823adf5a
			- A finite set of state machines communicating with each other.
		- What is an important feature of the Discrete event model? #card
		  id:: 64296f3d-e791-434a-9029-15710d9fdebe
			- Events carry a time stamp and are processed from an event queue sorted by time.
		- What are differential equations and polynomials commonly used for in the context of Embedded systems? #card
		  id:: 64296f3d-11d4-4fee-b56e-4ec541fe334f
			- Modeling analog circuits and physical systems.
		- In Asynchronous message passing, does the sender need to wait for the receiver to be ready? #card
		  card-last-interval:: -1
		  card-repeats:: 1
		  card-ease-factor:: 2.5
		  card-next-schedule:: 2023-04-03T22:00:00.000Z
		  card-last-reviewed:: 2023-04-03T06:05:01.041Z
		  card-last-score:: 1
		  id:: 64296f3d-c50a-4176-ae3a-723ad2e4ae09
			- No.
		- What triggers the execution of operations in a Dataflow program? #card
		  id:: 64296f3d-20f3-4936-82fb-c446b601f29c
			- The availability of data.
		- What occurs during a rendez-vous in Synchronous message passing? #card
		  card-last-interval:: -1
		  card-repeats:: 1
		  card-ease-factor:: 2.5
		  card-next-schedule:: 2023-04-03T22:00:00.000Z
		  card-last-reviewed:: 2023-04-03T06:12:25.503Z
		  card-last-score:: 1
		  id:: 64296f3d-ee71-4c00-a298-d3705c111b1d
			- Two processes communicate in instantaneous actions.
		- DONE What is the key idea in model-based designs? #card
		  card-last-interval:: -1
		  card-repeats:: 1
		  card-ease-factor:: 2.5
		  card-next-schedule:: 2023-04-03T22:00:00.000Z
		  card-last-reviewed:: 2023-04-03T06:13:50.171Z
		  card-last-score:: 1
		  id:: 64296f3d-d993-4c45-9a19-d8f921ae8cec
			- To have an abstract model of the system under design.
	- Model of communication
		- Shared memory: communication is performed by accessing the same memory from all components. In shared memory if write operations are involved, mechanisms for exclusive access must be provided (e.g semaphores, monitors, spin-locks etc.).
			- Message passing: messages are sent and received by the different components. Generally slower than shared memory.
				- Asynchronous message passing or non-blocking
				- Synchronous message passing or blocking communication
			- Extended rendez-vous, remote invocation: the sender is allowed to continue only after receiving an acknowledgment from the recipient.
	- [[GPT Generated Flashcards]]
		- What type of communication involves accessing the same memory from all components? #card
		  id:: 64296f3d-b4c1-4891-b903-6173a79ecec6
			- Shared memory.
		- What mechanism ensures exclusive access in shared memory communication? #card
		  id:: 64296f3d-bf7e-4763-a667-93a1aa086575
			- Semaphores, monitors, or spin-locks.
		- What type of communication in embedded systems involves sending and receiving messages between components? #card
		  id:: 64296f3d-00ca-42d3-8fb3-64c5d69a2e86
			- Message passing.
		- Which communication method is generally slower: shared memory or message passing? #card
		  id:: 64296f3d-70e4-4718-bbeb-4109316eb3d0
			- Message passing.
		- What is the difference between asynchronous and synchronous message passing? #card
		  id:: 64296f3d-c42a-4d5b-8424-66867dc1691d
			- Asynchronous is non-blocking, while synchronous is blocking communication.
		- In extended rendez-vous or remote invocation, when can the sender continue? #card
		  id:: 64296f3d-7692-48b7-a960-a31d6622d26a
			- After receiving an acknowledgment from the recipient.