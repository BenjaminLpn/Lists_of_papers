### asplos 2016 | 57 papers.
---
### Programming Uncertain <T>jhings.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872416
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872416?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, 
* **Abstract**: Innovation flourishes with good abstractions. For instance, codification of the IEEE Floating Point standard in 1985 was critical to the subsequent success of scientific computing. Programming languages currently lack appropriate abstractions for uncertain data. Applications already use estimates from sensors, machine learning, big data, humans, and approximate algorithms, but most programming languages do not help developers address correctness, programmability, and optimization problems due to estimates.

---
### WiSync: An Architecture for Fast Synchronization through On-Chip Wireless Communication.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872396
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872396?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multiple instruction, multiple data, 
* **Abstract**: In shared-memory multiprocessing, fine-grain synchronization is challenging because it requires frequent communication. As technology scaling delivers larger manycore chips, such pattern is expected to remain costly to support. In this paper, we propose to address this challenge by using on-chip wireless communication. Each core has a transceiver and an antenna to communicate with all the other cores. This environment supports very low latency global communication. Our architecture, called WiSync, uses a per-core Broadcast Memory (BM). When a core writes to its BM, all the other 100+ BMs get updated in less than 10 processor cycles. We also use a second wireless channel with cheaper transfers to execute barriers efficiently. WiSync supports multiprogramming, virtual memory, and context switching. Our evaluation with simulations of 128-threaded kernels and 64-threaded applications shows that WiSync speeds-up synchronization substantially. Compared to using advanced conventional synchronization, WiSync attains an average speedup of nearly one order of magnitude for the kernels, and 1.12 for PARSEC and SPLASH-2.

---
### ReBudget: Trading Off Efficiency vs. Fairness in Market-Based Multicore Resource Allocation via Runtime Budget Reassignment.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872382
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872382?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Theory of computation, Theory and algorithms for application domains, Algorithmic game theory and mechanism design, 
* **Abstract**: Efficiently allocating shared resources in computer systems is critical to optimizing execution. Recently, a number of market-based solutions have been proposed to attack this problem. Some of them provide provable theoretical bounds to efficiency and/or fairness losses under market equilibrium. However, they are limited to markets with potentially important constraints, such as enforcing equal budget for all players, or curve-fitting players' utility into a specific function type. Moreover, they do not generally provide an intuitive "knob" to control efficiency vs. fairness. In this paper, we introduce two new metrics, Market Utility Range (MUR) and Market Budget Range (MBR), through which we provide for the first time theoretical bounds on efficiency and fairness of market equilibria under arbitrary budget assignments. We leverage this result and propose ReBudget, an iterative budget re-assignment algorithm that can be used to control efficiency vs. fairness at run-time. We apply our algorithm to a multi-resource allocation problem in multicore chips. Our evaluation using detailed execution-driven simulations shows that our budget re-assignment technique is intuitive, effective, and efficient.

---
### Dirigent: Enforcing QoS for Latency-Critical Tasks on Shared Multicore Systems.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872394
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872394?download=true
* **Key Words**: Computer systems organization, 
* **Abstract**: Latency-critical applications suffer from both average performance degradation and reduced completion time predictability when collocated with batch tasks. Such variation forces the system to overprovision resources to ensure Quality of Service (QoS) for latency-critical tasks, degrading overall system throughput. We explore the causes of this variation and exploit the opportunities of mitigating variation directly to simultaneously improve both QoS and utilization. We develop, implement, and evaluate Dirigent, a lightweight performance-management runtime system that accurately controls the QoS of latency-critical applications at fine time scales, leveraging existing architecture mechanisms. We evaluate Dirigent on a real machine and show that it is significantly more effective than configurations representative of prior schemes.

---
### Paravirtual Remote I/O.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872378
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872378?download=true
* **Key Words**: Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Software infrastructure, Virtual machines, 
* **Abstract**: The traditional "trap and emulate" I/O paravirtualization model conveniently allows for I/O interposition, yet it inherently incurs costly guest-host context switches. The newer "sidecore" model eliminates this overhead by dedicating host (side)cores to poll the relevant guest memory regions and react accordingly without context switching. But the dedication of sidecores on each host might be wasteful when I/O activity is low, or it might not provide enough computational power when I/O activity is high. We propose to alleviate this problem at rack scale by consolidating the dedicated sidecores spread across several hosts onto one server. The hypervisor is then effectively split into two parts: the local hypervisor that hosts the VMs, and the remote hypervisor that processes their paravirtual I/O. We call this model vRIO---paraVirtual Remote I/O. We find that by increasing the latency somewhat, it provides comparable throughput with fewer sidecores and superior throughput with the same number of sidecores as compared to the state of the art. vRIO additionally constitutes a new, cost-effective way to consolidate I/O devices (on the remote hypervisor) while supporting efficient programmable I/O interposition.

---
### High Performance Packet Processing with FlexNIC.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872367
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872367?download=true
* **Key Words**: Hardware, Communication hardware, interfaces and storage, Networking hardware, Networks, Network architectures, Network components, End nodes, Network adapters, 
* **Abstract**: The recent surge of network I/O performance has put enormous pressure on memory and software I/O processing sub systems. We argue that the primary reason for high memory and processing overheads is the inefficient use of these resources by current commodity network interface cards (NICs). We propose FlexNIC, a flexible network DMA interface that can be used by operating systems and applications alike to reduce packet processing overheads. FlexNIC allows services to install packet processing rules into the NIC, which then executes simple operations on packets while exchanging them with host memory. Thus, our proposal moves some of the packet processing traditionally done in software to the NIC, where it can be done flexibly and at high speed.

---
### Specifying and Checking File System Crash-Consistency Models.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872406
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872406?download=true
* **Key Words**: Social and professional topics, Professional topics, Management of computing and information systems, File systems management, Software and its engineering, Software organization and properties, Software functional properties, Formal methods, Software verification, 
* **Abstract**: Applications depend on persistent storage to recover state after system crashes. But the POSIX file system interfaces do not define the possible outcomes of a crash. As a result, it is difficult for application writers to correctly understand the ordering of and dependencies between file system operations, which can lead to corrupt application state and, in the worst case, catastrophic data loss. This paper presents crash-consistency models, analogous to memory consistency models, which describe the behavior of a file system across crashes. Crash-consistency models include both litmus tests, which demonstrate allowed and forbidden behaviors, and axiomatic and operational specifications. We present a formal framework for developing crash-consistency models, and a toolkit, called Ferrite, for validating those models against real file system implementations. We develop a crash-consistency model for ext4, and use Ferrite to demonstrate unintuitive crash behaviors of the ext4 implementation. To demonstrate the utility of crash-consistency models to application writers, we use our models to prototype proof-of-concept verification and synthesis tools, as well as new library interfaces for crash-safe applications.

---
### Prudent Memory Reclamation in Procrastination-Based Synchronization.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872405
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2980024.2872405?download=true
* **Key Words**: Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Memory management, Allocation / deallocation strategies, 
* **Abstract**: Procrastination is the fundamental technique used in synchronization mechanisms such as Read-Copy-Update (RCU) where writers, in order to synchronize with readers, defer the freeing of an object until there are no readers referring to the object. The synchronization mechanism determines when the deferred object is safe to reclaim and when it is actually reclaimed. Hence, such memory reclamations are completely oblivious of the memory allocator state. This induces poor memory allocator performance, for instance, when the reclamations are ill-timed. Furthermore, deferred objects provide hints about the future that inform memory regions that are about to be freed. Although useful, hints are not exploited as deferred objects are not visible to memory allocators. We introduce Prudence, a dynamic memory allocator, that is tightly integrated with the synchronization mechanism to ensure visibility of deferred objects to the memory allocator. Such an integration enables Prudence to (i) identify the safe time to reclaim deferred objects' memory, (ii) have an inclusive view of the allocated, free and about-to-be-freed objects, and (iii) exploit optimizations based on the hints about the future during important state transitions. Our evaluation in the Linux kernel shows that Prudence integrated with RCU performs 3.9X to 28X better in micro-benchmarks compared to SLUB, a recent memory allocator in the Linux kernel. It also improves the overall performance perceptibly (4%-18%) for a mix of widely used synthetic and application benchmarks. Further, it performs better (up to 98%) in terms of object hits in caches, object cache churns, slab churns, peak memory usage and total fragmentation, when compared with the SLUB allocator.

---
### Whirlpool: Improving Dynamic Cache Management with Static Data Classification.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872363
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2980024.2872363?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, 
* **Abstract**: Cache hierarchies are increasingly non-uniform and difficult to manage. Several techniques, such as scratchpads or reuse hints, use static information about how programs access data to manage the memory hierarchy. Static techniques are effective on regular programs, but because they set fixed policies, they are vulnerable to changes in program behavior or available cache space. Instead, most systems rely on dynamic caching policies that adapt to observed program behavior. Unfortunately, dynamic policies spend significant resources trying to learn how programs use memory, and yet they often perform worse than a static policy. We present Whirlpool, a novel approach that combines static information with dynamic policies to reap the benefits of each. Whirlpool statically classifies data into pools based on how the program uses memory. Whirlpool then uses dynamic policies to tune the cache to each pool. Hence, rather than setting policies statically, Whirlpool uses static analysis to guide dynamic policies. We present both an API that lets programmers specify pools manually and a profiling tool that discovers pools automatically in unmodified binaries.

---
### TPC: Target-Driven Parallelism Combining Prediction and Correction to Reduce Tail Latency in Interactive Services.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872370
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2980024.2872370?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Client-server architectures, Computing methodologies, Machine learning, Learning paradigms, Supervised learning, Supervised learning by regression, Information systems, Information retrieval, Evaluation of retrieval results, Retrieval efficiency, Search engine architectures and scalability, Distributed retrieval, World Wide Web, Web searching and information discovery, Web search engines, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Process management, Multithreading, Scheduling, Theory of computation, Theory and algorithms for application domains, Machine learning theory, Boosting, 
* **Abstract**: In interactive services such as web search, recommendations, games and finance, reducing the tail latency is crucial to provide fast response to every user. Using web search as a driving example, we systematically characterize interactive workload to identify the opportunities and challenges for reducing tail latency. We find that the workload consists of mainly short requests that do not benefit from parallelism, and a few long requests which significantly impact the tail but exhibit high parallelism speedup. This motivates estimating request execution time, using a predictor, to identify long requests and to parallelize them. Prediction, however, is not perfect; a long request mispredicted as short is likely to contribute to the server tail latency, setting a ceiling on the achievable tail latency. We propose TPC, an approach that combines prediction information judiciously with dynamic correction for inaccurate prediction. Dynamic correction increases parallelism to accelerate a long request that is mispredicted as short. TPC carefully selects the appropriate target latencies based on system load and parallelism efficiency to reduce tail latency.

---
### How to Build Static Checking Systems Using Orders of Magnitude Less Code.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872364
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872364?download=true
* **Key Words**: Theory of computation, Semantics and reasoning, Program reasoning, Program analysis, 
* **Abstract**: Modern static bug finding tools are complex. They typically consist of hundreds of thousands of lines of code, and most of them are wedded to one language (or even one compiler). This complexity makes the systems hard to understand, hard to debug, and hard to retarget to new languages, thereby dramatically limiting their scope. This paper reduces checking system complexity by addressing a fundamental assumption, the assumption that checkers must depend on a full-blown language specification and compiler front end. Instead, our program checkers are based on drastically incomplete language grammars ("micro-grammars") that describe only portions of a language relevant to a checker. As a result, our implementation is tiny-roughly 2500 lines of code, about two orders of magnitude smaller than a typical system. We hope that this dramatic increase in simplicity will allow people to use more checkers on more systems in more languages.

---
### TxRace: Efficient Data Race Detection Using Commodity Hardware Transactional Memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872384
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872384?download=true
* **Key Words**: Software and its engineering, Software creation and management, Software verification and validation, Software defect analysis, Software testing and debugging, Software notations and tools, General programming languages, Language types, Concurrent programming languages, 
* **Abstract**: Detecting data races is important for debugging shared-memory multithreaded programs, but the high runtime overhead prevents the wide use of dynamic data race detectors. This paper presents TxRace, a new software data race detector that leverages commodity hardware transactional memory (HTM) to speed up data race detection. TxRace instruments a multithreaded program to transform synchronization-free regions into transactions, and exploits the conflict detection mechanism of HTM for lightweight data race detection at runtime. However, the limitations of the current best-effort commodity HTMs expose several challenges in using them for data race detection: (1) lack of ability to pinpoint racy instructions, (2) false positives caused by cache line granularity of conflict detection, and (3) transactional aborts for non-conflict reasons (e.g., capacity or unknown). To overcome these challenges, TxRace performs lightweight HTM-based data race detection at first, and occasionally switches to slow yet precise data race detection only for the small fraction of execution intervals in which potential races are reported by HTM. According to the experimental results, TxRace reduces the average runtime overhead of dynamic data race detection from 11.68x to 4.65x with only a small number of false negatives.

---
### CoGENT: Verifying High-Assurance File System Implementations.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872404
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872404?download=true
* **Key Words**: Software and its engineering, Software notations and tools, General programming languages, Software organization and properties, Software functional properties, Formal methods, Software verification, 
* **Abstract**: We present an approach to writing and formally verifying high-assurance file-system code in a restricted language called Cogent, supported by a certifying compiler that produces C code, high-level specification of Cogent, and translation correctness proofs. The language is strongly typed and guarantees absence of a number of common file system implementation errors. We show how verification effort is drastically reduced for proving higher-level properties of the file system implementation by reasoning about the generated formal specification rather than its low-level C code. We use the framework to write two Linux file systems, and compare their performance with their native C implementations.

---
### M3: A Hardware/Operating-System Co-Design to Tame Heterogeneous Manycores.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872371
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872371?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, Security and privacy, Security services, Access control, Software and its engineering, Software organization and properties, Software system structures, Distributed systems organizing principles, 
* **Abstract**: In the last decade, the number of available cores increased and heterogeneity grew. In this work, we ask the question whether the design of the current operating systems (OSes) is still appropriate if these trends continue and lead to abundantly available but heterogeneous cores, or whether it forces a fundamental rethinking of how systems are designed. We argue that: 1. hiding heterogeneity behind a common hardware interface unifies, to a large extent, the control and coordination of cores and accelerators in the OS, 2. isolating at the network-on-chip rather than with processor features (like privileged mode, memory management unit, ...), allows running untrusted code on arbitrary cores, and 3. providing OS services via protocols over the network-on-chip, instead of via system calls, makes them accessible to arbitrary types of cores as well.

---
### Sidewinder: An Energy Efficient and Developer Friendly Heterogeneous Architecture for Continuous Mobile Sensing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872398
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872398?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, 
* **Abstract**: Applications that perform continuous sensing on mobile phones have the potential to revolutionize everyday life. Examples range from medical and health monitoring applications, such as pedometers and fall detectors, to participatory sensing applications, such as noise pollution, traffic and seismic activity monitoring. Unfortunately, current mobile devices are a poor match for continuous sensing applications as they require the device to remain awake for extended periods of time, resulting in poor battery life. This paper presents Sidewinder, a new approach towards offloading sensor data processing to a low-power processor and waking up the main processor when events of interest occur. This approach differs from other heterogeneous architectures in that developers are presented with a programming interface that lets them construct application specific wake-up conditions by linking together and parameterizing predefined sensor data processing algorithms. Our experiments indicate performance that is comparable to approaches that provide fully programmable offloading, but do so with a much simpler programming interface that facilitates deployment and portability.

---
### OpenPiton: An Open Source Manycore Research Framework.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872414
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872414?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, 
* **Abstract**: Industry is building larger, more complex, manycore processors on the back of strong institutional knowledge, but academic projects face difficulties in replicating that scale. To alleviate these difficulties and to develop and share knowledge, the community needs open architecture frameworks for simulation, synthesis, and software exploration which support extensibility, scalability, and configurability, alongside an established base of verification tools and supported software. In this paper we present OpenPiton, an open source framework for building scalable architecture research prototypes from 1 core to 500 million cores. OpenPiton is the world's first open source, general-purpose, multithreaded manycore processor and framework. OpenPiton leverages the industry hardened OpenSPARC T1 core with modifications and builds upon it with a scratch-built, scalable uncore creating a flexible, modern manycore design. In addition, OpenPiton provides synthesis and backend scripts for ASIC and FPGA to enable other researchers to bring their designs to implementation. OpenPiton provides a complete verification infrastructure of over 8000 tests, is supported by mature software tools, runs full-stack multiuser Debian Linux, and is written in industry standard Verilog. Multiple implementations of OpenPiton have been created including a taped-out 25-core implementation in IBM's 32nm process and multiple Xilinx FPGA prototypes.

---
### COATCheck: Verifying Memory Ordering at the Hardware-OS Interface.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872399
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872399?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Hardware, Hardware validation, Functional verification, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Memory management, Virtual memory, 
* **Abstract**: Modern computer systems include numerous compute elements, from CPUs to GPUs to accelerators. Harnessing their full potential requires well-defined, properly-implemented memory consistency models (MCMs), and low-level system functionality such as virtual memory and address translation (AT). Unfortunately, it is difficult to specify and implement hardware-OS interactions correctly; in the past, many hardware and OS specification mismatches have resulted in implementation bugs in commercial processors. In an effort to resolve this verification gap, this paper makes the following contributions. First, we present COATCheck, an address translation-aware framework for specifying and statically verifying memory ordering enforcement at the microarchitecture and operating system levels. We develop a domain-specific language for specifying ordering enforcement, for including ordering-related OS events and hardware micro-operations, and for programmatically enumerating happens-before graphs. Using a fast and automated static constraint solver, COATCheck can efficiently analyze interesting and important memory ordering scenarios for modern, high-performance, out-of-order processors. Second, we show that previous work on Virtual Address Memory Consistency (VAMC) does not capture every translation-related ordering scenario of interest, and that some such cases even fall outside the traditional scope of consistency. We therefore introduce the term transistency model to describe the superset of consistency which captures all translation-aware sets of ordering rules.


---
### True IOMMU Protection from DMA Attacks: When Copy is Faster than Zero Copy.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872379
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872379?download=true
* **Key Words**: Security and privacy, Systems security, Operating systems security, 
* **Abstract**: Malicious I/O devices might compromise the OS using DMAs. The OS therefore utilizes the IOMMU to map and unmap every target buffer right before and after its DMA is processed, thereby restricting DMAs to their designated locations. This usage model, however, is not truly secure for two reasons: (1) it provides protection at page granularity only, whereas DMA buffers can reside on the same page as other data; and (2) it delays DMA buffer unmaps due to performance considerations, creating a vulnerability window in which devices can access in-use memory. We propose that OSes utilize the IOMMU differently, in a manner that eliminates these two flaws. Our new usage model restricts device access to a set of shadow DMA buffers that are never unmapped, and it copies DMAed data to/from these buffers, thus providing sub-page protection while eliminating the aforementioned vulnerability window. Our key insight is that the cost of interacting with, and synchronizing access to the slow IOMMU hardware---required for zero-copy protection against devices---make copying preferable to zero-copying.

---
### Silent Shredder: Zero-Cost Shredding for Secure Non-Volatile Main Memory Controllers.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872377
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872377?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, 
* **Abstract**: As non-volatile memory (NVM) technologies are expected to replace DRAM in the near future, new challenges have emerged. For example, NVMs have slow and power-consuming writes, and limited write endurance. In addition, NVMs have a data remanence vulnerability, i.e., they retain data for a long time after being powered off. NVM encryption alleviates the vulnerability, but exacerbates the limited endurance by increasing the number of writes to memory. We observe that, in current systems, a large percentage of main memory writes result from data shredding in operating systems, a process of zeroing out physical pages before mapping them to new processes, in order to protect previous processes' data. In this paper, we propose Silent Shredder, which repurposes initialization vectors used in standard counter mode encryption to completely eliminate the data shredding writes. Silent Shredder also speeds up reading shredded cache lines, and hence reduces power consumption and improves overall performance. To evaluate our design, we run three PowerGraph applications and 26 multi-programmed workloads from the SPEC 2006 suite, on a gem5-based full system simulator. Silent Shredder eliminates an average of 48.6% of the writes in the initialization and graph construction phases. It speeds up main memory reads by 3.3 times, and improves the number of instructions per cycle (IPC) by 6.4% on average. Finally, we discuss several use cases, including virtual machines' data isolation and user-level large data initialization, where Silent Shredder can be used effectively at no extra cost.

---
### Sego: Pervasive Trusted Metadata for Efficiently Verified Untrusted System Services.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872372
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872372?download=true
* **Key Words**: Security and privacy, Systems security, Operating systems security, Virtualization and security, Social and professional topics, Professional topics, Management of computing and information systems, File systems management, 
* **Abstract**: Sego is a hypervisor-based system that gives strong privacy and integrity guarantees to trusted applications, even when the guest operating system is compromised or hostile. Sego verifies operating system services, like the file system, instead of replacing them. By associating trusted metadata with user data across all system devices, Sego verifies system services more efficiently than previous systems, especially services that depend on data contents. We extensively evaluate Sego's performance on real workloads and implement a kernel fault injector to validate Sego's file system-agnostic crash consistency and recovery protocol.

---
### Synopsis of the ASPLOS '16 Wild and Crazy Ideas (WACI) Invited-Speakers Session.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2876512
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2876512?download=true
* **Key Words**: Hardware, Software and its engineering, Software notations and tools, General programming languages, Software organization and properties, Contextual software domains, Operating systems, 
* **Abstract**: The Wild and Crazy Ideas (WACI) session is a longstanding tradition at ASPLOS, soliciting talks that consist of forward-looking, visionary, inspiring, creative, far out or just plain amazing ideas presented in an exciting way. (Amusing elements in the presentations are tolerated ;-) but are in fact optional.)

---
### Brain Inspired Computing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872417
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872417?download=true
* **Key Words**: Hardware, 
* **Abstract**: No abstract available.

---
### Scaling up Superoptimization.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872387
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872387?download=true
* **Key Words**: Software and its engineering, Software creation and management, Software development techniques, Automatic programming, Software notations and tools, Compilers, 
* **Abstract**: Developing a code optimizer is challenging, especially for new, idiosyncratic ISAs. Superoptimization can, in principle, discover machine-specific optimizations automatically by searching the space of all instruction sequences. If we can increase the size of code fragments a superoptimizer can optimize, we will be able to discover more optimizations. We develop LENS, a search algorithm that increases the size of code a superoptimizer can synthesize by rapidly pruning away invalid candidate programs. Pruning is achieved by selectively refining the abstraction under which candidates are considered equivalent, only in the promising part of the candidate space. LENS also uses a bidirectional search strategy to prune the candidate space from both forward and backward directions. These pruning strategies allow LENS to solve twice as many benchmarks as existing enumerative search algorithms, while LENS is about 11-times faster.

---
### Lifting Assembly to Intermediate Representation: A Novel Approach Leveraging Compilers.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872380
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872380?download=true
* **Key Words**: Software and its engineering, Software notations and tools, Compilers, System description languages, Architecture description languages, Theory of computation, Formal languages and automata theory, Automata extensions, Transducers, Tree languages, Semantics and reasoning, Program reasoning, Program analysis, Theory and algorithms for application domains, Machine learning theory, 
* **Abstract**: Translating low-level machine instructions into higher-level intermediate language (IL) is one of the central steps in many binary analysis and instrumentation systems. Existing systems build such translators manually. As a result, it takes a great deal of effort to support new architectures. Even for widely deployed architectures, full instruction sets may not be modeled, e.g., mature systems such as Valgrind still lack support for AVX, FMA4 and SSE4.1 for x86 processors. To overcome these difficulties, we propose a novel approach that leverages knowledge about instruction set semantics that is already embedded into modern compilers such as GCC. In particular, we present a learning-based approach for automating the translation of assembly instructions to a compiler's architecture-neutral IL. We present an experimental evaluation that demonstrates the ability of our approach to easily support many architectures (x86, ARM and AVR), including their advanced instruction sets. Our implementation is available as open-source software.

---
### Architecture-Adaptive Code Variant Tuning.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872411
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872411?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Computing methodologies, Machine learning, Learning paradigms, Multi-task learning, Supervised learning, Machine learning algorithms, Feature selection, General and reference, Cross-computing tools and techniques, Performance, Software and its engineering, Software organization and properties, Extra-functional properties, Software performance, 
* **Abstract**: Code variants represent alternative implementations of a computation, and are common in high-performance libraries and applications to facilitate selecting the most appropriate implementation for a specific execution context (target architecture and input dataset). Automating code variant selection typically relies on machine learning to construct a model during an offline learning phase that can be quickly queried at runtime once the execution context is known. In this paper, we define a new approach called architecture-adaptive code variant tuning, where the variant selection model is learned on a set of source architectures, and then used to predict variants on a new target architecture without having to repeat the training process. We pose this as a multi-task learning problem, where each source architecture corresponds to a task; we use device features in the construction of the variant selection model. This work explores the effectiveness of multi-task learning and the impact of different strategies for device feature selection. We evaluate our approach on a set of benchmarks and a collection of six NVIDIA GPU architectures from three distinct generations. We achieve performance results that are mostly comparable to the previous approach of tuning for a single GPU architecture without having to repeat the learning phase.

---
### Scalable Kernel TCP Design and Implementation for Short-Lived Connections.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872391
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2980024.2872391?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Networks, Network performance evaluation, Network performance analysis, 
* **Abstract**: With the rapid growth of network bandwidth, increases in CPU cores on a single machine, and application API models demanding more short-lived connections, a scalable TCP stack is performance-critical. Although many clean-state designs have been proposed, production environments still call for a bottom-up parallel TCP stack design that is backward-compatible with existing applications.

---
### SpaceJMP: Programming with Multiple Virtual Address Spaces.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872366
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2980024.2872366?download=true
* **Key Words**: Software and its engineering, Software notations and tools, Compilers, Software organization and properties, Contextual software domains, Operating systems, Memory management, Virtual memory, Process management, Process synchronization, 
* **Abstract**: Memory-centric computing demands careful organization of the virtual address space, but traditional methods for doing so are inflexible and inefficient. If an application wishes to address larger physical memory than virtual address bits allow, if it wishes to maintain pointer-based data structures beyond process lifetimes, or if it wishes to share large amounts of memory across simultaneously executing processes, legacy interfaces for managing the address space are cumbersome and often incur excessive overheads. We propose a new operating system design that promotes virtual address spaces to first-class citizens, enabling process threads to attach to, detach from, and switch between multiple virtual address spaces. Our work enables data-centric applications to utilize vast physical memory beyond the virtual range, represent persistent pointer-rich data structures without special pointer representations, and share large amounts of memory between processes efficiently.

---
### memif: Towards Programming Heterogeneous Memory Asynchronously.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872401
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2980024.2872401?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, 
* **Abstract**: To harness a heterogeneous memory hierarchy, it is advantageous to integrate application knowledge in guiding frequent memory move, i.e., replicating or migrating virtual memory regions. To this end, we present memif, a protected OS service for asynchronous, hardware-accelerated memory move. Compared to the state of the art -- page migration in Linux, memif incurs low overhead and low latency; in order to do so, it not only redefines the semantics of kernel interface but also overhauls the underlying mechanisms, including request/completion management, race handling, and DMA engine configuration. We implement memif in Linux for a server-class system-on-chip that features heterogeneous memories. Compared to the current Linux page migration, memif reduces CPU usage by up to 15% for small pages and by up to 38x for large pages; in continuously serving requests, memif has no need for request batching and reduces latency by up to 63%. By crafting a small runtime atop memif, we improve the throughputs for a set of streaming workloads by up to 33%. Overall, memif has opened the door to software management of heterogeneous memory.

---
### NVWAL: Exploiting NVRAM in Write-Ahead Logging.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872392
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872392?download=true
* **Key Words**: Hardware, Integrated circuits, Semiconductor memory, Non-volatile memory, Information systems, Data management systems, Database management system engines, Database transaction processing, Database recovery, 
* **Abstract**: Emerging byte-addressable non-volatile memory is considered an alternative storage device for database logs that require persistency and high performance. In this work, we develop NVWAL (NVRAM Write-Ahead Logging) for SQLite. The contribution of NVWAL consists of three elements: (i) byte-granularity differential logging that effectively eliminates the excessive I/O overhead of filesystem-based logging or journaling, (ii) transaction-aware lazy synchronization that reduces cache synchronization overhead by two-thirds, and (iii) user-level heap management of the NVRAM persistent WAL structure, which reduces the overhead of managing persistent objects.

---
### High-Performance Transactions for Persistent Memories.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872381
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872381?download=true
* **Key Words**: Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Memory management, Main memory, 
* **Abstract**: Emerging non-volatile memory (NVRAM) technologies offer the durability of disk with the byte-addressability of DRAM. These devices will allow software to access persistent data structures directly in NVRAM using processor loads and stores, however, ensuring consistency of persistent data across power failures and crashes is difficult. Atomic, durable transactions are a widely used abstraction to enforce such consistency. Implementing transactions on NVRAM requires the ability to constrain the order of NVRAM writes, for example, to ensure that a transaction's log record is complete before it is marked committed. Since NVRAM write latencies are expected to be high, minimizing these ordering constraints is critical for achieving high performance. Recent work has proposed programming interfaces to express NVRAM write ordering constraints to hardware so that NVRAM writes may be coalesced and reordered while preserving necessary constraints. Unfortunately, a straightforward implementation of transactions under these interfaces imposes unnecessary constraints. We show how to remove these dependencies through a variety of techniques, notably, deferring commit until after locks are released. We present a comprehensive analysis contrasting two transaction designs across three NVRAM programming interfaces, demonstrating up to 2.5x speedup.

---
### High-Density Image Storage Using Approximate Memory Cells.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872413
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872413?download=true
* **Key Words**: Computer systems organization, Dependable and fault-tolerant systems and networks, Reliability, Computing methodologies, Computer graphics, Image compression, Hardware, Emerging technologies, Memory and dense storage, 
* **Abstract**: This paper proposes tailoring image encoding for an approximate storage substrate. We demonstrate that indiscriminately storing encoded images in approximate memory generates unacceptable and uncontrollable quality degradation. The key finding is that errors in the encoded bit streams have non-uniform impact on the decoded image quality. We develop a methodology to determine the relative importance of encoded bits and store them in an approximate storage substrate. The storage cells are optimized to reduce error rate via biasing and are tuned to meet the desired reliability requirement via selective error correction. In a case study with the progressive transform codec (PTC), a precursor to JPEG XR, the proposed approximate image storage system exhibits a 2.7x increase in density of pixels per silicon volume under bounded error rates, and this achievement is additive to the storage savings of PTC compression.

---
### Failure-Atomic Persistent Memory Updates via JUSTDO Logging.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872410
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872410?download=true
* **Key Words**: Computer systems organization, Dependable and fault-tolerant systems and networks, Reliability, 
* **Abstract**: Persistent memory invites applications to manipulate persistent data via load and store instructions. Because failures during updates may destroy transient data (e.g., in CPU registers), preserving data integrity in the presence of failures requires failure-atomic bundles of updates. Prior failure atomicity approaches for persistent memory entail overheads due to logging and CPU cache flushing. Persistent caches can eliminate the need for flushing, but conventional logging remains complex and memory intensive. We present the design and implementation of JUSTDO logging, a new failure atomicity mechanism that greatly reduces the memory footprint of logs, simplifies log management, and enables fast parallel recovery following failure. Crash-injection tests confirm that JUSTDO logging preserves application data integrity and performance evaluations show that it improves throughput 3x or more compared with a state-of-the-art alternative for a spectrum of data-intensive algorithms.

---
### Interference Management for Distributed Parallel Applications in Consolidated Clusters.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872388
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872388?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Networks, Network services, Cloud computing, 
* **Abstract**: Consolidating multiple applications on a system can improve the overall resource utilization of data center systems. However, such consolidation can adversely affect the performance of some applications due to interference caused by resource contention. Despite many prior studies on the interference effects in single-node systems, the interference behaviors of distributed parallel applications have not been investigated thoroughly. With distributed applications, a local interference in a node can affect the whole execution of an application spanning many nodes. This paper studies an interference modeling methodology for distributed applications to predict their performance under interference effects in consolidated clusters. This study first characterizes the effects of interference for various distributed applications over different interference settings, and analyzes how diverse interference intensities on multiple nodes affect the overall performance. Based on the characterization, this study proposes a static profiling-based model for interference propagation and heterogeneity behaviors. In addition, this paper presents use case studies of the modeling method, two interference-aware placement techniques for consolidated virtual clusters, which attempt to maximize the overall throughput or to guarantee the quality-of-service.

---
### Taurus: A Holistic Language Runtime System for Coordinating Distributed Managed-Language Applications.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872386
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872386?download=true
* **Key Words**: Networks, Network services, Cloud computing, Software and its engineering, Software notations and tools, Compilers, Runtime environments, Software organization and properties, Contextual software domains, Operating systems, Memory management, Garbage collection, Process management, Scheduling, Software infrastructure, Virtual machines, 
* **Abstract**: Many distributed workloads in today's data centers are written in managed languages such as Java or Ruby. Examples include big data frameworks such as Hadoop, data stores such as Cassandra or applications such as the SOLR search engine. These workloads typically run across many independent language runtime systems on different nodes. This setup represents a source of inefficiency, as these language runtime systems are unaware of each other. For example, they may perform Garbage Collection at times that are locally reasonable but not in a distributed setting.

---
### HCloud: Resource-Efficient Provisioning in Shared Cloud Systems.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872365
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872365?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, Networks, Network services, Cloud computing, 
* **Abstract**: Cloud computing promises flexibility and high performance for users and cost efficiency for operators. To achieve this, cloud providers offer instances of different sizes, both as long-term reservations and short-term, on-demand allocations. Unfortunately, determining the best provisioning strategy is a complex, multi-dimensional problem that depends on the load fluctuation and duration of incoming jobs, and the performance unpredictability and cost of resources. We first compare the two main provisioning strategies (reserved and on-demand resources) on Google Compute Engine (GCE) using three representative workload scenarios with batch and latency-critical applications. We show that either approach is suboptimal for performance or cost. We then present HCloud, a hybrid provisioning system that uses both reserved and on-demand resources. HCloud determines which jobs should be mapped to reserved versus on-demand resources based on overall load, and resource unpredictability. It also determines the optimal instance size an application needs to satisfy its Quality of Service (QoS) constraints. We demonstrate that hybrid configurations improve performance by 2.1x compared to fully on-demand provisioning, and reduce cost by 46% compared to fully reserved systems. We also show that hybrid strategies are robust to variation in system and job parameters, such as cost and system load.

---
### CloudSeer: Workflow Monitoring of Cloud Infrastructures via Interleaved Logs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872407
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872407?download=true
* **Key Words**: Networks, Network services, Cloud computing, Software and its engineering, Software creation and management, Software verification and validation, Operational analysis, Software defect analysis, Software testing and debugging, Software organization and properties, Extra-functional properties, Software performance, Software reliability, 
* **Abstract**: Cloud infrastructures provide a rich set of management tasks that operate computing, storage, and networking resources in the cloud. Monitoring the executions of these tasks is crucial for cloud providers to promptly find and understand problems that compromise cloud availability. However, such monitoring is challenging because there are multiple distributed service components involved in the executions. CloudSeer enables effective workflow monitoring. It takes a lightweight non-intrusive approach that purely works on interleaved logs widely existing in cloud infrastructures. CloudSeer first builds an automaton for the workflow of each management task based on normal executions, and then it checks log messages against a set of automata for workflow divergences in a streaming manner. Divergences found during the checking process indicate potential execution problems, which may or may not be accompanied by error log messages. For each potential problem, CloudSeer outputs necessary context information including the affected task automaton and related log messages hinting where the problem occurs to help further diagnosis. Our experiments on OpenStack, a popular open-source cloud infrastructure, show that CloudSeer's efficiency and problem-detection capability are suitable for online monitoring.

---
### LDX: Causality Inference by Lightweight Dual Execution.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872395
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872395?download=true
* **Key Words**: Security and privacy, Systems security, Information flow control, Software and its engineering, Software notations and tools, Compilers, Runtime environments, Source code generation, 
* **Abstract**: Causality inference, such as dynamic taint anslysis, has many applications (e.g., information leak detection). It determines whether an event e is causally dependent on a preceding event c during execution. We develop a new causality inference engine LDX. Given an execution, it spawns a slave execution, in which it mutates c and observes whether any change is induced at e. To preclude non-determinism, LDX couples the executions by sharing syscall outcomes. To handle path differences induced by the perturbation, we develop a novel on-the-fly execution alignment scheme that maintains a counter to reflect the progress of execution. The scheme relies on program analysis and compiler transformation. LDX can effectively detect information leak and security attacks with an average overhead of 6.08% while running the master and the slave concurrently on separate CPUs, much lower than existing systems that require instruction level monitoring. Furthermore, it has much better accuracy in causality inference.

---
### TaxDC: A Taxonomy of Non-Deterministic Concurrency Bugs in Datacenter Distributed Systems.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872374
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872374?download=true
* **Key Words**: Networks, Network services, Cloud computing, Software and its engineering, Software creation and management, Software verification and validation, Software defect analysis, Software testing and debugging, 
* **Abstract**: We present TaxDC, the largest and most comprehensive taxonomy of non-deterministic concurrency bugs in distributed systems. We study 104 distributed concurrency (DC) bugs from four widely-deployed cloud-scale datacenter distributed systems, Cassandra, Hadoop MapReduce, HBase and ZooKeeper. We study DC-bug characteristics along several axes of analysis such as the triggering timing condition and input preconditions, error and failure symptoms, and fix strategies, collectively stored as 2,083 classification labels in TaxDC database. We discuss how our study can open up many new research directions in combating DC bugs.

---
### RID: Finding Reference Count Bugs with Inconsistent Path Pair Checking.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872389
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872389?download=true
* **Key Words**: Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Process management, Power management, Software functional properties, Formal methods, Automated static analysis, 
* **Abstract**: Reference counts are widely used in OS kernels for resource management. However, reference counts are not trivial to be used correctly in large scale programs because it is left to developers to make sure that an increment to a reference count is always paired with a decrement. This paper proposes inconsistent path pair checking, a novel technique that can statically discover bugs related to reference counts without knowing how reference counts should be changed in a function. A prototype called RID is implemented and evaluations show that RID can discover more than 80 bugs which were confirmed by the developers in the latest Linux kernel. The results also show that RID tends to reveal bugs caused by developers' misunderstanding on API specifications or error conditions that are not handled properly.

---
### Maximizing Performance Under a Power Cap: A Comparison of Hardware, Software, and Hybrid Techniques.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872375
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872375?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Reconfigurable computing, Real-time systems, Real-time system architecture, Hardware, Power and energy, Power estimation and optimization, 
* **Abstract**: Power and thermal dissipation constrain multicore performance scaling. Modern processors are built such that they could sustain damaging levels of power dissipation, creating a need for systems that can implement processor power caps. A particular challenge is developing systems that can maximize performance within a power cap, and approaches have been proposed in both software and hardware. Software approaches are flexible, allowing multiple hardware resources to be coordinated for maximum performance, but software is slow, requiring a long time to converge to the power target. In contrast, hardware power capping quickly converges to the the power cap, but only manages voltage and frequency, limiting its potential performance. In this work we propose PUPiL, a hybrid software/hardware power capping system. Unlike previous approaches, PUPiL combines hardware's fast reaction time with software's flexibility. We implement PUPiL on real Linux/x86 platform and compare it to Intel's commercial hardware power capping system for both single and multi-application workloads. We find PUPiL provides the same reaction time as Intel's hardware with significantly higher performance. On average, PUPiL outperforms hardware by from 1:18-2:4 depending on workload and power target. Thus, PUPiL provides a promising way to enforce power caps with greater performance than current state-of-the-art hardware-only approaches.

---
### The Computational Sprinting Game.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872383
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872383?download=true
* **Key Words**: Hardware, Power and energy, Power estimation and optimization, Enterprise level and data centers power issues, Theory of computation, Theory and algorithms for application domains, Algorithmic game theory and mechanism design, 
* **Abstract**: Computational sprinting is a class of mechanisms that boost performance but dissipate additional power. We describe a sprinting architecture in which many, independent chip multiprocessors share a power supply and sprints are constrained by the chips' thermal limits and the rack's power limits. Moreover, we present the computational sprinting game, a multi-agent perspective on managing sprints. Strategic agents decide whether to sprint based on application phases and system conditions. The game produces an equilibrium that improves task throughput for data analytics workloads by 4-6× over prior greedy heuristics and performs within 90% of an upper bound on throughput from a globally optimized policy.

---
### An Energy-interference-free Hardware-Software Debugger for Intermittent Energy-harvesting Systems.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872409
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872409?download=true
* **Key Words**: Computer systems organization, Embedded and cyber-physical systems, Embedded systems, Embedded software, Hardware, Emerging technologies, Analysis and design of emerging devices and systems, Software and its engineering, Software organization and properties, Extra-functional properties, Software reliability, Software functional properties, Correctness, Consistency, 
* **Abstract**: Energy-autonomous computing devices have the potential to extend the reach of computing to a scale beyond either wired or battery-powered systems. However, these devices pose a unique set of challenges to application developers who lack both hardware and software support tools. Energy harvesting devices experience power intermittence which causes the system to reset and power-cycle unpredictably, tens to hundreds of times per second. This can result in code execution errors that are not possible in continuously-powered systems and cannot be diagnosed with conventional debugging tools such as JTAG and/or oscilloscopes. We propose the Energy-interference-free Debugger, a hardware and software platform for monitoring and debugging intermittent systems without adversely effecting their energy state. The Energy-interference-free Debugger re-creates a familiar debugging environment for intermittent software and augments it with debugging primitives for effective diagnosis of intermittence bugs. Our evaluation of the Energy-interference-free Debugger quantifies its energy-interference-freedom and shows its value in a set of debugging tasks in complex test programs and several real applications, including RFID code and a machine-learning-based activity recognition system.

---
### Programmer Productivity in a World of Mushy Interfaces: Challenges of the Post-ISA Reality.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2876511
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2876511?download=true
* **Key Words**: Computer systems organization, Software and its engineering, Software notations and tools, General programming languages, Software organization and properties, Contextual software domains, Operating systems, 
* **Abstract**: Since 1964, we had the notion that the instruction set architecture (ISA) is a useful and fairly opaque abstraction layer between hardware and software. Software rode hardware's performance wave while remaining gloriously oblivious to hardware's growing complexity. Unfortunately, the jig is up. We still have ISAs, but the abstraction no longer offers seamless portability---parallel software needs to be tuned for different core counts, and heterogeneous processing elements (CPUs, GPUs, accelerators) further complicate programmability. We are better at building large-scale heterogeneous processors than we are at programming them. Maintaining software across multiple current platforms is difficult and porting to future platforms is also difficult. There have been many technical responses: virtual ISAs (e.g., NVIDIA's PTX), higher-level programming interfaces (e.g., CUDA or OpenCL), and late-stage compilation and platform-specific tailoring (e.g., Android ART), etc.

---
### RAPID Programming of Pattern-Recognition Processors.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872393
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872393?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, Computing methodologies, Parallel computing methodologies, Parallel programming languages, Software and its engineering, Software notations and tools, Compilers, General programming languages, Language features, Concurrent programming structures, Patterns, 
* **Abstract**: We present RAPID, a high-level programming language and combined imperative and declarative model for programming pattern-recognition processors, such as Micron's Automata Processor (AP). The AP is a novel, non-Von Neumann architecture for direct execution of non-deterministic finite automata (NFAs), and has been demonstrated to provide substantial speedup for a variety of data-processing applications. RAPID is clear, maintainable, concise, and efficient both at compile and run time. Language features, such as code abstraction and parallel control structures, map well to pattern-matching problems, providing clarity and maintainability. For generation of efficient runtime code, we present algorithms to convert RAPID programs into finite automata. Further, we introduce a tessellation technique for configuring the AP, which significantly reduces compile time, increases programmer productivity, and improves maintainability. We evaluate five RAPID programs against custom, baseline implementations previously demonstrated to be significantly accelerated by the AP. We find that RAPID programs are much shorter in length, are expressible at a higher level of abstraction than their handcrafted counterparts, and yield generated code that is often more compact. In addition, our tessellation technique for configuring the AP has comparable device utilization to, and results in compilation that is up to four orders of magnitude faster than, current solutions.

---
### Proactive Control of Approximate Programs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872402
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872402?download=true
* **Key Words**: Computing methodologies, Artificial intelligence, Control methods, Software and its engineering, Software organization and properties, Extra-functional properties, Software functional properties, Correctness, Theory of computation, Design and analysis of algorithms, Approximation algorithms analysis, 
* **Abstract**: Approximate computing trades off accuracy of results for resources such as energy or computing time. There is a large and rapidly growing literature on approximate computing that has focused mostly on showing the benefits of approximate computing. However, we know relatively little about how to control approximation in a disciplined way. In this paper, we address the problem of controlling approximation for non-streaming programs that have a set of "knobs" that can be dialed up or down to control the level of approximation of different components in the program. We formulate this control problem as a constrained optimization problem, and describe a system called Capri that uses machine learning to learn cost and error models for the program, and uses these models to determine, for a desired level of approximation, knob settings that optimize metrics such as running time or energy usage. Experimental results with complex benchmarks from different problem domains demonstrate the effectiveness of this approach.

---
### AxGames: Towards Crowdsourcing Quality Target Determination in Approximate Computing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872376
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872376?download=true
* **Key Words**: Computer systems organization, Architectures, Human-centered computing, Human computer interaction (HCI), Interactive systems and tools, Software and its engineering, Software notations and tools, Development frameworks and environments, 
* **Abstract**: Approximate computing trades quality of application output for higher efficiency and performance. Approximation is useful only if its impact on application output quality is acceptable to the users. However, there is a lack of systematic solutions and studies that explore users' perspective on the effects of approximation. In this paper, we seek to provide one such solution for the developers to probe and discover the boundary of quality loss that most users will deem acceptable. We propose AxGames, a crowdsourced solution that enables developers to readily infer a statistical common ground from the general public through three entertaining games. The users engage in these games by betting on their opinion about the quality loss of the final output while the AxGames framework collects statistics about their perceptions. The framework then statistically analyzes the results to determine the acceptable levels of quality for a pair of (application, approximation technique). The three games are designed such that they effectively capture quality requirements with various tradeoffs and contexts. To evaluate AxGames, we examine seven diverse applications that produce user perceptible outputs and cover a wide range of domains, including image processing, optical character recognition, speech to text conversion, and audio processing. We recruit 700 participants/users through Amazon's Mechanical Turk to play the games that collect statistics about their perception on different levels of quality. Subsequently, the AxGames framework uses the Clopper-Pearson exact method, which computes a binomial proportion confidence interval, to analyze the collected statistics for each level of quality. Using this analysis, AxGames can statistically project the quality level that satisfies a given percentage of users. The developers can use these statistical projections to tune the level of approximation based on the user experience. We find that the level of acceptable quality loss significantly varies across applications. For instance, to satisfy 90% of users, the level of acceptable quality loss is 2% for one application (image processing) and 26% for another (audio processing). Moreover, the pattern with which the crowd responds to approximation takes significantly different shape and form depending on the class of applications. These results confirm the necessity of solutions that systematically explore the effect of approximation on the end user experience.

---
### A DNA-Based Archival Storage System.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872397
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872397?download=true
* **Key Words**: Hardware, Emerging technologies, Emerging interfaces, Memory and dense storage, Information systems, Information retrieval, Specialized information retrieval, Structure and multilingual text search, Chemical and biochemical retrieval, 
* **Abstract**: Demand for data storage is growing exponentially, but the capacity of existing storage media is not keeping up. Using DNA to archive data is an attractive possibility because it is extremely dense, with a raw limit of 1 exabyte/mm3 (109 GB/mm3), and long-lasting, with observed half-life of over 500 years. This paper presents an architecture for a DNA-based archival storage system. It is structured as a key-value store, and leverages common biochemical techniques to provide random access. We also propose a new encoding scheme that offers controllable redundancy, trading off reliability for density. We demonstrate feasibility, random access, and robustness of the proposed encoding with wet lab experiments involving 151 kB of synthesized DNA and a 42 kB random-access subset, and simulation experiments of larger sets calibrated to the wet lab experiments. Finally, we highlight trends in biotechnology that indicate the impending practicality of DNA storage for much larger datasets.

---
### Generating Configurable Hardware from Parallel Patterns.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872415
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2980024.2872415?download=true
* **Key Words**: Computing methodologies, Machine learning, Parallel computing methodologies, Parallel programming languages, Hardware, Electronic design automation, Hardware description languages and compilation, High-level and register-transfer level synthesis, Datapath optimization, Hardware-software codesign, Integrated circuits, Reconfigurable logic and FPGAs, Hardware accelerators, Software and its engineering, Software notations and tools, Compilers, Context specific languages, Domain specific languages, General programming languages, Language types, Functional languages, 
* **Abstract**: In recent years the computing landscape has seen an increasing shift towards specialized accelerators. Field programmable gate arrays (FPGAs) are particularly promising for the implementation of these accelerators, as they offer significant performance and energy improvements over CPUs for a wide class of applications and are far more flexible than fixed-function ASICs. However, FPGAs are difficult to program. Traditional programming models for reconfigurable logic use low-level hardware description languages like Verilog and VHDL, which have none of the productivity features of modern software languages but produce very efficient designs, and low-level software languages like C and OpenCL coupled with high-level synthesis (HLS) tools that typically produce designs that are far less efficient. Functional languages with parallel patterns are a better fit for hardware generation because they provide high-level abstractions to programmers with little experience in hardware design and avoid many of the problems faced when generating hardware from imperative languages. In this paper, we identify two important optimizations for using parallel patterns to generate efficient hardware: tiling and metapipelining. We present a general representation of tiled parallel patterns, and provide rules for automatically tiling patterns and generating metapipelines. We demonstrate experimentally that these optimizations result in speedups up to 39.4× on a set of benchmarks from the data analytics domain.

---
### DySel: Lightweight Dynamic Selection for Kernel-based Data-parallel Programming Model.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872373
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2980024.2872373?download=true
* **Key Words**: Software and its engineering, Software notations and tools, Compilers, Runtime environments, Source code generation, 
* **Abstract**: The rising pressure for simultaneously improving performance and reducing power is driving more diversity into all aspects of computing devices. An algorithm that is well-matched to the target hardware can run multiple times faster and more energy efficiently than one that is not. The problem is complicated by the fact that a program's input also affects the appropriate choice of algorithm. As a result, software developers have been faced with the challenge of determining the appropriate algorithm for each potential combination of target device and data. This paper presents DySel, a novel runtime system for automating such determination for kernel-based data parallel programming models such as OpenCL, CUDA, OpenACC, and C++AMP. These programming models cover many applications that demand high performance in mobile, cloud and high-performance computing. DySel systematically deploys candidate kernels on a small portion of the actual data to determine which achieves the best performance for the hardware-data combination. The test-deployment, referred to as micro-profiling, contributes to the final execution result and incurs less than 8% of overhead in the worst observed case when compared to an oracle. We show four major use cases where DySel provides significantly more consistent performance without tedious effort from the developer.

---
### Baymax: QoS Awareness and Increased Utilization for Non-Preemptive Accelerators in Warehouse Scale Computers.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872368
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2980024.2872368?download=true
* **Key Words**: Computer systems organization, Architectures, General and reference, Cross-computing tools and techniques, Performance, Hardware, Integrated circuits, Reconfigurable logic and FPGAs, Hardware accelerators, 
* **Abstract**: Modern warehouse-scale computers (WSCs) are being outfitted with accelerators to provide the significant compute required by emerging intelligent personal assistant (IPA) workloads such as voice recognition, image classification, and natural language processing. It is well known that the diurnal user access pattern of user-facing services provides a strong incentive to co-locate applications for better accelerator utilization and efficiency, and prior work has focused on enabling co-location on multicore processors. However, interference when co-locating applications on non-preemptive accelerators is fundamentally different than contention on multi-core CPUs and introduces a new set of challenges to reduce QoS violation. To address this open problem, we first identify the underlying causes for QoS violation in accelerator-outfitted servers. Our experiments show that queuing delay for the compute resources and PCI-e bandwidth contention for data transfer are the main two factors that contribute to the long tails of user-facing applications. We then present Baymax, a runtime system that orchestrates the execution of compute tasks from different applications and mitigates PCI-e bandwidth contention to deliver the required QoS for user-facing applications and increase the accelerator utilization. Using DjiNN, a deep neural network service, Sirius, an end-to-end IPA workload, and traditional applications on a Nvidia K40 GPU, our evaluation shows that Baymax improves the accelerator utilization by 91.3% while achieving the desired 99%-ile latency target for for user-facing applications. In fact, Baymax reduces the 99%-ile latency of user-facing applications by up to 195x over default execution.

---
### Analyzing Behavior Specialized Acceleration.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872412
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2980024.2872412?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, Computing methodologies, Modeling and simulation, Model development and analysis, Modeling methodologies, 
* **Abstract**: Hardware specialization has become a promising paradigm for overcoming the inefficiencies of general purpose microprocessors. Of significant interest are Behavioral Specialized Accelerators (BSAs), which are designed to efficiently execute code with only certain properties, but remain largely configurable or programmable. The most important strength of BSAs -- their ability to target a wide variety of codes -- also makes their interactions and analysis complex, raising the following questions: can multiple BSAs be composed synergistically, what are their interactions with the general purpose core, and what combinations favor which workloads? From a methodological standpoint, BSAs are also challenging, as they each require ISA development, compiler and assembler extensions, and either simulator or RTL models.

---
### PIFT: Predictive Information-Flow Tracking.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872403
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872403?download=true
* **Key Words**: Security and privacy, Systems security, Information flow control, 
* **Abstract**: Phones today carry sensitive information and have a great number of ways to communicate that data. As a result, malware that steal money, information, or simply disable functionality have hit the app stores. Current security solutions for preventing undesirable data leaks are mostly high-overhead and have not been practical enough for smartphones. In this paper, we show that simply monitoring just some instructions (only memory loads and stores) it is possible to achieve low overhead, highly accurate information flow tracking. Our method achieves 98% accuracy (0% false positive and 2% false negative) over DroidBench and was able to successfully catch seven real-world malware instances that steal phone number, location, and device ID using SMS messages and HTTP connections.

---
### HIPStR: Heterogeneous-ISA Program State Relocation.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872408
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872408?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, Security and privacy, Intrusion/anomaly detection and malware mitigation, Malware and its mitigation, 
* **Abstract**: Heterogeneous Chip Multiprocessors have been shown to provide significant performance and energy efficiency gains over homogeneous designs. Recent research has expanded the dimensions of heterogeneity to include diverse Instruction Set Architectures, called Heterogeneous-ISA Chip Multiprocessors. This work leverages such an architecture to realize substantial new security benefits, and in particular, to thwart Return-Oriented Programming. This paper proposes a novel security defense called HIPStR -- Heterogeneous-ISA Program State Relocation -- that performs dynamic randomization of run-time program state, both within and across ISAs. This technique outperforms the state-of-the-art just-in-time code reuse (JIT-ROP) defense by an average of 15.6%, while simultaneously providing greater security guarantees against classic return-into-libc, ROP, JOP, brute force, JIT-ROP, and several evasive variants.

---
### ANVIL: Software-Based Protection Against Next-Generation Rowhammer Attacks.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872390
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2872362.2872390?download=true
* **Key Words**: Computer systems organization, Dependable and fault-tolerant systems and networks, Reliability, General and reference, Cross-computing tools and techniques, Design, Experimentation, Document types, General conference proceedings, Hardware, Integrated circuits, Semiconductor memory, Dynamic memory, Robustness, Hardware reliability, Signal integrity and noise analysis, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Process management, Monitors, 
* **Abstract**: Ensuring the integrity and security of the memory system is critical. Recent studies have shown serious security concerns due to "rowhammer" attacks, where repeated accesses to a row of memory cause bit flips in adjacent rows. Recent work by Google's Project Zero has shown how to leverage rowhammer-induced bit-flips as the basis for security exploits that include malicious code injection and memory privilege escalation. Being an important security concern, industry has attempted to defend against rowhammer attacks. Deployed defenses employ two strategies: (1) doubling the system DRAM refresh rate and (2) restricting access to the CLFLUSH instruction that attackers use to bypass the cache to increase memory access frequency (i.e., the rate of rowhammering). We demonstrate that such defenses are inadequte: we implement rowhammer attacks that both avoid using the CLFLUSH instruction and cause bit flips with a doubled refresh rate. Our next-generation CLFLUSH-free rowhammer attack bypasses the cache by manipulating cache replacement state to allow frequent misses out of the last-level cache to DRAM rows of our choosing.

---
### ProteusTM: Abstraction Meets Performance in Transactional Memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872385
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872385?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Computing methodologies, Concurrent computing methodologies, Machine learning, Learning paradigms, Supervised learning, 
* **Abstract**: The Transactional Memory (TM) paradigm promises to greatly simplify the development of concurrent applications. This led, over the years, to the creation of a plethora of TM implementations delivering wide ranges of performance across workloads. Yet, no universal implementation fits each and every workload. In fact, the best TM in a given workload can reveal to be disastrous for another one. This forces developers to face the complex task of tuning TM implementations, which significantly hampers their wide adoption. In this paper, we address the challenge of automatically identifying the best TM implementation for a given workload. Our proposed system, ProteusTM, hides behind the TM interface a large library of implementations. Underneath, it leverages a novel multi-dimensional online optimization scheme, combining two popular learning techniques: Collaborative Filtering and Bayesian Optimization.

---
### CSR: Core Surprise Removal in Commodity Operating Systems.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872369
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872369?download=true
* **Key Words**: Computer systems organization, Dependable and fault-tolerant systems and networks, Reliability, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, 
* **Abstract**: One of the adverse effects of shrinking transistor sizes is that processors have become increasingly prone to hardware faults. At the same time, the number of cores per die rises. Consequently, core failures can no longer be ruled out, and future operating systems for many-core machines will have to incorporate fault tolerance mechanisms.

---
### CASPAR: Breaking Serialization in Lock-Free Multicore Synchronization.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/2872362.2872400
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/2954679.2872400?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Computing methodologies, Concurrent computing methodologies, Concurrent algorithms, 
* **Abstract**: In multicores, performance-critical synchronization is increasingly performed in a lock-free manner using atomic instructions such as CAS or LL/SC. However, when many processors synchronize on the same variable, performance can still degrade significantly. Contending writes get serialized, creating a non-scalable condition. Past proposals that build hardware queues of synchronizing processors do not fundamentally solve this problem---at best, they help to efficiently serialize the contending writes.
