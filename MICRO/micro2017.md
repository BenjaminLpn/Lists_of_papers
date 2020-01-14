### micro 2017 | 61 papers.
---
### Banshee: bandwidth-efficient DRAM caching via software/hardware cooperation.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124555
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124555?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, Parallel architectures, Multicore architectures, 
* **Abstract**: Placing the DRAM in the same package as a processor enables several times higher memory bandwidth than conventional off-package DRAM. Yet, the latency of in-package DRAM is not appreciably lower than that of off-package DRAM. A promising use of in-package DRAM is as a large cache. Unfortunately, most previous DRAM cache designs optimize mainly for cache hit latency and do not consider bandwidth efficiency as a first-class design constraint. Hence, as we show in this paper, these designs are suboptimal for use with in-package DRAM.

---
### Contutto: a novel FPGA-based prototyping platform enabling innovation in the memory subsystem of a server class processor.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124535
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124535?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Reconfigurable computing, Hardware, Emerging technologies, Analysis and design of emerging devices and systems, 
* **Abstract**: We demonstrate the use of an FPGA as a memory buffer in a POWER8® system, creating a novel prototyping platform that enables innovation in the memory subsystem of POWER-based servers. Our platform, called ConTutto, is pin-compatible with POWER8 buffered memory DIMMs and plugs into a memory slot of a standard POWER8 processor system, running at aggregate memory channel speeds of 35 GB/s per link. ConTutto, which means "with everything", is a platform to experiment with different memory technologies, such as STT-MRAM and NAND Flash, in an end-to-end system context. Enablement of STT-MRAM and NVDIMM using ConTutto shows up to 12.5x lower latency and 7.5x higher bandwidth compared to the respective technologies when attached to the PCIe bus. Moreover, due to the unique attach-point of the FPGA between the processor and system memory, ConTutto provides a means for in-line acceleration of certain computations on-route to memory, and enables sensitivity analysis for memory latency while running real applications. To the best of our knowledge, ConTutto is the first ever FPGA platform on the memory bus of a server class processor.

---
### Detecting and mitigating data-dependent DRAM failures by exploiting current memory content.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123945
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123945?download=true
* **Key Words**: Computer systems organization, Dependable and fault-tolerant systems and networks, Processors and memory architectures, Hardware, Integrated circuits, Semiconductor memory, Dynamic memory, 
* **Abstract**: DRAM cells in close proximity can fail depending on the data content in neighboring cells. These failures are called data-dependent failures. Detecting and mitigating these failures online, while the system is running in the field, enables various optimizations that improve reliability, latency, and energy efficiency of the system. For example, a system can improve performance and energy efficiency by using a lower refresh rate for most cells and mitigate the failing cells using higher refresh rates or error correcting codes. All these system optimizations depend on accurately detecting every possible data-dependent failure that could occur with any content in DRAM. Unfortunately, detecting all data-dependent failures requires the knowledge of DRAM internals specific to each DRAM chip. As internal DRAM architecture is not exposed to the system, detecting data-dependent failures at the system-level is a major challenge.

---
### Fine-grained DRAM: energy-efficient DRAM for extreme bandwidth systems.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124545
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124545?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Computing methodologies, Computer graphics, Graphics systems and interfaces, Graphics processors, Hardware, Integrated circuits, Semiconductor memory, Dynamic memory, Power and energy, 
* **Abstract**: Future GPUs and other high-performance throughput processors will require multiple TB/s of bandwidth to DRAM. Satisfying this bandwidth demand within an acceptable energy budget is a challenge in these extreme bandwidth memory systems. We propose a new high-bandwidth DRAM architecture, Fine-Grained DRAM (FGDRAM), which improves bandwidth by 4× and improves the energy efficiency of DRAM by 2× relative to the highest-bandwidth, most energy-efficient contemporary DRAM, High Bandwidth Memory (HBM2). These benefits are in large measure achieved by partitioning the DRAM die into many independent units, called grains, each of which has a local, adjacent I/O. This approach unlocks the bandwidth of all the banks in the DRAM to be used simultaneously, eliminating shared buses interconnecting various banks. Furthermore, the on-DRAM data movement energy is significantly reduced due to the much shorter wiring distance between the cell array and the local I/O. This FGDRAM architecture readily lends itself to leveraging existing techniques to reducing the effective DRAM row size in an area efficient manner, reducing wasteful row activate energy in applications with low locality. In addition, when FGDRAM is paired with a memory controller optimized to exploit the additional concurrency provided by the independent grains, it improves GPU system performance by 19% over an iso-bandwidth and iso-capacity future HBM baseline. Thus, this energy-efficient, high-bandwidth FGDRAM architecture addresses the needs of future extreme-bandwidth memory systems.

---
### UDP: a programmable accelerator for extract-transform-load workloads and more.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123983
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123983?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Hardware, Very large scale integration design, Application-specific VLSI designs, Application specific processors, Information systems, Data management systems, Information integration, Extraction, transformation and loading, Theory of computation, Design and analysis of algorithms, Data structures design and analysis, Pattern matching, 
* **Abstract**: Big data analytic applications give rise to large-scale extract-transform-load (ETL) as a fundamental step to transform new data into a native representation. ETL workloads pose significant performance challenges on conventional architectures, so we propose the design of the unstructured data processor (UDP), a software programmable accelerator that includes multi-way dispatch, variable-size symbol support, Flexible-source dispatch (stream buffer and scalar registers), and memory addressing to accelerate ETL kernels both for current and novel future encoding and compression. Specifically, UDP excels at branch-intensive and symbol and pattern-oriented workloads, and can offload them from CPUs.

---
### UNFOLD: a memory-efficient speech recognizer using on-the-fly WFST composition.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124542
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124542?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Special purpose systems, Computing methodologies, Artificial intelligence, Natural language processing, Speech recognition, 
* **Abstract**: Accurate, real-time Automatic Speech Recognition (ASR) requires huge memory storage and computational power. The main bottleneck in state-of-the-art ASR systems is the Viterbi search on a Weighted Finite State Transducer (WFST). The WFST is a graph-based model created by composing an Acoustic Model (AM) and a Language Model (LM) offline. Offline composition simplifies the implementation of a speech recognizer as only one WFST has to be searched. However, the size of the composed WFST is huge, typically larger than a Gigabyte, resulting in a large memory footprint and memory bandwidth requirements.

---
### IDEAL: image denoising accelerator.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123941
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123941?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Neural networks, Special purpose systems, Parallel architectures, Single instruction, multiple data, Real-time systems, Real-time system architecture, 
* **Abstract**: Computational imaging pipelines (CIPs) convert the raw output of imaging sensors into the high-quality images that are used for further processing. This work studies how Block-Matching and 3D filtering (BM3D), a state-of-the-art denoising algorithm can be implemented to meet the demands of user-interactive (UI) applications. Denoising is the most computationally demanding stage of a CIP taking more than 95% of time on a highly-optimized software implementation [29]. We analyze the performance and energy consumption of optimized software implementations on three commodity platforms and find that their performance is inadequate.

---
### Pipelining a triggered processing element.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124551
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124551?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Interconnection architectures, Multicore architectures, Multiple instruction, multiple data, Serial architectures, Pipeline computing, Reduced instruction set computing, Hardware, Power and energy, 
* **Abstract**: Programmable spatial architectures composed of ensembles of autonomous fixed-ISA processing elements offer a compelling design point between the flexibility of an FPGA and the compute density of a GPU or shared-memory many-core. The design regularity of spatial architectures demands examination of the processing element microarchitecture early in the design process to optimize overall efficiency.

---
### Efficient exception handling support for GPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123950
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123950?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Memory management, Virtual memory, 
* **Abstract**: Operating systems have long relied on the exception handling mechanism to implement numerous virtual memory features and optimizations. However, today's GPUs have a limited support for exceptions, which prevents implementation of such techniques. The existing solution forwards GPU memory faults to the CPU while the faulting instruction is stalled in the GPU pipeline. This approach prevents preemption of the faulting threads, and results in underutilized hardware resources while the page fault is being resolved by the CPU.

---
### Beyond the socket: NUMA-aware GPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124534
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124534?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Single instruction, multiple data, Computing methodologies, Computer graphics, Graphics systems and interfaces, Graphics processors, 
* **Abstract**: GPUs achieve high throughput and power efficiency by employing many small single instruction multiple thread (SIMT) cores. To minimize scheduling logic and performance variance they utilize a uniform memory system and leverage strong data parallelism exposed via the programming model. With Moore's law slowing, for GPUs to continue scaling performance (which largely depends on SIMT core count) they are likely to embrace multi-socket designs where transistors are more readily available. However when moving to such designs, maintaining the illusion of a uniform memory system is increasingly difficult. In this work we investigate multi-socket non-uniform memory access (NUMA) GPU designs and show that significant changes are needed to both the GPU interconnect and cache architectures to achieve performance scalability. We show that application phase effects can be exploited allowing GPU sockets to dynamically optimize their individual interconnect and cache policies, minimizing the impact of NUMA effects. Our NUMA-aware GPU outperforms a single GPU by 1.5×, 2.3×, and 3.2× while achieving 89%, 84%, and 76% of theoretical application scalability in 2, 4, and 8 sockets designs respectively. Implementable today, NUMA-aware multi-socket GPUs may be a promising candidate for scaling GPU performance beyond a single socket.

---
### Mosaic: a GPU memory manager with application-transparent support for multiple page sizes.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123975
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123975?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, 
* **Abstract**: Contemporary discrete GPUs support rich memory management features such as virtual memory and demand paging. These features simplify GPU programming by providing a virtual address space abstraction similar to CPUs and eliminating manual memory management, but they introduce high performance overheads during (1) address translation and (2) page faults. A GPU relies on high degrees of thread-level parallelism (TLP) to hide memory latency. Address translation can undermine TLP, as a single miss in the translation lookaside buffer (TLB) invokes an expensive serialized page table walk that often stalls multiple threads. Demand paging can also undermine TLP, as multiple threads often stall while they wait for an expensive data transfer over the system I/O (e.g., PCIe) bus when the GPU demands a page.

---
### Regless: just-in-time operand staging for GPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123974
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123974?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Single instruction, multiple data, Software and its engineering, Software notations and tools, Compilers, 
* **Abstract**: The register file is one of the largest and most power-hungry structures in a Graphics Processing Unit (GPU), because massive multithreading requires all the register state for every active thread to be available. Previous approaches to making register accesses more efficient have optimized how registers are stored, but they must keep all values for active threads in a large, high-bandwidth structure. If operand storage is to be reduced further, there will not be enough capacity for every live value to be stored at the same time. Our insight is that computation graphs can be sliced into regions and operand storage can be allocated to these regions as they are encountered at run time, allowing a small operand staging unit to replace the register file. Most operand values have a short lifetime that is contained in one region, so their value does not need to persist in the staging unit past the end of that region. The small number of longer-lived operands can be stored in lower-bandwidth global memory, but the hardware must anticipate their use to fetch them early enough to avoid stalls. In RegLess, hardware uses compiler annotations to anticipate warps' operand usage at run time, allowing the register file to be replaced with an operand staging unit 25% of the size, saving 75% of register file energy and 11% of total GPU energy with no average performance loss.

---
### SCRATCH: an end-to-end application-aware soft-GPGPU architecture and trimming tool.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123953
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123953?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Computing methodologies, Machine learning, Hardware, Electronic design automation, High-level and register-transfer level synthesis, Hardware-software codesign, 
* **Abstract**: Applying advanced signal processing and artificial intelligence algorithms is often constrained by power and energy consumption limitations, in high performance and embedded, cyber-physical and super-computing devices and systems. Although Graphics Processing Units (GPUs) helped to mitigate the throughput-per-Watt performance problem in many compute-intensive applications, dealing more efficiently with the autonomy requirements of intelligent systems demands power-oriented customized architectures that are specially tuned for each application, preferably without manual redesign of the entire hardware and capable of supporting legacy code. Hence, this work proposes a new SCRATCH framework that aims at automatically identifying the specific requirements of each application kernel, regarding instruction set and computing unit demands, allowing for the generation of application-specific and FPGA-implementable trimmed-down GPU-inspired architectures. The work is based on an improved version of the original MIAOW system (here named MIAOW2.0), which is herein extended to support a set of 156 instructions and enhanced to provide a fast prefetch memory system and a dual-clock domain. Experimental results with 17 highly relevant benchmarks, using integer and floating-point arithmetic, demonstrate that we have been able to achieve an average of 140× speedup and 115× higher energy-efficiency levels (instructions-per-Joule) when compared to the original MIAOW system, and a 2.4× speedup and 2.1× energy-efficiency gains compared against our optimized version without pruning.

---
### Proteus: a flexible and fast software supported hardware logging approach for NVM.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124539
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124539?download=true
* **Key Words**: Computer systems organization, Architectures, Serial architectures, Hardware, Emerging technologies, Memory and dense storage, 
* **Abstract**: Emerging non-volatile memory (NVM) technologies, such as phase-change memory, spin-transfer torque magnetic memory, memristor, and 3D Xpoint, are encouraging the development of new architectures that support the challenges of persistent programming. An important remaining challenge is dealing with the high logging overheads introduced by durable transactions.

---
### Efficient support of position independence on non-volatile memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124543
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124543?download=true
* **Key Words**: Computer systems organization, Architectures, Hardware, Emerging technologies, Memory and dense storage, Software and its engineering, Software notations and tools, Compilers, General programming languages, 
* **Abstract**: This paper explores solutions for enabling efficient supports of position independence of pointer-based data structures on byte-addressable None-Volatile Memory (NVM). When a dynamic data structure (e.g., a linked list) gets loaded from persistent storage into main memory in different executions, the locations of the elements contained in the data structure could differ in the address spaces from one run to another. As a result, some special support must be provided to ensure that the pointers contained in the data structures always point to the correct locations, which is called position independence.

---
### Incidental computing on IoT nonvolatile processors.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124533
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124533?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Special purpose systems, Parallel architectures, Single instruction, multiple data, Embedded and cyber-physical systems, Embedded systems, Embedded hardware, System on a chip, 
* **Abstract**: Batteryless IoT devices powered through energy harvesting face a fundamental imbalance between the potential volume of collected data and the amount of energy available for processing that data locally. However, many such devices perform similar operations across each new input record, which provides opportunities for mining the potential information in buffered historical data, at potentially lower effort, while processing new data rather than abandoning old inputs due to limited computational energy. We call this approach incidental computing, and highlight synergies between this approach and approximation techniques when deployed on a non-volatile processor platform (NVP). In addition to incidental computations, the backup and restore operations in an incidental NVP provide approximation opportunities and optimizations that are unique to NVPs.

---
### Summarizer: trading communication with computing near storage.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124553
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124553?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Dependable and fault-tolerant systems and networks, Secondary storage organization, Embedded and cyber-physical systems, Embedded systems, Firmware, 
* **Abstract**: Modern data center solid state drives (SSDs) integrate multiple general-purpose embedded cores to manage flash translation layer, garbage collection, wear-leveling, and etc., to improve the performance and the reliability of SSDs. As the performance of these cores steadily improves there are opportunities to repurpose these cores to perform application driven computations on stored data, with the aim of reducing the communication between the host processor and the SSD. Reducing host-SSD bandwidth demand cuts down the I/O time which is a bottleneck for many applications operating on large data sets. However, the embedded core performance is still significantly lower than the host processor, as generally wimpy embedded cores are used within SSD for cost effective reasons. So there is a trade-off between the computation overhead associated with near SSD processing and the reduction in communication overhead to the host system.

---
### Memory cocktail therapy: a general learning-based framework to optimize dynamic tradeoffs in NVMs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124548
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124548?download=true
* **Key Words**: Hardware, Emerging technologies, Memory and dense storage, 
* **Abstract**: Non-volatile memories (NVMs) have attracted significant interest recently due to their high-density, low static power, and persistence. There are, however, several challenges associated with building practical systems from NVMs, including limited write endurance and long latencies. Researchers have proposed a variety of architectural techniques which can achieve different tradeoffs between lifetime, performance and energy efficiency; however, no individual technique can satisfy requirements for all applications and different objectives. Hence, we propose Memory Cocktail Therapy (MCT), a general, learning-based framework that adaptively chooses the best techniques for the current application and objectives.

---
### A many-core architecture for in-memory data processing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123985
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123985?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Special purpose systems, Parallel architectures, Multicore architectures, 
* **Abstract**: For many years, the highest energy cost in processing has been data movement rather than computation, and energy is the limiting factor in processor design [21]. As the data needed for a single application grows to exabytes [56], there is clearly an opportunity to design a bandwidth-optimized architecture for big data computation by specializing hardware for data movement. We present the Data Processing Unit or DPU, a shared memory many-core that is specifically designed for high bandwidth analytics workloads. The DPU contains a unique Data Movement System (DMS), which provides hardware acceleration for data movement and partitioning operations at the memory controller that is sufficient to keep up with DDR bandwidth. The DPU also provides acceleration for core to core communication via a unique hardware RPC mechanism called the Atomic Transaction Engine. Comparison of a DPU chip fabricated in 40nm with a Xeon processor on a variety of data processing applications shows a 3× - 15× performance per watt advantage.

---
### Cache automaton.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123986
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123986?download=true
* **Key Words**: Hardware, Emerging technologies, Analysis and design of emerging devices and systems, Emerging architectures, Theory of computation, Formal languages and automata theory, 
* **Abstract**: Finite State Automata are widely used to accelerate pattern matching in many emerging application domains like DNA sequencing and XML parsing. Conventional CPUs and compute-centric accelerators are bottlenecked by memory bandwidth and irregular memory access patterns in automata processing.

---
### Ambit: in-memory accelerator for bulk bitwise operations using commodity DRAM technology.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124544
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124544?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Single instruction, multiple data, Hardware, Integrated circuits, Reconfigurable logic and FPGAs, Hardware accelerators, Semiconductor memory, Dynamic memory, 
* **Abstract**: Many important applications trigger bulk bitwise operations, i.e., bitwise operations on large bit vectors. In fact, recent works design techniques that exploit fast bulk bitwise operations to accelerate databases (bitmap indices, BitWeaving) and web search (BitFunnel). Unfortunately, in existing architectures, the throughput of bulk bitwise operations is limited by the memory bandwidth available to the processing unit (e.g., CPU, GPU, FPGA, processing-in-memory).

---
### DRISA: a DRAM-based reconfigurable in-situ accelerator.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123977
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123977?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Neural networks, Reconfigurable computing, Hardware, Integrated circuits, Semiconductor memory, Dynamic memory, 
* **Abstract**: Data movement between the processing units and the memory in traditional von Neumann architecture is creating the "memory wall" problem. To bridge the gap, two approaches, the memory-rich processor (more on-chip memory) and the compute-capable memory (processing-in-memory) have been studied. However, the first one has strong computing capability but limited memory capacity/bandwidth, whereas the second one is the exact the opposite.

---
### Pageforge: a near-memory content-aware page-merging architecture.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124540
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124540?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Cloud computing, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Memory management, Software infrastructure, Virtual machines, 
* **Abstract**: To reduce the memory requirements of virtualized environments, modern hypervisors are equipped with the capability to search the memory address space and merge identical pages --- a process called page deduplication. This process uses a combination of data hashing and exhaustive comparison of pages, which consumes processor cycles and pollutes caches.

---
### RHMD: evasion-resilient hardware malware detectors.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123972
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123972?download=true
* **Key Words**: Security and privacy, Intrusion/anomaly detection and malware mitigation, Malware and its mitigation, Security in hardware, Hardware security implementation, 
* **Abstract**: Hardware Malware Detectors (HMDs) have recently been proposed as a defense against the proliferation of malware. These detectors use low-level features, that can be collected by the hardware performance monitoring units on modern CPUs to detect malware as a computational anomaly. Several aspects of the detector construction have been explored, leading to detectors with high accuracy. In this paper, we explore the question of how well evasive malware can avoid detection by HMDs. We show that existing HMDs can be effectively reverse-engineered and subsequently evaded, allowing malware to hide from detection without substantially slowing it down (which is important for certain types of malware). This result demonstrates that the current generation of HMDs can be easily defeated by evasive malware. Next, we explore how well a detector can evolve if it is exposed to this evasive malware during training. We show that simple detectors, such as logistic regression, cannot detect the evasive malware even with retraining. More sophisticated detectors can be retrained to detect evasive malware, but the retrained detectors can be reverse-engineered and evaded again. To address these limitations, we propose a new type of Resilient HMDs (RHMDs) that stochastically switch between different detectors. These detectors can be shown to be provably more difficult to reverse engineer based on resent results in probably approximately correct (PAC) learnability theory. We show that indeed such detectors are resilient to both reverse engineering and evasion, and that the resilience increases with the number and diversity of the individual detectors. Our results demonstrate that these HMDs offer effective defense against evasive malware at low additional complexity.

---
### Software-based gate-level information flow security for IoT systems.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123955
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123955?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Special purpose systems, Embedded and cyber-physical systems, Embedded systems, 
* **Abstract**: The growing movement to connect literally everything to the internet (internet of things or IoT) through ultra-low-power embedded microprocessors poses a critical challenge for information security. Gate-level tracking of information flows has been proposed to guarantee information flow security in computer systems. However, such solutions rely on non-commodity, secure-by-design processors. In this work, we observe that the need for secure-by-design processors arises because previous works on gate-level information flow tracking assume no knowledge of the application running in a system. Since IoT systems typically run a single application over and over for the lifetime of the system, we see a unique opportunity to provide application-specific gate-level information flow security for IoT systems. We develop a gate-level symbolic analysis framework that uses knowledge of the application running in a system to efficiently identify all possible information flow security vulnerabilities for the system. We leverage this information to provide security guarantees on commodity processors. We also show that security vulnerabilities identified by our analysis framework can be eliminated through software modifications at 15% energy overhead, on average, obviating the need for secure-by-design hardware. Our framework also allows us to identify and eliminate only the vulnerabilities that an application is prone to, reducing the cost of information flow security by 3.3× compared to a software-based approach that assumes no application knowledge.

---
### How secure is your cache against side-channel attacks?
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124546
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124546?download=true
* **Key Words**: Computer systems organization, Dependable and fault-tolerant systems and networks, Processors and memory architectures, General and reference, Cross-computing tools and techniques, Evaluation, Security and privacy, Security in hardware, Hardware attacks and countermeasures, Side-channel analysis and countermeasures, 
* **Abstract**: Security-critical data can leak through very unexpected side channels, making side-channel attacks very dangerous threats to information security. Of these, cache-based side-channel attacks are some of the most problematic. This is because caches are essential for the performance of modern computers, but an intrinsic property of all caches - the different access times for cache hits and misses - is the property exploited to leak information in time-based cache side-channel attacks. Recently, different secure cache architectures have been proposed to defend against these attacks. However, we do not have a reliable method for evaluating a cache's resilience against different classes of cache side-channel attacks, which is the goal of this paper.

---
### Constructing and characterizing covert channels on GPGPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124538
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124538?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Single instruction, multiple data, Security and privacy, Security in hardware, Hardware attacks and countermeasures, Hardware reverse engineering, 
* **Abstract**: General Purpose Graphics Processing Units (GPGPUs) are present in most modern computing platforms. They are also increasingly integrated as a computational resource on clusters, data centers, and cloud infrastructure, making them possible targets for attacks. We present a first study of covert channel attacks on GPGPUs. GPGPU attacks offer a number of attractive properties relative to CPU covert channels. These channels also have characteristics different from their counterparts on CPUs. To enable the attack, we first reverse engineer the hardware block scheduler as well as the warp to warp scheduler to characterize how co-location is established. We exploit this information to manipulate the scheduling algorithms to create co-residency between the trojan and the spy. We study contention on different resources including caches, functional units and memory, and construct operational covert channels on all these resources. We also investigate approaches to increase the bandwidth of the channel including: (1) using synchronization to reduce the communication cycle and increase robustness of the channel; (2) exploiting the available parallelism on the GPU to increase the bandwidth; and (3) exploiting the scheduling algorithms to create exclusive co-location to prevent interference from other possible applications. We demonstrate operational versions of all channels on three different Nvidia GPGPUs, obtaining error-free bandwidth of over 4 Mbps, making it the fastest known microarchitectural covert channel under realistic conditions.

---
### Scale-out acceleration for machine learning.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123979
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123979?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Cloud computing, Computing methodologies, Machine learning, Hardware, Integrated circuits, Reconfigurable logic and FPGAs, Hardware accelerators, 
* **Abstract**: The growing scale and complexity of Machine Learning (ML) algorithms has resulted in prevalent use of distributed general-purpose systems. In a rather disjoint effort, the community is focusing mostly on high performance single-node accelerators for learning. This work bridges these two paradigms and offers CoSMIC, a full computing stack constituting language, compiler, system software, template architecture, and circuit generators, that enable programmable acceleration of learning at scale. CoSMIC enables programmers to exploit scale-out acceleration using FPGAs and Programmable ASICs (P-ASICs) from a high-level and mathematical Domain-Specific Language (DSL). Nonetheless, CoSMIC does not require programmers to delve into the onerous task of system software development or hardware design. CoSMIC achieves three conflicting objectives of efficiency, automation, and programmability, by integrating a novel multi-threaded template accelerator architecture and a cohesive stack that generates the hardware and software code from its high-level DSL. CoSMIC can accelerate a wide range of learning algorithms that are most commonly trained using parallel variants of gradient descent. The key is to distribute partial gradient calculations of the learning algorithms across the accelerator-augmented nodes of the scale-out system. Additionally, CoSMIC leverages the parallelizability of the algorithms to offer multi-threaded acceleration within each node. Multi-threading allows CoSMIC to efficiently exploit the numerous resources that are becoming available on modern FPGAs/P-ASICs by striking a balance between multi-threaded parallelism and single-threaded performance. CoSMIC takes advantage of algorithmic properties of ML to offer a specialized system software that optimizes task allocation, role-assignment, thread management, and internode communication. We evaluate the versatility and efficiency of CoSMIC for 10 different machine learning applications from various domains. On average, a 16-node CoSMIC with UltraScale+ FPGAs offers 18.8× speedup over a 16-node Spark system with Xeon processors while the programmer only writes 22--55 lines of code. CoSMIC offers higher scalability compared to the state-of-the-art Spark; scaling from 4 to 16 nodes with CoSMIC yields 2.7× improvements whereas Spark offers 1.8×. These results confirm that the full-stack approach of CoSMIC takes an effective and vital step towards enabling scale-out acceleration for machine learning.

---
### Bit-pragmatic deep neural network computing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123982
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123982?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Single instruction, multiple data, Computing methodologies, Machine learning, Machine learning approaches, Neural networks, Hardware, Integrated circuits, Logic circuits, Arithmetic and datapath circuits, 
* **Abstract**: Deep Neural Networks expose a high degree of parallelism, making them amenable to highly data parallel architectures. However, data-parallel architectures often accept inefficiency in individual computations for the sake of overall efficiency. We show that on average, activation values of convolutional layers during inference in modern Deep Convolutional Neural Networks (CNNs) contain 92% zero bits. Processing these zero bits entails ineffectual computations that could be skipped. We propose Pragmatic (PRA), a massively data-parallel architecture that eliminates most of the ineffectual computations on-the-fly, improving performance and energy efficiency compared to state-of-the-art high-performance accelerators [5]. The idea behind PRA is deceptively simple: use serial-parallel shift-and-add multiplication while skipping the zero bits of the serial input. However, a straightforward implementation based on shift-and-add multiplication yields unacceptable area, power and memory access overheads compared to a conventional bit-parallel design. PRA incorporates a set of design decisions to yield a practical, area and energy efficient design.

---
### CirCNN: accelerating and compressing deep neural networks using block-circulant weight matrices.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124552
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124552?download=true
* **Key Words**: Computer systems organization, Embedded and cyber-physical systems, Embedded systems, Embedded hardware, 
* **Abstract**: Large-scale deep neural networks (DNNs) are both compute and memory intensive. As the size of DNNs continues to grow, it is critical to improve the energy efficiency and performance while maintaining accuracy. For DNNs, the model size is an important factor affecting performance, scalability and energy efficiency. Weight pruning achieves good compression ratios but suffers from three drawbacks: 1) the irregular network structure after pruning, which affects performance and throughput; 2) the increased training complexity; and 3) the lack of rigirous guarantee of compression ratio and inference accuracy.

---
### Using branch predictors to predict brain activity in brain-machine implants.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123943
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123943?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Special purpose systems, Embedded and cyber-physical systems, Embedded systems, Embedded hardware, Real-time systems, Real-time system architecture, Hardware, Emerging technologies, Biology-related information processing, Bio-embedded electronics, Neural systems, 
* **Abstract**: A key problem with implantable brain-machine interfaces is that they need extreme energy efficiency. One way of lowering energy consumption is to use the low power modes available on the processors embedded in these devices. We present a technique to predict when neuronal activity of interest is likely to occur so that the processor can run at nominal operating frequency at those times, and be placed in low power modes otherwise. To achieve this, we discover that branch predictors can also predict brain activity. We perform brain surgeries on awake and anesthetized mice, and evaluate the ability of several branch predictors to predict neuronal activity in the cerebellum. We find that perceptron branch predictors can predict cerebellar activity with accuracies as high as 85%. Consequently, we co-opt branch predictors to dictate when to transition between low power and normal operating modes, saving as much as 59% of processor energy.

---
### Load value prediction via path-based address prediction: avoiding mispredictions due to conflicting stores.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123951
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123951?download=true
* **Key Words**: Computer systems organization, Architectures, Serial architectures, Pipeline computing, Reduced instruction set computing, Superscalar architectures, 
* **Abstract**: Current flagship processors excel at extracting instruction-level-parallelism (ILP) by forming large instruction windows. Even then, extracting ILP is inherently limited by true data dependencies. Value prediction was proposed to address this limitation. Many challenges face value prediction, in this work we focus on two of them. Challenge #1: store instructions change the values in memory, rendering the values in the value predictor stale, and resulting in value mispredictions and a retraining penalty. Challenge #2: value mispredictions trigger costly pipeline flushes. To minimize the number of pipeline flushes, value predictors employ stringent, yet necessary, high confidence requirements to guarantee high prediction accuracy. Such requirements can negatively impact training time and coverage.

---
### Multiperspective reuse prediction.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123942
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123942?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Hardware, Integrated circuits, Semiconductor memory, Static memory, 
* **Abstract**: The disparity between last-level cache and memory latencies motivates the search for efficient cache management policies. Recent work in predicting reuse of cache blocks enables optimizations that significantly improve cache performance and efficiency. However, the accuracy of the prediction mechanisms limits the scope of optimization.

---
### CSALT: context switch aware large TLB.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124549
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124549?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, 
* **Abstract**: Computing in virtualized environments has become a common practice for many businesses. Typically, hosting companies aim for lower operational costs by targeting high utilization of host machines maintaining just enough machines to meet the demand. In this scenario, frequent virtual machine context switches are common, resulting in increased TLB miss rates (often, by over 5X when contexts are doubled) and subsequent expensive page walks. Since each TLB miss in a virtual environment initiates a 2D page walk, the data caches get filled with a large fraction of page table entries (often, in excess of 50%) thereby evicting potentially more useful data contents.

---
### RTLcheck: verifying the memory consistency of RTL designs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124536
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124536?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Hardware, Hardware validation, Functional verification, Assertion checking, 
* **Abstract**: Paramount to the viability of a parallel architecture is the correct implementation of its memory consistency model (MCM). Although tools exist for verifying consistency models at several design levels, a problematic verification gap exists between checking an abstract microarchitectural specification of a consistency model and verifying that the actual processor RTL implements it correctly.

---
### Architecting hierarchical coherence protocols for push-button parametric verification.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123971
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123971?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Hardware, Hardware validation, Functional verification, Model checking, 
* **Abstract**: Recent work in formal verification theory and verification-aware design has sought to bridge the divide between the class of protocols architects want to design and the class of protocols that are verifiable with state of the art tools. Particularly the recent Neo work in formal verification theory, for the first time, formalizes how to compose flat subprotocols with an arbitrary number of nodes into a hierarchy while maintaining correct behavior. However, it is unclear if this theory scales to realistic systems. Moreover, there is a diversity of systems architects would be interested in, to which it is not clear if the theory applies.

---
### PARSNIP: performant architecture for race safety with no impact on precision.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123946
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123946?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Software and its engineering, Software notations and tools, Software maintenance tools, 
* **Abstract**: Data race detection is a useful dynamic analysis for multithreaded programs that is a key building block in record-and-replay, enforcing strong consistency models, and detecting concurrency bugs. Existing software race detectors are precise but slow, and hardware support for precise data race detection relies on assumptions like type safety that many programs violate in practice.

---
### Harnessing voltage margins for energy efficiency in multicore CPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124537
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124537?download=true
* **Key Words**: Hardware, Power and energy, Power estimation and optimization, Robustness, Hardware reliability, Process, voltage and temperature variations, 
* **Abstract**: In this paper, we present the first automated system-level analysis of multicore CPUs based on ARMv8 64-bit architecture (8-core, 28nm X-Gene 2 micro-server by AppliedMicro) when pushed to operate in scaled voltage conditions. We report detailed system-level effects including SDCs, corrected/uncorrected errors and application/system crashes. Our study reveals large voltage margins (that can be harnessed for energy savings) and also large Vmin variation among the 8 cores of the CPU chip, among 3 different chips (a nominal rated and two sigma chips), and among different benchmarks.

---
### Race-to-sleep + content caching + display caching: a recipe for energy-efficient video streaming on handhelds.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123948
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123948?download=true
* **Key Words**: Computer systems organization, Architectures, Embedded and cyber-physical systems, Embedded systems, Embedded hardware, Human-centered computing, Ubiquitous and mobile computing, Ubiquitous and mobile computing theory, concepts and paradigms, Mobile computing, 
* **Abstract**: Video streaming has become the most common application in handhelds and this trend is expected to grow in future to account for about 75% of all mobile data traffic by 2021. Thus, optimizing the performance and energy consumption of video processing in mobile devices is critical for sustaining the handheld market growth. In this paper, we propose three complementary techniques, race-to-sleep, content caching and display caching, to minimize the energy consumption of the video processing flows. Unlike the state-of-the-art frame-by-frame processing of a video decoder, the first scheme, race-to-sleep, uses two approaches, called batching of frames and frequency boosting to prolong its sleep state for saving energy, while avoiding any frame drops. The second scheme, content caching, exploits the content similarity of smaller video blocks, called macroblocks, to design a novel cache organization for reducing the memory pressure. The third scheme, in turn, takes advantage of content similarity at the display controller to facilitate display caching further improving energy efficiency. We integrate these three schemes for developing an end-to-end video processing framework and evaluate our design on a comprehensive mobile system design platform with a variety of video processing workloads. Our evaluations show that the proposed three techniques complement each other in improving performance by avoiding frame drops and reducing the energy consumption of video streaming applications by 21%, on average, compared to the current baseline design.

---
### BVF: enabling significant on-chip power savings via bit-value-favor for throughput processors.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123944
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123944?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Single instruction, multiple data, Hardware, Integrated circuits, Semiconductor memory, Dynamic memory, Static memory, Power and energy, Power estimation and optimization, 
* **Abstract**: Power reduction is one of the primary tasks for designing modern processors, especially for high-performance throughput processors such as GPU due to their high power budget. In this paper, we propose a novel circuit-architecture co-design scheme to harvest enormous power savings for GPU on-chip SRAM and interconnects. We propose a new 8T SRAM that exhibits asymmetric energy consumption for bit value 0/1, in terms of read, write and standby. We name this feature Bit-Value-Favor (BVF). To harvest the power benefits from BVF on GPUs, we propose three coding methods at architectural level to maximize the occurrence of bit-1s over bit-0s in the on-chip data and instruction streams, leading to substantial chip-level power reduction. Experimental results across a large spectrum of 58 representative GPU applications demonstrate that our proposed BVF design can bring an average of 21% and 24% chip power reduction under 28nm and 40nm process technologies, with negligible design overhead. Further sensitivity studies show that the effectiveness of our design is robust to DVFS, warp scheduling policies and different SRAM capacities.

---
### Xylem: enhancing vertical thermal conduction in 3D processor-memory stacks.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124547
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124547?download=true
* **Key Words**: Computer systems organization, Architectures, Hardware, Integrated circuits, 3D integrated circuits, 
* **Abstract**: In upcoming architectures that stack processor and DRAM dies, temperatures are higher because of the increased transistor density and the high inter-layer thermal resistance. However, past research has underestimated the extent of the thermal bottleneck. Recent experimental work shows that the Die-to-Die (D2D) layers hinder effective heat transfer, likely leading to the capping of core frequencies.

---
### Unleashing the power of GPU for physically-based rendering via dynamic ray shuffling.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124532
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124532?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Single instruction, multiple data, 
* **Abstract**: Computer graphics is generally divided into two branches: real-time rendering and physically-based rendering. Conventional graphics processing units (GPUs) were designed to accelerate the former which is based on the standard Z-buffer algorithm. However, many applications in entertainment, science, and industry require high quality visual effects such as soft-shadows, reflections, and diffuse lighting interactions which are difficult to achieve with the Z-buffer algorithm, but are straightforward to implement using physically-based rendering methods. Physically-based rendering can already be implemented on present programmable GPUs. However, for physically-based rendering on GPUs, a large portion of the processing power is wasted due to low utilization of SIMD units. This is because the core algorithm of physically-based rendering, ray tracing, suffers from Single Instruction, Multiple Thread (SIMT) control flow divergences. In this paper, we propose the Dynamic Ray Shuffling (DRS) architecture for GPUs to address this problem. Our key insight is that the primary control flow divergences are caused by inconsistent ray traversal states of a warp, and can be eliminated by dynamically shuffling rays. Experimental results show that, for an estimated 0.11% area cost, DRS significantly improves the SIMD efficiency for the tested benchmarks from 41.06% to 81.04% on average. With this, the performance of a physically-based rendering method such as path tracing can be improved by 1.67X--1.92X, and 1.79X on average.

---
### GPUpd: a fast and scalable multi-GPU architecture using cooperative projection and distribution.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123968
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123968?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Computing methodologies, Computer graphics, Graphics systems and interfaces, Graphics processors, 
* **Abstract**: Graphics Processing Unit (GPU) vendors have been scaling single-GPU architectures to satisfy the ever-increasing user demands for faster graphics processing. However, as it gets extremely difficult to further scale single-GPU architectures, the vendors are aiming to achieve the scaled performance by simultaneously using multiple GPUs connected with newly developed, fast inter-GPU networks (e.g., NVIDIA NVLink, AMD XDMA). With fast inter-GPU networks, it is now promising to employ split frame rendering (SFR) which improves both frame rate and single-frame latency by assigning disjoint regions of a frame to different GPUs. Unfortunately, the scalability of current SFR implementations is seriously limited as they suffer from a large amount of redundant computation among GPUs.

---
### Versapipe: a versatile programming framework for pipelined computing on GPU.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123978
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123978?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, Computing methodologies, Parallel computing methodologies, General and reference, Cross-computing tools and techniques, Performance, 
* **Abstract**: Pipeline is an important programming pattern, while GPU, designed mostly for data-level parallel executions, lacks an efficient mechanism to support pipeline programming and executions. This paper provides a systematic examination of various existing pipeline execution models on GPU, and analyzes their strengths and weaknesses. To address their shortcomings, this paper then proposes three new execution models equipped with much improved controllability, including a hybrid model that is capable of getting the strengths of all. These insights ultimately lead to the development of a software programming framework named VersaPipe. With VersaPipe, users only need to write the operations for each pipeline stage. VersaPipe will then automatically assemble the stages into a hybrid execution model and configure it to achieve the best performance. Experiments on a set of pipeline benchmarks and a real-world face detection application show that VersaPipe produces up to 6.90X (2.88X on average) speedups over the original manual implementations.

---
### Wireframe: supporting data-dependent parallelism through dependency graph execution in GPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123976
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123976?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Data flow architectures, Parallel architectures, Single instruction, multiple data, 
* **Abstract**: GPUs lack fundamental support for data-dependent parallelism and synchronization. While CUDA Dynamic Parallelism signals progress in this direction, many limitations and challenges still remain. This paper introduces Wireframe, a hardware-software solution that enables generalized support for data-dependent parallelism and synchronization. Wireframe enables applications to naturally express execution dependencies across different thread blocks through a dependency graph abstraction at run-time, which is sent to the GPU hardware at kernel launch. At run-time, the hardware enforces the dependencies specified in the dependency graph through a dependency-aware thread block scheduler. Overall, Wireframe is able to improve total execution time up to 65.20% with an average of 45.07%.

---
### Schedtask: a hardware-assisted task scheduler.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123984
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123984?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Cloud computing, Parallel architectures, Multicore architectures, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Memory management, Virtual memory, Process management, Scheduling, 
* **Abstract**: The execution of workloads such as web servers and database servers typically switches back and forth between different tasks such as user applications, system call handlers, and interrupt handlers. The combined size of the instruction footprints of such tasks typically exceeds that of the i-cache (16--32 KB). This causes a lot of i-cache misses and thereby reduces the application's performance. Hence, we propose SchedTask, a hardware-assisted task scheduler that improves the performance of such workloads by executing tasks with similar instruction footprints on the same core. We start by decomposing the combined execution of the OS and the applications into sequences of instructions called SuperFunctions. We propose a scheme to determine the amount of overlap between the instruction footprints of different SuperFunctions by using Bloom filters. We then use a hierarchical scheduler to execute SuperFunctions with similar instruction footprints on the same core. For a suite of 8 popular OS-intensive workloads, we report an increase in the application's performance of up to 29 percentage points (mean: 11.4 percentage points) over state of the art scheduling techniques.

---
### Exploiting heterogeneity for tail latency and energy efficiency.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123956
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123956?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Process management, Scheduling, 
* **Abstract**: Interactive service providers have strict requirements on high-percentile (tail) latency to meet user expectations. If providers meet tail latency targets with less energy, they increase profits, because energy is a significant operating expense. Unfortunately, optimizing tail latency and energy are typically conflicting goals. Our work resolves this conflict by exploiting servers with per-core Dynamic Voltage and Frequency Scaling (DVFS) and Asymmetric Multicore Processors (AMPs). We introduce the Adaptive Slow-to-Fast scheduling framework, which matches the heterogeneity of the workload --- a mix of short and long requests --- to the heterogeneity of the hardware --- cores running at different speeds. The scheduler prioritizes long requests to faster cores by exploiting the insight that long requests reveal themselves. We use control theory to design threshold-based scheduling policies that use individual request progress, load, competition, and latency targets to optimize performance and energy. We configure our framework to optimize Energy Efficiency for a given Tail Latency (EETL) for both DVFS and AMP. In this framework, each request self-schedules, starting on a slow core and then migrating itself to faster cores. At high load, when a desired AMP core speed s is not available for a request but a faster core is, the longest request on an s core type migrates early to make room for the other request. Compared to per-core DVFS systems, EETL for AMPs delivers the same tail latency, reduces energy by 18% to 50%, and improves capacity (throughput) by 32% to 82%. We demonstrate that our framework effectively exploits dynamic DVFS and static AMP heterogeneity to reduce provisioning and operational costs for interactive services.

---
### TMI: thread memory isolation for false sharing repair.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123947
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123947?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Software and its engineering, Software notations and tools, Compilers, Runtime environments, 
* **Abstract**: Cache contention in the form of false sharing and true sharing arises when threads overshare cache lines at high frequency. Such oversharing can reduce or negate the performance benefits of parallel execution. Prior systems for detecting and repairing cache contention lack efficiency in detection or repair, contain subtle memory consistency flaws, or require invasive changes to the program environment.

---
### Estimating and understanding architectural risk.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124541
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124541?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Computing methodologies, Modeling and simulation, Model development and analysis, Modeling methodologies, Uncertainty quantification, 
* **Abstract**: Designing a system in an era of rapidly evolving application behaviors and significant technology shifts involves taking on risk that a design will fail to meet its performance goals. While risk assessment and management are expected in both business and investment, these aspects are typically treated as independent to questions of performance and efficiency in architecture analysis. As hardware and software characteristics become uncertain (i.e. samples from a distribution), we demonstrate that the resulting performance distributions quickly grow beyond our ability to reason about with intuition alone. We further show that knowledge of the performance distribution can be used to significantly improve both the average case performance and minimize the risk of under-performance (which we term architectural risk). Our automated framework can be used to quantify the areas where trade-offs between expected performance and the "tail" of performance are most acute and provide new insights supporting architectural decision making (such as core selection) under uncertainty. Importantly it can do this even without a priori knowledge of an analytic model governing that uncertainty.

---
### Hybrid analog-digital solution of nonlinear partial differential equations.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124550
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124550?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Analog computers, Heterogeneous (hybrid) systems, Hardware, Very large scale integration design, Application-specific VLSI designs, Application specific integrated circuits, Mathematics of computing, Mathematical analysis, Differential equations, Partial differential equations, Nonlinear equations, 
* **Abstract**: We tackle the important problem class of solving nonlinear partial differential equations. While nonlinear PDEs are typically solved in high-performance supercomputers, they are increasingly used in graphics and embedded systems, where efficiency is important.

---
### Taming the instruction bandwidth of quantum computers via hardware-managed error correction.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123940
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123940?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Quantum computing, 
* **Abstract**: A quantum computer consists of quantum bits (qubits) and a control processor that acts as an interface between the programmer and the qubits. As qubits are very sensitive to noise, they rely on continuous error correction to maintain the correct state. Current proposals rely on software-managed error correction and require large instruction bandwidth, which must scale in proportion to the number of qubits. While such a design may be reasonable for small-scale quantum computers, we show that instruction bandwidth tends to become a critical bottleneck for scaling quantum computers.

---
### Optimized surface code communication in superconducting quantum computers.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123949
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123949?download=true
* **Key Words**: Hardware, Emerging technologies, Quantum technologies, Quantum computation, Quantum error correction and fault tolerance, 
* **Abstract**: Quantum computing (QC) is at the cusp of a revolution. Machines with 100 quantum bits (qubits) are anticipated to be operational by 2020 [30, 73], and several-hundred-qubit machines are around the corner. Machines of this scale have the capacity to demonstrate quantum supremacy, the tipping point where QC is faster than the fastest classical alternative for a particular problem. Because error correction techniques will be central to QC and will be the most expensive component of quantum computation, choosing the lowest-overhead error correction scheme is critical to overall QC success. This paper evaluates two established quantum error correction codes---planar and double-defect surface codes---using a set of compilation, scheduling and network simulation tools. In considering scalable methods for optimizing both codes, we do so in the context of a full microarchitectural and compiler analysis. Contrary to previous predictions, we find that the simpler planar codes are sometimes more favorable for implementation on superconducting quantum computers, especially under conditions of high communication congestion.

---
### Architectural tradeoffs for biodegradable computing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123980
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123980?download=true
* **Key Words**: Hardware, Electronic design automation, Modeling and parameter extraction, Emerging technologies, Analysis and design of emerging devices and systems, Emerging architectures, Emerging simulation, Circuit substrates, Carbon based electronics, Power and energy, Impact on the environment, Very large scale integration design, Standard cell libraries, Social and professional topics, Professional topics, Computing industry, Sustainability, 
* **Abstract**: Organic thin-film transistors (OTFTs) have attracted increased attention because of the possibility to produce environmentally friendly low-cost, lightweight, flexible, and even biodegradable devices. With an increasing number of complex applications being proposed for organic and biodegradable semiconductors, the need for computation horsepower also rises. However, due to the process characteristic differences, direct adaptation of silicon-based circuit designs and traditional computer architecture wisdom is not applicable.

---
### Improving the effectiveness of searching for isomorphic chains in superword level parallelism.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3124554
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3124554?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Single instruction, multiple data, Software and its engineering, Software notations and tools, Compilers, Source code generation, 
* **Abstract**: Most high-performance microprocessors come equipped with general-purpose Single Instruction Multiple Data (SIMD) execution engines to enhance performance. Compilers use auto-vectorization techniques to identify vector parallelism and generate SIMD code so that applications can enjoy the performance benefits provided by SIMD units. Superword Level Parallelism (SLP), one such vectorization technique, forms vector operations by merging isomorphic instructions into a vector operation and linking many such operations into long isomorphic chains. However, effective grouping of isomorphic instructions remains a key challenge for SLP algorithms.

---
### Data movement aware computation partitioning.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123954
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123954?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, 
* **Abstract**: Data access costs dominate the execution times of most parallel applications and they are expected to be even more important in the future. To address this, recent research has focused on Near Data Processing (NDP) as a new paradigm that tries to bring computation to data, instead of bringing data to computation (which is the norm in conventional computing). This paper explores the potential of compiler support in exploiting NDP in the context of emerging manycore systems. To that end, we propose a novel compiler algorithm that partitions the computations in a given loop nest into subcomputations and schedules the resulting subcomputations on different cores with the goal of reducing the distance-to-data on the on-chip network. An important characteristic of our approach is that it exploits NDP while taking advantage of data locality. Our experiments with 12 multithreaded applications running on a state-of-the-art commercial manycore system indicate that the proposed compiler-based approach significantly reduces data movements on the on-chip network by taking advantage of NDP, and these benefits lead to an average execution time improvement of 18.4%.

---
### Mirage cores: the illusion of many out-of-order cores using in-order hardware.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123969
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123969?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, Parallel architectures, Multicore architectures, Hardware, Power and energy, Power estimation and optimization, Chip-level power issues, 
* **Abstract**: Heterogenous chip multiprocessors (Het-CMPs) offer a combination of large Out-of-Order (OoO) cores optimized for high single-threaded performance and small In-Order (InO) cores optimized for low-energy and area costs. Due to practical constraints, CMP designers must choose to either optimize for total system throughput by utilizing many InO cores or maximize single-thread execution with fewer OoO cores. We propose Mirage Cores, a novel Het-CMP design where clusters of InO cores are architected around an OoO in a manner that optimizes for both throughput and single-thread performance. The insight behind Mirage Cores is that InO cores can achieve near-OoO performance if they are provided with the dynamic instruction schedule of an OoO core. To leverage this, Mirage Cores employs an OoO core as an optimal instruction schedule generator as well as a high-performance alternative for all neighboring InO cores. We also develop intelligent runtime schedulers which orchestrate the arbitration and migration of applications between the InO cores and the central OoO. Fast and timely transfer of dynamic schedules from the OoO to InO allows Mirage Cores to create the appearance of all OoO cores to the user using underlying In-Order hardware.

---
### Using intra-core loop-task accelerators to improve the productivity and performance of task-based parallel programs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3136952
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3136952?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Single instruction, multiple data, Software and its engineering, Software notations and tools, Compilers, Runtime environments, 
* **Abstract**: Task-based parallel programming frameworks offer compelling productivity and performance benefits for modern chip multi-processors (CMPs). At the same time, CMPs also provide packed-SIMD units to exploit fine-grain data parallelism. Two fundamental challenges make using packed-SIMD units with task-parallel programs particularly difficult: (1) the intra-core parallel abstraction gap; and (2) inefficient execution of irregular tasks. To address these challenges, we propose augmenting CMPs with intra-core loop-task accelerators (LTAs). We introduce a lightweight hint in the instruction set to elegantly encode loop-task execution and an LTA microarchitectural template that can be configured at design time for different amounts of spatial/temporal decoupling to efficiently execute both regular and irregular loop tasks. Compared to an in-order CMP baseline, CMP+LTA results in an average speedup of 4.2X (1.8X area normalized) and similar energy efficiency. Compared to an out-of-order CMP baseline, CMP+LTA results in an average speedup of 2.3X (1.5X area normalized) and also improves energy efficiency by 3.2X. Our work suggests augmenting CMPs with lightweight LTAs can improve performance and efficiency on both regular and irregular loop-task parallel programs with minimal software changes.

---
### Architectural opportunities for novel dynamic EMI shifting (DEMIS).
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123973
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123973?download=true
* **Key Words**: Hardware, Communication hardware, interfaces and storage, Signal processing systems, Noise reduction, Wireless devices, Robustness, Hardware reliability, Signal integrity and noise analysis, 
* **Abstract**: Processors emit non-trivial amounts of electromagnetic radiation, creating interference in frequency bands used by wireless communication technologies such as cellular, WiFi and Bluetooth. We introduce the problem of in-band radio frequency noise as a form of electromagnetic interference (EMI) to the computer architecture community as a technical challenge to be addressed.

---
### DeftNN: addressing bottlenecks for DNN execution on GPUs via synapse vector elimination and near-compute data fission.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123970
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123970?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Single instruction, multiple data, Computing methodologies, Machine learning, Machine learning approaches, Neural networks, General and reference, Cross-computing tools and techniques, Performance, 
* **Abstract**: Deep neural networks (DNNs) are key computational building blocks for emerging classes of web services that interact in real time with users via voice, images and video inputs. Although GPUs have gained popularity as a key accelerator platform for deep learning workloads, the increasing demand for DNN computation leaves a significant gap between the compute capabilities of GPU-enabled datacenters and the compute needed to service demand.

---
### Hardware supported persistent object address translation.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123981
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123981?download=true
* **Key Words**: Computer systems organization, Architectures, Serial architectures, Superscalar architectures, Hardware, Emerging technologies, Memory and dense storage, 
* **Abstract**: Emerging non-volatile main memory technologies create a new opportunity for writing programs with a large, byte-addressable persistent storage that can be accessed through regular memory instructions. These new memory-as-storage technologies impose significant challenges to current programming models. In particular, some emerging persistent programming frameworks, like the NVM Library (NVML), implement relocatable persistent objects that can be mapped anywhere in the virtual address space. To make this work, persistent objects are referenced using object identifiers (ObjectID), rather than pointers, that need to be translated to an address before the object can be read or written. Frequent translation from ObjectID to address incurs significant overhead.

---
### An experimental microarchitecture for a superconducting quantum processor.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3123939.3123952
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3123939.3123952?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Quantum computing, General and reference, Document types, General conference proceedings, Hardware, Emerging technologies, Quantum technologies, 
* **Abstract**: Quantum computers promise to solve certain problems that are intractable for classical computers, such as factoring large numbers and simulating quantum systems. To date, research in quantum computer engineering has focused primarily at opposite ends of the required system stack: devising high-level programming languages and compilers to describe and optimize quantum algorithms, and building reliable low-level quantum hardware. Relatively little attention has been given to using the compiler output to fully control the operations on experimental quantum processors. Bridging this gap, we propose and build a prototype of a flexible control microarchitecture supporting quantum-classical mixed code for a superconducting quantum processor. The microarchitecture is based on three core elements: (i) a codeword-based event control scheme, (ii) queue-based precise event timing control, and (iii) a flexible multilevel instruction decoding mechanism for control. We design a set of quantum microinstructions that allows flexible control of quantum operations with precise timing. We demonstrate the microarchitecture and microinstruction set by performing a standard gate-characterization experiment on a transmon qubit.
