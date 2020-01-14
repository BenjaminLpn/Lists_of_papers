### asplos 2017 | 58 papers.
---
### Big Data Analytics and Intelligence at Alibaba Cloud.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037699
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037699?download=true
* **Key Words**: 
* **Abstract**: No abstract available.

---
### Determining Application-specific Peak Power and Energy Requirements for Ultra-low Power Processors.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037711
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037711?download=true
* **Key Words**: 
* **Abstract**: Many emerging applications such as IoT, wearables, implantables, and sensor networks are power- and energy-constrained. These applications rely on ultra-low-power processors that have rapidly become the most abundant type of processor manufactured today. In the ultra-low-power embedded systems used by these applications, peak power and energy requirements are the primary factors that determine critical system characteristics, such as size, weight, cost, and lifetime. While the power and energy requirements of these systems tend to be application-specific, conventional techniques for rating peak power and energy cannot accurately bound the power and energy requirements of an application running on a processor, leading to over-provisioning that increases system size and weight. In this paper, we present an automated technique that performs hardware-software co-analysis of the application and ultra-low-power processor in an embedded system to determine application-specific peak power and energy requirements. Our technique provides more accurate, tighter bounds than conventional techniques for determining peak power and energy requirements, reporting 15% lower peak power and 17% lower peak energy, on average, than a conventional approach based on profiling and guardbanding. Compared to an aggressive stressmark-based approach, our technique reports power and energy bounds that are 26% and 26% lower, respectively, on average. Also, unlike conventional approaches, our technique reports guaranteed bounds on peak power and energy independent of an application's input set. Tighter bounds on peak power and energy can be exploited to reduce system size, weight, and cost.

---
### Prophet: Precise QoS Prediction on Non-Preemptive Accelerators to Improve Utilization in Warehouse-Scale Computers.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037700
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037700?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Real-time systems, General and reference, Cross-computing tools and techniques, Performance, 
* **Abstract**: Guaranteeing Quality-of-Service (QoS) of latency-sensitive applications while improving server utilization through application co-location is important yet challenging in modern datacenters. The key challenge is that when applications are co-located on a server, performance interference due to resource contention can be detrimental to the application QoS. Although prior work has proposed techniques to identify "safe" co-locations where application QoS is satisfied by predicting the performance interference on multicores, no such prediction technique on accelerators such as GPUs.

---
### Mallacc: Accelerating Memory Allocation.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037736
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037736?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Cloud computing, Other architectures, Special purpose systems, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Memory management, Allocation / deallocation strategies, 
* **Abstract**: Recent work shows that dynamic memory allocation consumes nearly 7% of all cycles in Google datacenters. With the trend towards increased specialization of hardware, we propose Mallacc, an in-core hardware accelerator designed for broad use across a number of high-performance, modern memory allocators. The design of Mallacc is quite different from traditional throughput-oriented hardware accelerators. Because memory allocation requests tend to be very frequent, fast, and interspersed inside other application code, accelerators must be optimized for latency rather than throughput and area overheads must be kept to a bare minimum. Mallacc accelerates the three primary operations of a typical memory allocation request: size class computation, retrieval of a free memory block, and sampling of memory usage. Our results show that malloc latency can be reduced by up to 50% with a hardware cost of less than 1500 um2 of silicon area, less than 0.006% of a typical high-performance processor core.

---
### REDSPY: Exploring Value Locality in Software.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037729
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037729?download=true
* **Key Words**: General and reference, Cross-computing tools and techniques, Performance, 
* **Abstract**: Complex code bases with several layers of abstractions have abundant inefficiencies that affect the execution time. Value redundancy is a kind of inefficiency where the same values are repeatedly computed, stored, or retrieved over the course of execution. Not all redundancies can be easily detected or eliminated with compiler optimization passes due to the inherent limitations of the static analysis.

---
### Translation-Triggered Prefetching.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037705
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037705?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Serial architectures, Pipeline computing, 
* **Abstract**: We propose translation-enabled memory prefetching optimizations or TEMPO, a low-overhead hardware mechanism to boost memory performance by exploiting the operating system's (OS) virtual memory subsystem. We are the first to make the following observations: (1) a substantial fraction (20-40%) of DRAM references in modern big- data workloads are devoted to accessing page tables; and (2) when memory references require page table lookups in DRAM, the vast majority of them (98%+) also look up DRAM for the subsequent data access. TEMPO exploits these observations to enable DRAM row-buffer and on-chip cache prefetching of the data that page tables point to. TEMPO requires trivial changes to the memory controller (under 3% additional area), no OS or application changes, and improves performance by 10-30% and energy by 1-14%.

---
### Typed Architectures: Architectural Support for Lightweight Scripting.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037726
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037726?download=true
* **Key Words**: Computer systems organization, Architectures, Serial architectures, Software and its engineering, Software notations and tools, Context specific languages, Scripting languages, 
* **Abstract**: Dynamic scripting languages are becoming more and more widely adopted not only for fast prototyping but also for developing production-grade applications. They provide high-productivity programming environments featuring high levels of abstraction with powerful built-in functions, automatic memory management, object-oriented programming paradigm and dynamic typing. However, their flexible, dynamic type systems easily become the source of inefficiency in terms of instruction count, memory footprint, and energy consumption. This overhead makes it challenging to deploy these high-productivity programming technologies on emerging single-board computers for IoT applications. Addressing this challenge, this paper introduces Typed Architectures, a high-efficiency, low-cost execution substrate for dynamic scripting languages, where each data variable retains high-level type information at an ISA level. Typed Architectures calculate and check the dynamic type of each variable implicitly in hardware, rather than explicitly in software, hence significantly reducing instruction count for dynamic type checking. Besides, Typed Architectures introduce polymorphic instructions (e.g., xadd), which are bound to the correct native instruction at runtime within the pipeline (e.g., add or fadd) to efficiently implement polymorphic operators. Finally, Typed Architectures provide hardware support for flexible yet efficient type tag extraction and insertion, capturing common data layout patterns of tag-value pairs. Our evaluation using a fully synthesizable RISC-V RTL design on FPGA shows that Typed Architectures achieve geomean speedups of 11.2% and 9.9% with maximum speedups of 32.6% and 43.5% for two production-grade scripting engines for JavaScript and Lua, respectively. Moreover, Typed Architectures improve the energy-delay product (EDP) by 19.3% for JavaScript and 16.5% for Lua with an area overhead of 1.6% at a 40nm technology node.

---
### Failure-Atomic Slotted Paging for Persistent Memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037737
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037737?download=true
* **Key Words**: Hardware, Integrated circuits, Semiconductor memory, Non-volatile memory, Information systems, Data management systems, Database management system engines, Database transaction processing, Database recovery, Transaction logging, Record and buffer management, 
* **Abstract**: The slotted-page structure is a database page format commonly used for managing variable-length records. In this work, we develop a novel "failure-atomic slotted page structure" for persistent memory that leverages byte addressability and durability of persistent memory to minimize redundant write operations used to maintain consistency in traditional database systems. Failure-atomic slotted paging consists of two key elements: (i) in-place commit per page using hardware transactional memory and (ii) slot header logging that logs the commit mark of each page. The proposed scheme is implemented in SQLite and compared against NVWAL, the current state-of-the-art scheme. Our performance study shows that our failure-atomic slotted paging shows optimal performance for database transactions that insert a single record. For transactions that touch more than one database page, our proposed slot-header logging scheme minimizes the logging overhead by avoiding duplicating pages and logging only the metadata of the dirty pages. Overall, we find that our failure-atomic slotted-page management scheme reduces database logging overhead to 1/6 and improves query response time by up to 33% compared to NVWAL.

---
### What Scalable Programs Need from Transactional Memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037750
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037750?download=true
* **Key Words**: Software and its engineering, Software notations and tools, Compilers, Runtime environments, General programming languages, Language types, Parallel programming languages, 
* **Abstract**: Transactional memory (TM) has been the focus of numerous studies, and it is supported in processors such as the IBM Blue Gene/Q and Intel Haswell. Many studies have used the STAMP benchmark suite to evaluate their designs. However, the speedups obtained for the STAMP benchmarks on all TM systems we know of are quite limited; for example, with 64 threads on the IBM Blue Gene/Q, we observe a median speedup of 1.4X using the Blue Gene/Q hardware transactional memory (HTM), and a median speedup of 4.1X using a software transactional memory (STM).

---
### TriCheck: Memory Model Verification at the Trisection of Software, Hardware, and ISA.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037719
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037719?download=true
* **Key Words**: General and reference, Cross-computing tools and techniques, Verification, Software and its engineering, Software organization and properties, Software functional properties, Correctness, Consistency, Formal methods, Software verification, 
* **Abstract**: Memory consistency models (MCMs) which govern inter-module interactions in a shared memory system, are a significant, yet often under-appreciated, aspect of system design. MCMs are defined at the various layers of the hardware-software stack, requiring thoroughly verified specifications, compilers, and implementations at the interfaces between layers. Current verification techniques evaluate segments of the system stack in isolation, such as proving compiler mappings from a high-level language (HLL) to an ISA or proving validity of a microarchitectural implementation of an ISA.

---
### An Analysis of Persistent Memory Use with WHISPER.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037730
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037730?download=true
* **Key Words**: Information systems, Information storage systems, Information storage technologies, Storage class memory, Phase change memory, 
* **Abstract**: Emerging non-volatile memory (NVM) technologies promise durability with read and write latencies comparable to volatile memory (DRAM). We define Persistent Memory (PM) as NVM accessed with byte addressability at low latency via normal memory instructions. Persistent-memory applications ensure the consistency of persistent data by inserting ordering points between writes to PM allowing the construction of higher-level transaction mechanisms. An epoch is a set of writes to PM between ordering points.

---
### ProRace: Practical Data Race Detection for Production Use.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037708
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037708?download=true
* **Key Words**: Software and its engineering, Software creation and management, Software verification and validation, Software defect analysis, Software testing and debugging, Software notations and tools, General programming languages, Language types, Concurrent programming languages, Software organization and properties, Contextual software domains, Operating systems, 
* **Abstract**: This paper presents ProRace, a dynamic data race detector practical for production runs. It is lightweight, but still offers high race detection capability. To track memory accesses, ProRace leverages instruction sampling using the performance monitoring unit (PMU) in commodity processors. Our PMU driver enables ProRace to sample more memory accesses at a lower cost compared to the state-of-the-art Linux driver. Moreover, ProRace uses PMU-provided execution contexts including register states and program path, and reconstructs unsampled memory accesses offline. This technique allows \ProRace to overcome inherent limitations of sampling and improve the detection coverage by performing data race detection on the trace with not only sampled but also reconstructed memory accesses. Experiments using racy production software including apache and mysql shows that, with a reasonable offline cost, ProRace incurs only 2.6% overhead at runtime with 27.5% detection probability with a sampling period of 10,000.

---
### Crossing Guard: Mediating Host-Accelerator Coherence Interactions.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037715
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037715?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, Hardware, Integrated circuits, Reconfigurable logic and FPGAs, Hardware accelerators, Robustness, 
* **Abstract**: Specialized hardware accelerators have performance and energy-efficiency advantages over general-purpose processors. To fully realize these benefits and aid programmability, accelerators may share a physical and virtual address space and full cache coherence with the host system. However, allowing accelerators -- particularly those designed by third parties -- to directly communicate with host coherence protocols poses several problems. Host coherence protocols are complex, vary between companies, and may be proprietary, increasing burden on accelerator designers. Bugs in the accelerator implementation may cause crashes and other serious consequences to the host system.

---
### An Architecture Supporting Formal and Compositional Binary Analysis.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037733
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037733?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, High-level language architectures, Real-time systems, Real-time system architecture, Hardware, Robustness, Safety critical systems, Software and its engineering, Software creation and management, Software verification and validation, Formal software verification, Software notations and tools, Formal language definitions, Semantics, General programming languages, Language types, Assembly languages, Functional languages, Software organization and properties, Software functional properties, Formal methods, Automated static analysis, Software verification, Theory of computation, Logic, Type theory, Verification by model checking, Semantics and reasoning, Program reasoning, Program analysis, Program verification, Program semantics, Operational semantics, 
* **Abstract**: Building a trustworthy life-critical embedded system requires deep reasoning about the potential effects that sequences of machine instructions can have on full system operation. Rather than trying to analyze complete binaries and the countless ways their instructions can interact with one another --- memory, side effects, control registers, implicit state, etc. --- we explore a new approach. We propose an architecture controlled by a thin computational layer designed to tightly correspond with the lambda calculus, drawing on principles of functional programming to bring the assembly much closer to myriad reasoning frameworks, such as the Coq proof assistant. This approach allows assembly-level verified versions of critical code to operate safely in tandem with arbitrary code, including imperative and unverified system components, without the need for large supporting trusted computing bases. We demonstrate that this computational layer can be built in such a way as to simultaneously provide full programmability and compact, precise, and complete semantics, while still using hardware resources comparable to normal embedded systems. To demonstrate the practicality of this approach, our FPGA-implemented prototype runs an embedded medical application which monitors and treats life-threatening arrhythmias. Though the system integrates untrusted and imperative components, our architecture allows for the formal verification of multiple properties of the end-to-end system, including a proof of correctness of the assembly-level implementation of the core algorithm, the integrity of trusted data via a non-interference proof, and a guarantee that our prototype meets critical timing requirements.

---
### AsyncClock: Scalable Inference of Asynchronous Event Causality.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037712
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037712?download=true
* **Key Words**: Software and its engineering, Software creation and management, Software verification and validation, Software defect analysis, Software testing and debugging, Theory of computation, Semantics and reasoning, Program reasoning, Program analysis, 
* **Abstract**: Asynchronous programming model is commonly used in mobile systems and Web 2.0 environments. Asynchronous race detectors use algorithms that are an order of magnitude performance and space inefficient compared to conventional data race detectors. We solve this problem by identifying and addressing two important problems in reasoning about causality between asynchronous events.

---
### Black-box Concurrent Data Structures for NUMA Architectures.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037721
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037721?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Software and its engineering, Software notations and tools, General programming languages, Language features, Concurrent programming structures, Software organization and properties, Contextual software domains, Operating systems, Communications management, Message passing, Process management, Concurrency control, Multithreading, Mutual exclusion, Process synchronization, Software functional properties, Correctness, Consistency, Synchronization, Theory of computation, Design and analysis of algorithms, Concurrent algorithms, Parallel algorithms, Shared memory algorithms, Models of computation, Concurrency, Distributed computing models, Parallel computing models, 
* **Abstract**: High-performance servers are Non-Uniform Memory Access (NUMA) machines. To fully leverage these machines, programmers need efficient concurrent data structures that are aware of the NUMA performance artifacts. We propose Node Replication (NR), a black-box approach to obtaining such data structures. NR takes an arbitrary sequential data structure and automatically transforms it into a NUMA-aware concurrent data structure satisfying linearizability. Using NR requires no expertise in concurrent data structure design, and the result is free of concurrency bugs. NR draws ideas from two disciplines: shared-memory algorithms and distributed systems. Briefly, NR implements a NUMA-aware shared log, and then uses the log to replicate data structures consistently across NUMA nodes. NR is best suited for contended data structures, where it can outperform lock-free algorithms by 3.1x, and lock-based solutions by 30x. To show the benefits of NR to a real application, we apply NR to the data structures of Redis, an in-memory storage system. The result outperforms other methods by up to 14x. The cost of NR is additional memory for its log and replicas.

---
### CoRAL: Confined Recovery in Distributed Asynchronous Graph Processing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037747
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037747?download=true
* **Key Words**: Computer systems organization, Dependable and fault-tolerant systems and networks, General and reference, Cross-computing tools and techniques, Performance, Networks, Network performance evaluation, Software and its engineering, Software organization and properties, Software system structures, Distributed systems organizing principles, 
* **Abstract**: Existing distributed asynchronous graph processing systems employ checkpointing to capture globally consistent snapshots and rollback all machines to most recent checkpoint to recover from machine failures. In this paper we argue that recovery in distributed asynchronous graph processing does not require the entire execution state to be rolled back to a globally consistent state due to the relaxed asynchronous execution semantics. We define the properties required in the recovered state for it to be usable for correct asynchronous processing and develop CoRAL, a lightweight checkpointing and recovery algorithm. First, this algorithm carries out confined recovery that only rolls back graph execution states of the failed machines to affect recovery. Second, it relies upon lightweight checkpoints that capture locally consistent snapshots with a reduced peak network bandwidth requirement. Our experiments using real-world graphs show that our technique recovers from failures and finishes processing 1.5x to 3.2x faster compared to the traditional asynchronous checkpointing and recovery mechanism when failures impact 1 to 6 machines of a 16 machine cluster. Moreover, capturing locally consistent snapshots significantly reduces intermittent high peak bandwidth usage required to save the snapshots -- the average reduction in 99th percentile bandwidth ranges from 22% to 51% while 1 to 6 snapshot replicas are being maintained.

---
### KickStarter: Fast and Accurate Computations on Streaming Graphs via Trimmed Approximations.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037748
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037748?download=true
* **Key Words**: Mathematics of computing, Discrete mathematics, Graph theory, Graph algorithms, 
* **Abstract**: Continuous processing of a streaming graph maintains an approximate result of the iterative computation on a recent version of the graph. Upon a user query, the accurate result on the current graph can be quickly computed by feeding the approximate results to the iterative computation --- a form of incremental computation that corrects the (small amount of) error in the approximate result. Despite the effectiveness of this approach in processing growing graphs, it is generally not applicable when edge deletions are present --- existing approximations can lead to either incorrect results (e.g., monotonic computations terminate at an incorrect minima/maxima) or poor performance (e.g., with approximations, convergence takes longer than performing the computation from scratch).

---
### Browsix: Bridging the Gap Between Unix and the Browser.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037727
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037727?download=true
* **Key Words**: Information systems, World Wide Web, Web interfaces, Browsers, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, 
* **Abstract**: Applications written to run on conventional operating systems typically depend on OS abstractions like processes, pipes, signals, sockets, and a shared file system. Porting these applications to the web currently requires extensive rewriting or hosting significant portions of code server-side because browsers present a nontraditional runtime environment that lacks OS functionality.

---
### Optimizing CNNs on Multicores for Scalability, Performance and Goodput.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037745
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037745?download=true
* **Key Words**: Computing methodologies, Machine learning, Machine learning approaches, Neural networks, 
* **Abstract**: Convolutional Neural Networks (CNN) are a class of Ar- tificial Neural Networks (ANN) that are highly efficient at the pattern recognition tasks that underlie difficult AI prob- lems in a variety of domains, such as speech recognition, object recognition, and natural language processing. CNNs are, however, computationally intensive to train. This paper presents the first characterization of the per- formance optimization opportunities for training CNNs on CPUs. Our characterization includes insights based on the structure of the network itself (i.e., intrinsic arithmetic inten- sity of the convolution and its scalability under parallelism) as well as dynamic properties of its execution (i.e., sparsity of the computation).

---
### Locality Transformations for Nested Recursive Iteration Spaces.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037720
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037720?download=true
* **Key Words**: General and reference, Cross-computing tools and techniques, Performance, Software and its engineering, Software notations and tools, Compilers, General programming languages, Language features, Recursion, 
* **Abstract**: There has been a significant amount of effort invested in designing scheduling transformations such as loop tiling and loop fusion that rearrange the execution of dynamic instances of loop nests to place operations that access the same data close together temporally. In recent years, there has been interest in designing similar transformations that operate on recursive programs, but until now these transformations have only considered simple scenarios: multiple recursions to be fused, or a recursion nested inside a simple loop. This paper develops the first set of scheduling transformations for nested recursions: recursive methods that call other recursive methods. These are the recursive analog to nested loops. We present a transformation called recursion twisting that automatically improves locality at all levels of the memory hierarchy, and show that this transformation can yield substantial performance improvements across several benchmarks that exhibit nested recursion.

---
### Locality-Aware CTA Clustering for Modern GPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037709
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037709?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Single instruction, multiple data, Software and its engineering, Software notations and tools, Compilers, Runtime environments, 
* **Abstract**: Cache is designed to exploit locality; however, the role of on-chip L1 data caches on modern GPUs is often awkward. The locality among global memory requests from different SMs (Streaming Multiprocessors) is predominantly harvested by the commonly-shared L2 with long access latency; while the in-core locality, which is crucial for performance delivery, is handled explicitly by user-controlled scratchpad memory. In this work, we disclose another type of data locality that has been long ignored but with performance boosting potential --- the inter-CTA locality. Exploiting such locality is rather challenging due to unclear hardware feasibility, unknown and inaccessible underlying CTA scheduler, and small in-core cache capacity. To address these issues, we first conduct a thorough empirical exploration on various modern GPUs and demonstrate that inter-CTA locality can be harvested, both spatially and temporally, on L1 or L1/Tex unified cache. Through further quantification process, we prove the significance and commonality of such locality among GPU applications, and discuss whether such reuse is exploitable. By leveraging these insights, we propose the concept of CTA-Clustering and its associated software-based techniques to reshape the default CTA scheduling in order to group the CTAs with potential reuse together on the same SM. Our techniques require no hardware modification and can be directly deployed on existing GPUs. In addition, we incorporate these techniques into an integrated framework for automatic inter-CTA locality optimization. We evaluate our techniques using a wide range of popular GPU applications on all modern generations of NVIDIA GPU architectures. The results show that our proposed techniques significantly improve cache performance through reducing L2 cache transactions by 55%, 65%, 29%, 28% on average for Fermi, Kepler, Maxwell and Pascal, respectively, leading to an average of 1.46x, 1.48x, 1.45x, 1.41x (up to 3.8x, 3.6x, 3.1x, 3.3x) performance speedups for applications with algorithm-related inter-CTA reuse.

---
### Sound Loop Superoptimization for Google Native Client.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037754
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037754?download=true
* **Key Words**: General and reference, Cross-computing tools and techniques, Performance, Security and privacy, Systems security, Browser security, Software and its engineering, Software creation and management, Software verification and validation, Formal software verification, Software notations and tools, Compilers, General programming languages, Language types, Assembly languages, 
* **Abstract**: Software fault isolation (SFI) is an important technique for the construction of secure operating systems, web browsers, and other extensible software. We demonstrate that superoptimization can dramatically improve the performance of Google Native Client, a SFI system that ships inside the Google Chrome Browser. Key to our results are new techniques for superoptimization of loops: we propose a new architecture for superoptimization tools that incorporates both a fully sound verification technique to ensure correctness and a bounded verification technique to guide the search to optimized code. In our evaluation we optimize 13 libc string functions, formally verify the correctness of the optimizations and report a median and average speedup of 25% over the libraries shipped by Google.

---
### Improving Datacenter Efficiency.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3046426
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3046426?download=true
* **Key Words**: 
* **Abstract**: Internet companies can improve datacenter efficiency and reduce costs, by minimizing resource waste while avoiding (or limiting) performance degradation. In this talk, I will first overview a few of the efficiency-related efforts we are undertaking at Microsoft, including leveraging workload history to improve resource management. I will then discuss some lessons from deploying these efforts in production and how they relate to academic research.

---
### DudeTM: Building Durable Transactions with Decoupling for Persistent Memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037714
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037714?download=true
* **Key Words**: General and reference, Cross-computing tools and techniques, Reliability, Information systems, Information storage systems, Storage management, Software and its engineering, Software organization and properties, Extra-functional properties, Software reliability, 
* **Abstract**: Emerging non-volatile memory (NVM) offers non-volatility, byte-addressability and fast access at the same time. To make the best use of these properties, it has been shown by empirical evidence that programs should access NVM directly through CPU load and store instructions, so that the overhead of a traditional file system or database can be avoided. Thus, durable transactions become a common choice of applications for accessing persistent memory data in a crash consistent manner. However, existing durable transaction systems employ either undo logging, which requires a fence for every memory write, or redo logging, which requires intercepting all memory reads within transactions.

---
### ReFlex: Remote Flash ≈ Local Flash.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037732
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037732?download=true
* **Key Words**: Information systems, Information storage systems, Storage architectures, Storage network architectures, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, 
* **Abstract**: Remote access to NVMe Flash enables flexible scaling and high utilization of Flash capacity and IOPS within a datacenter. However, existing systems for remote Flash access either introduce significant performance overheads or fail to isolate the multiple remote clients sharing each Flash device. We present ReFlex, a software-based system for remote Flash access, that provides nearly identical performance to accessing local Flash. ReFlex uses a dataplane kernel to closely integrate networking and storage processing to achieve low latency and high throughput at low resource requirements. Specifically, ReFlex can serve up to 850K IOPS per core over TCP/IP networking, while adding 21us over direct access to local Flash. ReFlex uses a QoS scheduler that can enforce tail latency and throughput service-level objectives (SLOs) for thousands of remote clients. We show that ReFlex allows applications to use remote Flash while maintaining their original performance with local Flash.

---
### Approximate Storage of Compressed and Encrypted Videos.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037718
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037718?download=true
* **Key Words**: Computer systems organization, Dependable and fault-tolerant systems and networks, Reliability, Computing methodologies, Computer graphics, Image compression, Hardware, Emerging technologies, Memory and dense storage, Security and privacy, Formal methods and theory of security, Security requirements, Security services, Digital rights management, 
* **Abstract**: The popularization of video capture devices has created strong storage demand for encoded videos. Approximate storage can ease this demand by enabling denser storage at the expense of occasional errors. Unfortunately, even minor storage errors, such as bit flips, can result in major visual damage in encoded videos. Similarly, video encryption, widely employed for privacy and digital rights management, may create long dependencies between bits that show little or no tolerance to storage errors.

---
### Exploiting Intra-Request Slack to Improve SSD Performance.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037728
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037728?download=true
* **Key Words**: Hardware, Communication hardware, interfaces and storage, External storage, Integrated circuits, Semiconductor memory, Non-volatile memory, 
* **Abstract**: With Solid State Disks (SSDs) offering high degrees of parallelism, SSD controllers place data and direct requests to exploit the maximum offered hardware parallelism. In the quest to maximize parallelism and utilization, sub-requests of a request that are directed to different flash chips by the scheduler can experience differential wait times since their individual queues are not coordinated and load balanced at all times. Since the macro request is considered complete only when its last sub-request completes, some of its sub-requests that complete earlier have to necessarily wait for this last sub-request. This paper opens the door to a new class of schedulers to leverage such slack between sub-requests in order to improve response times. Specifically, the paper presents the design and implementation of a slack-enabled re-ordering scheduler, called Slacker, for sub-requests issued to each flash chip. Layered under a modern SSD request scheduler, Slacker estimates the slack of each incoming sub-request to a flash chip and allows them to jump ahead of existing sub-requests with sufficient slack so as to not detrimentally impact their response times. Slacker is simple to implement and imposes only marginal additions to the hardware. Using a spectrum of 21 workloads with diverse read-write characteristics, we show that Slacker provides as much as 19.5%, 13% and 14.5% improvement in response times, with average improvements of 12%, 6.5% and 8.5%, for write-intensive, read-intensive and read-write balanced workloads, respectively.

---
### Graspan: A Single-machine Disk-based Graph System for Interprocedural Static Analyses of Large-scale Systems Code.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037744
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037744?download=true
* **Key Words**: Information systems, Data management systems, Database design and models, Graph-based database models, Theory of computation, Semantics and reasoning, Program reasoning, Program analysis, 
* **Abstract**: There is more than a decade-long history of using static analysis to find bugs in systems such as Linux. Most of the existing static analyses developed for these systems are simple checkers that find bugs based on pattern matching. Despite the presence of many sophisticated interprocedural analyses, few of them have been employed to improve checkers for systems code due to their complex implementations and poor scalability. In this paper, we revisit the scalability problem of interprocedural static analysis from a "Big Data" perspective. That is, we turn sophisticated code analysis into Big Data analytics and leverage novel data processing techniques to solve this traditional programming language problem. We develop Graspan, a disk-based parallel graph system that uses an edge-pair centric computation model to compute dynamic transitive closures on very large program graphs.

---
### SC-DCNN: Highly-Scalable Deep Convolutional Neural Network using Stochastic Computing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037746
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037746?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Neural networks, General and reference, Document types, General conference proceedings, Hardware, Electronic design automation, Logic synthesis, Combinational synthesis, Sequential synthesis, Emerging technologies, Analysis and design of emerging devices and systems, Emerging architectures, Integrated circuits, Logic circuits, Arithmetic and datapath circuits, Design modules and hierarchy, Finite state machines, Reconfigurable logic and FPGAs, Hardware accelerators, Very large scale integration design, Application-specific VLSI designs, Application specific integrated circuits, 
* **Abstract**: With the recent advance of wearable devices and Internet of Things (IoTs), it becomes attractive to implement the Deep Convolutional Neural Networks (DCNNs) in embedded and portable systems. Currently, executing the software-based DCNNs requires high-performance servers, restricting the widespread deployment on embedded and mobile IoT devices. To overcome this obstacle, considerable research efforts have been made to develop highly-parallel and specialized DCNN accelerators using GPGPUs, FPGAs or ASICs.

---
### 3DGates: An Instruction-Level Energy Analysis and Optimization of 3D Printers.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037752
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037752?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Reconfigurable computing, Special purpose systems, Embedded and cyber-physical systems, Embedded systems, Firmware, Sensors and actuators, General and reference, Cross-computing tools and techniques, Software and its engineering, Software organization and properties, 
* **Abstract**: As the next-generation manufacturing driven force, 3D printing technology is having a transformative effect on various industrial domains and has been widely applied in a broad spectrum of applications. It also progresses towards other versatile fields with portable battery-powered 3D printers working on a limited energy budget. While reducing manufacturing energy is an essential challenge in industrial sustainability and national economics, this growing trend motivates us to explore the energy consumption of the 3D printer for the purpose of energy efficiency. To this end, we perform an in-depth analysis of energy consumption in commercial, off-the-shelf 3D printers from an instruction-level perspective. We build an instruction-level energy model and an energy profiler to analyze the energy cost during the fabrication process. From the insights obtained by the energy profiler, we propose and implement a cross-layer energy optimization solution, called 3DGates, which spans the instruction-set, the compiler and the firmware. We evaluate 3DGates over 338 benchmarks on a 3D printer and achieve an overall energy reduction of 25%.

---
### Efficient Address Translation for Architectures with Multiple Page Sizes.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037704
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093336.3037704?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Serial architectures, Pipeline computing, 
* **Abstract**: Processors and operating systems (OSes) support multiple memory page sizes. Superpages increase Translation Lookaside Buffer (TLB) hits, while small pages provide fine-grained memory protection. Ideally, TLBs should perform well for any distribution of page sizes. In reality, set-associative TLBs -- used frequently for their energy efficiency compared to fully-associative TLBs -- cannot (easily) support multiple page sizes concurrently. Instead, commercial systems typically implement separate set-associative TLBs for different page sizes. This means that when superpages are allocated aggressively, TLB misses may, counter intuitively, increase even if entries for small pages remain unused (and vice-versa). We invent MIX TLBs, energy-frugal set-associative structures that concurrently support all page sizes by exploiting superpage allocation patterns. MIX TLBs boost the performance (often by 10-30%) of big-memory applications on native CPUs, virtualized CPUs, and GPUs. MIX TLBs are simple and require no OS or program changes.

---
### Page Fault Support for Network Controllers.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037710
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093336.3037710?download=true
* **Key Words**: Hardware, Communication hardware, interfaces and storage, Networking hardware, Networks, Network components, End nodes, Network adapters, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Memory management, Virtual memory, Software infrastructure, Virtual machines, 
* **Abstract**: Direct network I/O allows network controllers (NICs) to expose multiple instances of themselves, to be used by untrusted software without a trusted intermediary. Direct I/O thus frees researchers from legacy software, fueling studies that innovate in multitenant setups. Such studies, however, overwhelmingly ignore one serious problem: direct memory accesses (DMAs) of NICs disallow page faults, forcing systems to either pin entire address spaces to physical memory and thereby hinder memory utilization, or resort to APIs that pin/unpin memory buffers before/after they are DMAed, which complicates the programming model and hampers performance.

---
### Towards "Full Containerization" in Containerized Network Function Virtualization.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037713
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093336.3037713?download=true
* **Key Words**: Mathematics of computing, Discrete mathematics, Graph theory, Network flows, Networks, Network components, Middle boxes / network appliances, Network performance evaluation, Network performance modeling, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Memory management, Theory of computation, Design and analysis of algorithms, Online algorithms, Caching and paging algorithms, 
* **Abstract**: With exploding traffic stuffing existing network infra-structure, today's telecommunication and cloud service providers resort to Network Function Virtualization (NFV) for greater agility and economics. Pioneer service provider such as AT&T proposes to adopt container in NFV to achieve shorter Virtualized Network Function (VNF) provisioning time and better runtime performance. However, we characterize typical NFV work-loads on the containers and find that the performance is unsatisfactory. We observe that the shared host OS net-work stack is the main bottleneck, where the traffic flow processing involves a large amount of intermediate memory buffers and results in significant last level cache pollution. Existing OS memory allocation policies fail to exploit the locality and data sharing information among buffers. In this paper, we propose NetContainer, a software framework that achieves fine-grained hardware resource management for containerized NFV platform. NetContainer employs a cache access overheads guided page coloring scheme to coordinately address the inter-flow cache access overheads and intra-flow cache access overheads. It maps the memory buffer pages that manifest low cache access overheads (across a flow or among the flows) to the same last level cache partition. NetContainer exploits a footprint theory based method to estimate the cache access overheads and a Min-Cost Max-Flow model to guide the memory buffer mappings. We implement the NetContainer in Linux kernel and extensively evaluate it with real NFV workloads. Exper-imental results show that NetContainer outperforms conventional page coloring-based memory allocator by 48% in terms of successful call rate.

---
### FLEP: Enabling Flexible and Efficient Preemption on GPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037742
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037742?download=true
* **Key Words**: Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Process management, Multiprocessing / multiprogramming / multitasking, 
* **Abstract**: GPUs are widely adopted in HPC and cloud computing platforms to accelerate general-purpose workloads. However, modern GPUs do not support flexible preemption, leading to performance and priority inversion problems in multi-tasking environments.

---
### SaberLDA: Sparsity-Aware Learning of Topic Models on GPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037740
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037740?download=true
* **Key Words**: Information systems, Information retrieval, Document representation, Document topic models, Theory of computation, Design and analysis of algorithms, Parallel algorithms, Vector / streaming algorithms, 
* **Abstract**: Latent Dirichlet Allocation (LDA) is a popular tool for analyzing discrete count data such as text and images. Applications require LDA to handle both large datasets and a large number of topics. Though distributed CPU systems have been used, GPU-based systems have emerged as a promising alternative because of the high computational power and memory bandwidth of GPUs. However, existing GPU-based LDA systems cannot support a large number of topics because they use algorithms on dense data structures whose time and space complexity is linear to the number of topics.

---
### Moonwalk: NRE Optimization in ASIC Clouds.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037749
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037749?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Cloud computing, Hardware, Emerging technologies, Analysis and design of emerging devices and systems, Emerging architectures, Power and energy, Power estimation and optimization, Enterprise level and data centers power issues, Very large scale integration design, Application-specific VLSI designs, Application specific integrated circuits, Economics of chip design and manufacturing, 
* **Abstract**: Cloud services are becoming increasingly globalized and data-center workloads are expanding exponentially. GPU and FPGA-based clouds have illustrated improvements in power and performance by accelerating compute-intensive workloads. ASIC-based clouds are a promising way to optimize the Total Cost of Ownership (TCO) of a given datacenter computation (e.g. YouTube transcoding) by reducing both energy consumption and marginal computation cost.

---
### Dynamic Resource Management for Efficient Utilization of Multitasking GPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037707
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037707?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Single instruction, multiple data, Hardware, Very large scale integration design, On-chip resource management, Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Process management, Multiprocessing / multiprogramming / multitasking, 
* **Abstract**: As graphics processing units (GPUs) are broadly adopted, running multiple applications on a GPU at the same time is beginning to attract wide attention. Recent proposals on multitasking GPUs have focused on either spatial multitasking, which partitions GPU resource at a streaming multiprocessor (SM) granularity, or simultaneous multikernel (SMK), which runs multiple kernels on the same SM. However, multitasking performance varies heavily depending on the resource partitions within each scheme, and the application mixes. In this paper, we propose GPU Maestro that performs dynamic resource management for efficient utilization of multitasking GPUs. GPU Maestro can discover the best performing GPU resource partition exploiting both spatial multitasking and SMK. Furthermore, dynamism within a kernel and interference between the kernels are automatically considered because GPU Maestro finds the best performing partition through direct measurements. Evaluations show that GPU Maestro can improve average system throughput by 20.2% and 13.9% over the baseline spatial multitasking and SMK, respectively.

---
### Identifying Security Critical Properties for the Dynamic Verification of a Processor.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037734
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037734?download=true
* **Key Words**: Computer systems organization, Architectures, Computing methodologies, Machine learning, Learning paradigms, Supervised learning, Security and privacy, Security in hardware, Theory of computation, Semantics and reasoning, Program reasoning, Invariants, 
* **Abstract**: We present a methodology for identifying security critical properties for use in the dynamic verification of a processor. Such verification has been shown to be an effective way to prevent exploits of vulnerabilities in the processor, given a meaningful set of security properties. We use known processor errata to establish an initial set of security-critical invariants of the processor. We then use machine learning to infer an additional set of invariants that are not tied to any particular, known vulnerability, yet are critical to security.

---
### Verification of a Practical Hardware Security Architecture Through Static Information Flow Analysis.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037739
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037739?download=true
* **Key Words**: Security and privacy, Formal methods and theory of security, Logic and verification, Security in hardware, Hardware security implementation, 
* **Abstract**: Hardware-based mechanisms for software isolation are becoming increasingly popular, but implementing these mechanisms correctly has proved difficult, undermining the root of security. This work introduces an effective way to formally verify important properties of such hardware security mechanisms. In our approach, hardware is developed using a lightweight security-typed hardware description language (HDL) that performs static information flow analysis. We show the practicality of our approach by implementing and verifying a simplified but realistic multi-core prototype of the ARM TrustZone architecture. To make the security-typed HDL expressive enough to verify a realistic processor, we develop new type system features. Our experiments suggest that information flow analysis is efficient, and programmer effort is modest. We also show that information flow constraints are an effective way to detect hardware vulnerabilities, including several found in commercial processors.

---
### CHERI JNI: Sinking the Java Security Model into the C.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037725
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037725?download=true
* **Key Words**: Hardware, Emerging technologies, Analysis and design of emerging devices and systems, Emerging languages and compilers, Security and privacy, Software and application security, 
* **Abstract**: Java provides security and robustness by building a high-level security model atop the foundation of memory protection. Unfortunately, any native code linked into a Java program -- including the million lines used to implement the standard library -- is able to bypass both the memory protection and the higher-level policies. We present a hardware-assisted implementation of the Java native code interface, which extends the guarantees required for Java's security model to native code.

---
### GRIFFIN: Guarding Control Flows Using Intel Processor Trace.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037716
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037716?download=true
* **Key Words**: Security and privacy, Systems security, Operating systems security, 
* **Abstract**: Researchers are actively exploring techniques to enforce control-flow integrity (CFI), which restricts program execution to a predefined set of targets for each indirect control transfer to prevent code-reuse attacks. While hardware-assisted CFI enforcement may have the potential for advantages in performance and flexibility over software instrumentation, current hardware-assisted defenses are either incomplete (i.e., do not enforce all control transfers) or less efficient in comparison. We find that the recent introduction of hardware features to log complete control-flow traces, such as Intel Processor Trace (PT), provides an opportunity to explore how efficient and flexible a hardware-assisted CFI enforcement system may become. While Intel PT was designed to aid in offline debugging and failure diagnosis, we explore its effectiveness for online CFI enforcement over unmodified binaries by designing a parallelized method for enforcing various types of CFI policies. We have implemented a prototype called GRIFFIN in the Linux 4.2 kernel that enables complete CFI enforcement over a variety of software, including the Firefox browser and its jitted code. Our experiments show that GRIFFIN can enforce fine-grained CFI policies with shadow stack as recommended by researchers at a performance that is comparable to software-only instrumentation techniques. In addition, we find that alternative logging approaches yield significant performance improvements for trace processing, identifying opportunities for further hardware assistance.

---
### Bolt: I Know What You Did Last Summer... In The Cloud.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037703
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037703?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Cloud computing, Security and privacy, Systems security, 
* **Abstract**: Cloud providers routinely schedule multiple applications per physical host to increase efficiency. The resulting interference on shared resources often leads to performance degradation and, more importantly, security vulnerabilities. Interference can leak important information ranging from a service's placement to confidential data, like private keys. We present Bolt, a practical system that accurately detects the type and characteristics of applications sharing a cloud platform based on the interference an adversary sees on shared resources. Bolt leverages online data mining techniques that only require 2-5 seconds for detection. In a multi-user study on EC2, Bolt correctly identifies the characteristics of 385 out of 436 diverse workloads. Extracting this information enables a wide spectrum of previously-impractical cloud attacks, including denial of service attacks (DoS) that increase tail latency by 140x, as well as resource freeing (RFA) and co-residency attacks. Finally, we show that while advanced isolation mechanisms, such as cache partitioning lower detection accuracy, they are insufficient to eliminate these vulnerabilities altogether. To do so, one must either disallow core sharing, or only allow it between threads of the same application, leading to significant inefficiencies and performance penalties.

---
### Neurosurgeon: Collaborative Intelligence Between the Cloud and Mobile Edge.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037698
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093336.3037698?download=true
* **Key Words**: Human-centered computing, Ubiquitous and mobile computing, Ubiquitous and mobile computing theory, concepts and paradigms, Mobile computing, Software and its engineering, Software organization and properties, Software system structures, Distributed systems organizing principles, Cloud computing, 
* **Abstract**: The computation for today's intelligent personal assistants such as Apple Siri, Google Now, and Microsoft Cortana, is performed in the cloud. This cloud-only approach requires significant amounts of data to be sent to the cloud over the wireless network and puts significant computational pressure on the datacenter. However, as the computational resources in mobile devices become more powerful and energy efficient, questions arise as to whether this cloud-only processing is desirable moving forward, and what are the implications of pushing some or all of this compute to the mobile devices on the edge.

---
### Thermostat: Application-transparent Page Management for Two-tiered Main Memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037706
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093336.3037706?download=true
* **Key Words**: Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Memory management, 
* **Abstract**: The advent of new memory technologies that are denser and cheaper than commodity DRAM has renewed interest in two-tiered main memory schemes. Infrequently accessed application data can be stored in such memories to achieve significant memory cost savings. Past research on two-tiered main memory has assumed a 4KB page size. However, 2MB huge pages are performance critical in cloud applications with large memory footprints, especially in virtualized cloud environments, where nested paging drastically increases the cost of 4KB page management. We present Thermostat, an application-transparent huge-page-aware mechanism to place pages in a dual-technology hybrid memory system while achieving both the cost advantages of two-tiered memory and performance advantages of transparent huge pages. We present an online page classification mechanism that accurately classifies both 4KB and 2MB pages as hot or cold while incurring no observable performance overhead across several representative cloud applications. We implement Thermostat in Linux kernel version 4.5 and evaluate its effectiveness on representative cloud computing workloads running under KVM virtualization. We emulate slow memory with performance characteristics approximating near-future high-density memory technology and show that Thermostat migrates up to 50% of application footprint to slow memory while limiting performance degradation to 3%, thereby reducing memory cost up to 30%.

---
### Breaking the Boundaries in Heterogeneous-ISA Datacenters.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037738
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093336.3037738?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Heterogeneous (hybrid) systems, Software and its engineering, Software notations and tools, Compilers, Software organization and properties, Contextual software domains, Operating systems, 
* **Abstract**: Energy efficiency is one of the most important design considerations in running modern datacenters. Datacenter operating systems rely on software techniques such as execution migration to achieve energy efficiency across pools of machines. Execution migration is possible in datacenters today because they consist mainly of homogeneous-ISA machines. However, recent market trends indicate that alternate ISAs such as ARM and PowerPC are pushing into the datacenter, meaning current execution migration techniques are no longer applicable. How can execution migration be applied in future heterogeneous-ISA datacenters?

---
### Automated Synthesis of Comprehensive Memory Model Litmus Test Suites.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037723
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093336.3037723?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Multicore architectures, Hardware, Hardware validation, Functional verification, Coverage metrics, Software and its engineering, Software organization and properties, Software functional properties, Correctness, Synchronization, 
* **Abstract**: The memory consistency model is a fundamental part of any shared memory architecture or programming model. Modern weak memory models are notoriously difficult to define and to implement correctly. Most real-world programming languages, compilers, and (micro)architectures therefore rely heavily on black-box testing methodologies. The success of such techniques requires that the suite of litmus tests used to perform the testing be comprehensive--it should ideally stress all obscure corner cases of the model and of its implementation. Most litmus test suites today are generated from some combination of manual effort and randomization; however, the complex and subtle nature of contemporary memory models means that manual effort is both error-prone and subject to incomplete coverage.

---
### DCatch: Automatically Detecting Distributed Concurrency Bugs in Cloud Systems.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037735
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093336.3037735?download=true
* **Key Words**: Software and its engineering, Software creation and management, Software verification and validation, Software defect analysis, Software testing and debugging, Software organization and properties, Extra-functional properties, Software reliability, Software system structures, Distributed systems organizing principles, Cloud computing, 
* **Abstract**: In big data and cloud computing era, reliability of distributed systems is extremely important. Unfortunately, distributed concurrency bugs, referred to as DCbugs, widely exist. They hide in the large state space of distributed cloud systems and manifest non-deterministically depending on the timing of distributed computation and communication. Effective techniques to detect DCbugs are desired. This paper presents a pilot solution, DCatch, in the world of DCbug detection. DCatch predicts DCbugs by analyzing correct execution of distributed systems. To build DCatch, we design a set of happens-before rules that model a wide variety of communication and concurrency mechanisms in real-world distributed cloud systems. We then build runtime tracing and trace analysis tools to effectively identify concurrent conflicting memory accesses in these systems. Finally, we design tools to help prune false positives and trigger DCbugs. We have evaluated DCatch on four representative open-source distributed cloud systems, Cassandra, Hadoop MapReduce, HBase, and ZooKeeper. By monitoring correct execution of seven workloads on these systems, DCatch reports 32 DCbugs, with 20 of them being truly harmful.

---
### Towards Practical Default-On Multi-Core Record/Replay.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037751
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093336.3037751?download=true
* **Key Words**: Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, 
* **Abstract**: We present Castor, a record/replay system for multi-core applications that provides consistently low and predictable overheads. With Castor, developers can leave record and replay on by default, making it practical to record and reproduce production bugs, or employ fault tolerance to recover from hardware failures.

---
### Pallas: Semantic-Aware Checking for Finding Deep Bugs in Fast Path.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037743
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093336.3037743?download=true
* **Key Words**: Software and its engineering, Software organization and properties, Contextual software domains, Operating systems, Extra-functional properties, Software reliability, 
* **Abstract**: Software optimization is constantly a serious concern for developing high-performance systems. To accelerate the workflow execution of a specific functionality, software developers usually define and implement a fast path to speed up the critical and commonly executed functions in the workflow. However, producing a bug-free fast path is nontrivial. Our study on the Linux kernel discloses that a committed fast path can have up to 19 follow-up patches for bug fixing, and most of them are deep semantic bugs, which are difficult to be pinpointed by existing bug-finding tools.

---
### Hardware-Software Co-design to Mitigate DRAM Refresh Overheads: A Case for Refresh-Aware Process Scheduling.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037724
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037724?download=true
* **Key Words**: 
* **Abstract**: DRAM cells need periodic refresh to maintain data integrity. With high capacity DRAMs, DRAM refresh poses a significant performance bottleneck as the number of rows to be refreshed (and hence the refresh cycle time, tRFC) with each refresh command increases. Modern day DRAMs perform refresh at a rank-level, while LPDDRs used in mobile environments support refresh at a per-bank level. Rank-level refresh degrades the performance significantly since none of the banks in a rank can serve the on-demand requests. Per-bank refresh alleviates some of the performance bottlenecks as the other banks in a rank are available for on-demand requests. Typical DRAM retention time is in the order several of milliseconds, viz, 64msec for environments operating in temperatures below 85 deg C and 32msec for environments operating above 85 deg C.

---
### Kill the Program Counter: Reconstructing Program Behavior in the Processor Cache Hierarchy.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037701
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037701?download=true
* **Key Words**: General and reference, Cross-computing tools and techniques, Performance, Hardware, Integrated circuits, Semiconductor memory, Dynamic memory, 
* **Abstract**: Data prefetching and cache replacement algorithms have been intensively studied in the design of high performance microprocessors. Typically, the data prefetcher operates in the private caches and does not interact with the replacement policy in the shared Last-Level Cache (LLC). Similarly, most replacement policies do not consider demand and prefetch requests as different types of requests. In particular, program counter (PC)-based replacement policies cannot learn from prefetch requests since the data prefetcher does not generate a PC value. PC-based policies can also be negatively affected by compiler optimizations. In this paper, we propose a holistic cache management technique called Kill-the-PC (KPC) that overcomes the weaknesses of traditional prefetching and replacement policy algorithms. KPC cache management has three novel contributions. First, a prefetcher which approximates the future use distance of prefetch requests based on its prediction confidence. Second, a simple replacement policy provides similar or better performance than current state-of-the-art PC-based prediction using global hysteresis. Third, KPC integrates prefetching and replacement policy into a whole system which is greater than the sum of its parts. Information from the prefetcher is used to improve the performance of the replacement policy and vice-versa. Finally, KPC removes the need to propagate the PC through entire on-chip cache hierarchy while providing a holistic cache management approach with better performance than state-of-the-art PC-, and non-PC-based schemes. Our evaluation shows that KPC provides 8% better performance than the best combination of existing prefetcher and replacement policy for multi-core workloads.

---
### TETRIS: Scalable and Efficient Neural Network Acceleration with 3D Memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037702
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037702?download=true
* **Key Words**: Computer systems organization, Architectures, Other architectures, Neural networks, 
* **Abstract**: The high accuracy of deep neural networks (NNs) has led to the development of NN accelerators that improve performance by two orders of magnitude. However, scaling these accelerators for higher performance with increasingly larger NNs exacerbates the cost and energy overheads of their memory systems, including the on-chip SRAM buffers and the off-chip DRAM channels.

---
### History-Based Arbitration for Fairness in Processor-Interconnect of NUMA Servers.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037753
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3093337.3037753?download=true
* **Key Words**: Computer systems organization, Architectures, Parallel architectures, Interconnection architectures, 
* **Abstract**: NUMA (non-uniform memory access) servers are commonly used in high-performance computing and datacenters. Within each server, a processor-interconnect (e.g., Intel QPI, AMD HyperTransport) is used to communicate between the different sockets or nodes. In this work, we explore the impact of the processor-interconnect on overall performance -- in particular, the performance un- fairness caused by processor-interconnect arbitration. It is well known that locally-fair arbitration does not guarantee globally-fair bandwidth sharing as closer nodes receive more bandwidth in a multi-hop network. However, this work demonstrates that the opposite can occur in a commodity NUMA server where remote nodes receive higher bandwidth (and perform better). We analyze this problem and iden- tify that this occurs because of external concentration used in router micro-architectures for processor-interconnects without globally-aware arbitration. While accessing remote memory can occur in any NUMA system, performance un- fairness (or performance variation) is more critical in cloud computing and virtual machines with shared resources. We demonstrate how this unfairness creates significant performance variation when a workload is executed on the Xen virtualization platform. We then provide analysis using synthetic workloads to better understand the source of unfair- ness and eliminate the impact of other shared resources, including the shared last-level cache and main memory. To provide fairness, we propose a novel, history-based arbitration that tracks the history of arbitration grants made in the previous history window. A weighted arbitration is done based on the history to provide global fairness. Through simulations, we show our proposed history-based arbitration can provide global fairness and minimize the processor- interconnect performance unfairness at low cost.

---
### Enabling Lightweight Transactions with Precision Time.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037722
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037722?download=true
* **Key Words**: Information systems, Information storage systems, Storage architectures, Distributed storage, 
* **Abstract**: Distributed transactional storage is an important service in today's data centers. Achieving high performance without high complexity is often a challenge for these systems due to sophisticated consistency protocols and multiple layers of abstraction. In this paper we show how to combine two emerging technologies---Software-Defined Flash (SDF) and precise synchronized clocks---to improve performance and reduce complexity for transactional storage within the data center.

---
### IncBricks: Toward In-Network Computation with an In-Network Cache.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037731
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037731?download=true
* **Key Words**: Computer systems organization, Architectures, Distributed architectures, Cloud computing, Hardware, Communication hardware, interfaces and storage, Networking hardware, Networks, Network services, In-network processing, 
* **Abstract**: The emergence of programmable network devices and the increasing data traffic of datacenters motivate the idea of in-network computation. By offloading compute operations onto intermediate networking devices (e.g., switches, network accelerators, middleboxes), one can (1) serve network requests on the fly with low latency; (2) reduce datacenter traffic and mitigate network congestion; and (3) save energy by running servers in a low-power mode. However, since (1) existing switch technology doesn't provide general computing capabilities, and (2) commodity datacenter networks are complex (e.g., hierarchical fat-tree topologies, multipath communication), enabling in-network computation inside a datacenter is challenging.

---
### AMNESIAC: Amnesic Automatic Computer.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037741
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037741?download=true
* **Key Words**: 
* **Abstract**: Due to imbalances in technology scaling, the energy consumption of data storage and communication by far exceeds the energy consumption of actual data production, i.e., computation. As a consequence, recomputing data can become more energy efficient than storing and retrieving precomputed data. At the same time, recomputation can relax the pressure on the memory hierarchy and the communication bandwidth. This study hence assesses the energy efficiency prospects of trading computation for communication. We introduce an illustrative proof-of-concept design, identify practical limitations, and provide design guidelines.

---
### Voltage Regulator Efficiency Aware Power Management.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3037697.3037717
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3037697.3037717?download=true
* **Key Words**: Computer systems organization, Architectures, Hardware, Power and energy, 
* **Abstract**: Conventional off-chip voltage regulators are typically bulky and slow, and are inefficient at exploiting system and workload variability using Dynamic Voltage and Frequency Scaling (DVFS). On-die integration of voltage regulators has the potential to increase the energy efficiency of computer systems by enabling power control at a fine granularity in both space and time. The energy conversion efficiency of on-chip regulators, however, is typically much lower than off-chip regulators, which results in significant energy losses. Fine-grained power control and high voltage regulator efficiency are difficult to achieve simultaneously, with either emerging on-chip or conventional off-chip regulators.
