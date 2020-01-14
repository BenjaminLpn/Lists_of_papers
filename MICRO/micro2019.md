### micro 2019 | 80 papers.
---
### Wire-Aware Architecture and Dataflow for CNN Accelerators.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358316
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358316?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Neural networks 
* **Abstract**: In spite of several recent advancements, data movement in modern CNN accelerators remains a significant bottleneck. Architectures like Eyeriss implement large scratchpads within individual processing elements, while architectures like TPU v1 implement large systolic arrays and large monolithic caches. Several data movements in these prior works are therefore across long wires, and account for much of the energy consumption. In this work, we design a new wire-aware CNN accelerator, WAX, that employs a deep and distributed memory hierarchy, thus enabling data movement over short wires in the common case. An array of computational units, each with a small set of registers, is placed adjacent to a subarray of a large cache to form a single tile. Shift operations among these registers allow for high reuse with little wire traversal overhead. This approach optimizes the common case, where register fetches and access to a few-kilobyte buffer can be performed at very low cost. Operations beyond the tile require traversal over the cache's H-tree interconnect, but represent the uncommon case. For high reuse of operands, we introduce a family of new data mappings and dataflows. The best dataflow, WAXFlow-3, achieves a 2× improvement in performance and a 2.6-4.4× reduction in energy, relative to Eyeriss. As more WAX tiles are added, performance scales well until 128 tiles.

---
### Simba: Scaling Deep-Learning Inference with Multi-Chip-Module-Based Architecture.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358302
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358302?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Data flow architectures Neural networks Special purpose systems Parallel architectures Interconnection architectures Multicore architectures 
* **Abstract**: Package-level integration using multi-chip-modules (MCMs) is a promising approach for building large-scale systems. Compared to a large monolithic die, an MCM combines many smaller chiplets into a larger system, substantially reducing fabrication and design costs. Current MCMs typically only contain a handful of coarse-grained large chiplets due to the high area, performance, and energy overheads associated with inter-chiplet communication. This work investigates and quantifies the costs and benefits of using MCMs with fine-grained chiplets for deep learning inference, an application area with large compute and on-chip storage requirements. To evaluate the approach, we architected, implemented, fabricated, and tested Simba, a 36-chiplet prototype MCM system for deep-learning inference. Each chiplet achieves 4 TOPS peak performance, and the 36-chiplet MCM package achieves up to 128 TOPS and up to 6.1 TOPS/W. The MCM is configurable to support a flexible mapping of DNN layers to the distributed compute and storage units. To mitigate inter-chiplet communication overheads, we introduce three tiling optimizations that improve data locality. These optimizations achieve up to 16% speedup compared to the baseline layer mapping. Our evaluation shows that Simba can process 1988 images/s running ResNet-50 with batch size of one, delivering inference latency of 0.50 ms.

---
### ShapeShifter: Enabling Fine-Grain Data Width Adaptation in Deep Learning.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358295
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358295?download=true
* **Key Words**: 
* **Abstract**: We show that selecting a data width for all values in Deep Neural Networks, quantized or not and even if that width is different per layer, amounts to worst-case design. Much shorter data widths can be used if we target the common case by adjusting the data type width at a much finer granularity. We propose ShapeShifter, where we group weights and activations and encode them using a width specific to each group and where typical group sizes vary from 16 to 256 values. The per group widths are selected statically for the weights and dynamically by hardware for the activations. We present two applications of ShapeShifter. In the first, that is applicable to any system, ShapeShifter reduces off- and on-chip storage and communication. This ShapeShifter-based memory compression is simple and low cost yet reduces off-chip traffic to 33% and 36% for 8-bit and 16-bit models respectively. This makes it possible to sustain higher performance for a given off-chip memory interface while also boosting energy efficiency. In the second application, we show how ShapeShifter can be implemented as a surgical extension over designs that exploit variable precision in time.

---
### MI6: Secure Enclaves in a Speculative Out-of-Order Processor.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358310
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358310?download=true
* **Key Words**: Computer systems organization Architectures Parallel architectures Multicore architectures 
* **Abstract**: Recent attacks have broken process isolation by exploiting microarchitectural side channels that allow indirect access to shared microarchitectural state. Enclaves strengthen the process abstraction to restore isolation guarantees.

---
### Cyclone: Detecting Contention-Based Cache Information Leaks Through Cyclic Interference.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358273
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358273?download=true
* **Key Words**: Security and privacy Intrusion/anomaly detection and malware mitigation Malware and its mitigation Security in hardware Hardware attacks and countermeasures Side-channel analysis and countermeasures 
* **Abstract**: Micro-architecture units like caches are notorious for leaking secrets across security domains. An attacker program can contend for on-chip state or bandwidth and can even use speculative execution in processors to drive this contention; and protecting against all contention-driven attacks is exceptionally challenging. Prior works can mitigate contention channels through caches by partitioning the larger, lower-level caches or by looking for anomalous performance or contention behavior. Neither scales to large number of fine-grained domains as required by browsers and web-services that place many domains within the same address space.

---
### CleanupSpec: An "Undo" Approach to Safe Speculation.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358314
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358314?download=true
* **Key Words**: Computer systems organization Architectures Security and privacy Security in hardware Hardware attacks and countermeasures Side-channel analysis and countermeasures 
* **Abstract**: Speculation-based attacks affect hundreds of millions of computers. These attacks typically exploit caches to leak information, using speculative instructions to cause changes to the cache state. Hardware-based solutions that protect against such forms of attacks try to prevent any speculative changes to the cache sub-system by delaying them. For example, InvisiSpec, a recent work, splits the load into two operations: the first operation is speculative and obtains the value and the second operation is non-speculative and changes the state of the cache. Unfortunately, such a "Redo" based approach typically incurs slowdown due to the requirement of extra operations for correctly speculated loads, that form the large majority of loads.

---
### eAP: A Scalable and Efficient In-Memory Accelerator for Automata Processing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358324
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358324?download=true
* **Key Words**: Computer systems organization Architectures Parallel architectures Multiple instruction, single data Hardware Emerging technologies Analysis and design of emerging devices and systems Emerging architectures Theory of computation Formal languages and automata theory 
* **Abstract**: Accelerating finite automata processing benefits regular-expression workloads and a wide range of other applications that do not map obviously to regular expressions, including pattern mining, bioinformatics, and machine learning. Existing in-memory automata processing accelerators suffer from inefficient routing architectures. They are either incapable of efficiently place-and-route a highly connected automaton or require an excessive amount of hardware resources.

---
### ComputeDRAM: In-Memory Compute Using Off-the-Shelf DRAMs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358260
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358260?download=true
* **Key Words**: Computer systems organization Architectures Parallel architectures Hardware Integrated circuits Semiconductor memory Dynamic memory 
* **Abstract**: In-memory computing has long been promised as a solution to the "Memory Wall" problem. Recent work has proposed using chargesharing on the bit-lines of a memory in order to compute in-place and with massive parallelism, all without having to move data across the memory bus. Unfortunately, prior work has required modification to RAM designs (e.g. adding multiple row decoders) in order to open multiple rows simultaneously. So far, the competitive and low-margin nature of the DRAM industry has made commercial DRAM manufacturers resist adding any additional logic into DRAM. This paper addresses the need for in-memory computation with little to no change to DRAM designs. It is the first work to demonstrate in-memory computation with off-the-shelf, unmodified, commercial, DRAM. This is accomplished by violating the nominal timing specification and activating multiple rows in rapid succession, which happens to leave multiple rows open simultaneously, thereby enabling bit-line charge sharing. We use a constraint-violating command sequence to implement and demonstrate row copy, logical OR, and logical AND in unmodified, commodity, DRAM. Subsequently, we employ these primitives to develop an architecture for arbitrary, massively-parallel, computation. Utilizing a customized DRAM controller in an FPGA and commodity DRAM modules, we characterize this opportunity in hardware for all major DRAM vendors. This work stands as a proof of concept that in-memory computation is possible with unmodified DRAM modules and that there exists a financially feasible way for DRAM manufacturers to support in-memory compute.

---
### CASCADE: Connecting RRAMs to Extend Analog Dataflow In An End-To-End In-Memory Processing Paradigm.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358328
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358328?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Neural networks Parallel architectures Single instruction, multiple data 
* **Abstract**: Processing in memory (PIM) is a concept to enable massively parallel dot products while keeping one set of operands in memory. PIM is ideal for computationally demanding deep neural networks (DNNs) and recurrent neural networks (RNNs). Processing in resistive RAM (RRAM) is particularly appealing due to RRAM's high density and low energy. A key limitation of PIM is the cost of multibit analog-to-digital (A/D) conversions that can defeat the efficiency and performance benefits of PIM. In this work, we demonstrate the CASCADE architecture that connects multiply-accumulate (MAC) RRAM arrays with buffer RRAM arrays to extend the processing in analog and in memory: dot products are followed by partial-sum buffering and accumulation to implement a complete DNN or RNN layer. Design choices are made and the interface is designed to enable a variation-tolerant, robust analog dataflow. A new memory mapping scheme named R-Mapping is devised to enable the in-RRAM accumulation of partial sums; and an analog summation scheme is used to reduce the number of A/D conversions required to obtain the final sum. CASCADE is compared with recent in-RRAM computation architectures using state-of-the-art DNN and RNN benchmarks. The results demonstrate that CASCADE improves the energy efficiency by 3.5× while maintaining a competitive throughput.

---
### ZCOMP: Reducing DNN Cross-Layer Memory Footprint Using Vector Extensions.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358305
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358305?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Neural networks Parallel architectures Single instruction, multiple data 
* **Abstract**: Deep Neural Networks (DNNs) are becoming the prevalent approach in computer vision, machine learning, natural language processing, and speech recognition applications. Although DNNs are perceived as compute-intensive tasks, they also apply intense pressure on the capacity and bandwidth of the memory hierarchy, primarily due to the large intermediate data communicated across network layers. Prior work on hardware DNN accelerators leverages the cross-layer data sparsity via fully-customized datapaths. However, dynamically compressing/expanding such data is a challenging task for general-purpose multi-processors with virtual memory and hardware-managed coherent cache hierarchies.

---
### Boosting the Performance of CNN Accelerators with Dynamic Fine-Grained Channel Gating.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358283
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358283?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Neural networks Computing methodologies Machine learning Machine learning approaches Neural networks 
* **Abstract**: This paper proposes a new fine-grained dynamic pruning technique for CNN inference, named channel gating, and presents an accelerator architecture that can effectively exploit the dynamic sparsity. Intuitively, channel gating identifies the regions in the feature map of each CNN layer that contribute less to the classification result and turns off a subset of channels for computing the activations in these less important regions. Unlike static network pruning, which removes redundant weights or neurons prior to inference, channel gating exploits dynamic sparsity specific to each input at run time and in a structured manner. To maximize compute savings while minimizing accuracy loss, channel gating learns the gating thresholds together with weights automatically through training. Experimental results show that the proposed approach can significantly speed up state-of-the-art networks with a marginal accuracy loss, and enable a trade-off between performance and accuracy. This paper also shows that channel gating can be supported with a small set of extensions to a CNN accelerator, and implements a prototype for quantized ResNet-18 models. The accelerator shows an average speedup of 2.3× for ImageNet when the theoretical FLOP reduction is 2.8×, indicating that the hardware can effectively exploit the dynamic sparsity exposed by channel gating.

---
### SparTen: A Sparse Tensor Accelerator for Convolutional Neural Networks.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358291
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358291?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Neural networks Special purpose systems 
* **Abstract**: Convolutional neural networks (CNNs) are emerging as powerful tools for image processing. Recent machine learning work has reduced CNNs' compute and data volumes by exploiting the naturally-occurring and actively-transformed zeros in the feature maps and filters. While previous semi-sparse architectures exploit one-sided sparsity either in the feature maps or the filters, but not both, a recent fully-sparse architecture, called Sparse CNN (SCNN), exploits two-sided sparsity to improve performance and energy over dense architectures. However, sparse vector-vector dot product, a key primitive in sparse CNNs, would be inefficient using the representation adopted by SCNN. The dot product requires finding and accessing non-zero elements in matching positions in the two sparse vectors -- an inner join using the position as the key with a single value field. SCNN avoids the inner join by performing a Cartesian product capturing the relevant multiplications. However, SCNN's approach incurs several considerable overheads and is not applicable to non-unit-stride convolutions. Further, exploiting reuse in sparse CNNs fundamentally causes systematic load imbalance not addressed by SCNN. We propose SparTen which achieves efficient inner join by providing support for native two-sided sparse execution and memory storage. To tackle load imbalance, SparTen employs a software scheme, called greedy balancing, which groups filters by density via two variants, a software-only one which uses whole-filter density and a software-hardware hybrid which uses finer-grain density. Our simulations show that, on average, SparTen performs 4.7x, 1.8x, and 3x better than a dense architecture, one-sided sparse architecture, and SCNN, respectively. An FPGA implementation shows that SparTen performs 4.3x and 1.9x better than a dense architecture and a one-sided sparse architecture, respectively.

---
### EDEN: Enabling Energy-Efficient, High-Performance Deep Neural Network Inference Using Approximate DRAM.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358280
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358280?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Neural networks Special purpose systems Computing methodologies Machine learning Machine learning approaches Neural networks Hardware Integrated circuits Semiconductor memory Dynamic memory 
* **Abstract**: The effectiveness of deep neural networks (DNN) in vision, speech, and language processing has prompted a tremendous demand for energy-efficient high-performance DNN inference systems. Due to the increasing memory intensity of most DNN workloads, main memory can dominate the system's energy consumption and stall time. One effective way to reduce the energy consumption and increase the performance of DNN inference systems is by using approximate memory, which operates with reduced supply voltage and reduced access latency parameters that violate standard specifications. Using approximate memory reduces reliability, leading to higher bit error rates. Fortunately, neural networks have an intrinsic capacity to tolerate increased bit errors. This can enable energy-efficient and high-performance neural network inference using approximate DRAM devices.

---
### eCNN: A Block-Based and Highly-Parallel CNN Accelerator for Edge Inference.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358263
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358263?download=true
* **Key Words**: Computer systems organization Embedded and cyber-physical systems Embedded systems Embedded hardware Computing methodologies Machine learning 
* **Abstract**: Convolutional neural networks (CNNs) have recently demonstrated superior quality for computational imaging applications. Therefore, they have great potential to revolutionize the image pipelines on cameras and displays. However, it is difficult for conventional CNN accelerators to support ultra-high-resolution videos at the edge due to their considerable DRAM bandwidth and power consumption. Therefore, finding a further memory- and computation-efficient microarchitecture is crucial to speed up this coming revolution.

---
### Dynamic Multi-Resolution Data Storage.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358282
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358282?download=true
* **Key Words**: 
* **Abstract**: Approximate computing that works on less precise data leads to significant performance gains and energy-cost reductions for compute kernels. However, without leveraging the full-stack design of computer systems, modern computer architectures undermine the potential of approximate computing.

---
### Exploiting Process Similarity of 3D Flash Memory for High Performance SSDs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358311
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358311?download=true
* **Key Words**: Computer systems organization Embedded and cyber-physical systems Embedded systems Firmware Hardware Integrated circuits Semiconductor memory Non-volatile memory 
* **Abstract**: 3D NAND flash memory exhibits two contrasting process characteristics from its manufacturing process. While process variability between different horizontal layers are well known, little has been systematically investigated about strong process similarity (PS) within the horizontal layer. In this paper, based on an extensive characterization study using real 3D flash chips, we show that 3D NAND flash memory possesses very strong process similarity within a 3D flash block: the word lines (WLs) on the same horizontal layer of the 3D flash block exhibit virtually equivalent reliability characteristics. This strong process similarity, which was not previously utilized, opens simple but effective new optimization opportunities for 3D flash memory. In this paper, we focus on exploiting the process similarity for improving the I/O latency. By carefully reusing various flash operating parameters monitored from accessing the leading WL, the remaining WLs on the same horizontal layer can be quickly accessed, avoiding unnecessary redundant steps for subsequent program and read operations. We also propose a new program sequence, called mixed order scheme (MOS), for 3D NAND flash memory which can further reduce the program latency. We have implemented a PS-aware FTL, called cubeFTL, which takes advantage of the proposed techniques. Our evaluation results show that cubeFTL can improve the IOPS by up to 48% over an existing PS-unaware FTL.

---
### DeepStore: In-Storage Acceleration for Intelligent Queries.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358320
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358320?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Special purpose systems Dependable and fault-tolerant systems and networks Secondary storage organization Information systems Information retrieval 
* **Abstract**: Recent advancements in deep learning techniques facilitate intelligent-query support in diverse applications, such as content-based image retrieval and audio texturing. Unlike conventional key-based queries, these intelligent queries lack efficient indexing and require complex compute operations for feature matching. To achieve high-performance intelligent querying against massive datasets, modern computing systems employ GPUs in-conjunction with solid-state drives (SSDs) for fast data access and parallel data processing. However, our characterization with various intelligent-query workloads developed with deep neural networks (DNNs), shows that the storage I/O bandwidth is still the major bottleneck that contributes 56%--90% of the query execution time.

---
### FIDR: A Scalable Storage System for Fine-Grain Inline Data Reduction with Efficient Memory Handling.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358303
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358303?download=true
* **Key Words**: Computer systems organization Architectures Hardware Communication hardware, interfaces and storage Information systems Information storage systems 
* **Abstract**: Storage systems play a critical role in modern servers which run highly data-intensive applications. To satisfy the high performance and capacity demands of such applications, storage systems now deploy an array of fast SSDs per server. To reduce the storage cost of employing many SSDs per server, storage systems actively perform inline data reduction (e.g., data deduplication, compression). Existing inline data reduction studies can achieve high performance and scalability by offloading computation-intensive data-reduction operations to dedicated hardware accelerators. However, such existing studies suffer from limited workload support and scalability. For example, they reduce only large data blocks, which incur many IO requests, leading to low data reduction rates, and their offloading overlooks memory-intensive operations, leading to the unoptimal scalability.

---
### Ensemble of Diverse Mappings: Improving Reliability of Quantum Computers by Orchestrating Dissimilar Mistakes.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358257
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358257?download=true
* **Key Words**: Hardware Emerging technologies Quantum technologies 
* **Abstract**: Near-term quantum computers do not have the ability to perform error correction. Such Noisy Intermediate Scale Quantum (NISQ) computers can produce incorrect output as the computation is subjected to errors. The applications on a NISQ machine try to infer the correct output by running the same program thousands of times and logging the output. If the error rates are low and the errors are not correlated, then the correct answer can be inferred as the one appearing with the highest frequency. Unfortunately, quantum computers are subjected to correlated errors, which can cause an incorrect answer to appear more frequently than the correct answer.

---
### Partial Compilation of Variational Algorithms for Noisy Intermediate-Scale Quantum Machines.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358313
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358313?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Quantum computing 
* **Abstract**: Quantum computing is on the cusp of reality with Noisy Intermediate-Scale Quantum (NISQ) machines currently under development and testing. Some of the most promising algorithms for these machines are variational algorithms that employ classical optimization coupled with quantum hardware to evaluate the quality of each candidate solution. Recent work used GRadient Descent Pulse Engineering (GRAPE) to translate quantum programs into highly optimized machine control pulses, resulting in a significant reduction in the execution time of programs. This is critical, as quantum machines can barely support the execution of short programs before failing.

---
### Mitigating Measurement Errors in Quantum Computers by Exploiting State-Dependent Bias.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358265
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358265?download=true
* **Key Words**: Hardware Emerging technologies Quantum technologies 
* **Abstract**: Quantum computers are susceptible to errors. While quantum computers can be guarded against errors using error correction codes, near-term quantum computers will not have sufficient number of qubits to implement error correction and must perform their computation in the presence of errors. Qubit measurement is typically the most error-prone operation on a quantum computer, with measurement errors ranging from 8% to 30% reported on current machines. This goal of this paper is to mitigate measurement errors by exploiting the state-dependent bias of measurement errors.

---
### A Case for Multi-Programming Quantum Computers.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358287
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358287?download=true
* **Key Words**: Hardware Emerging technologies Quantum technologies 
* **Abstract**: Existing and near-term quantum computers face significant reliability challenges because of high error rates caused by noise. Such machines are operated in the Noisy Intermediate Scale Quantum (NISQ) model of computing. As NISQ machines exhibit high error-rates, only programs that require a few qubits can be executed reliably. Therefore, NISQ machines tend to underutilize its resources. In this paper, we propose to improve the throughput and utilization of NISQ machines by using multi-programming and enabling the NISQ machine to concurrently execute multiple workloads.

---
### FlexLearn: Fast and Highly Efficient Brain Simulations Using Flexible On-Chip Learning.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358268
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358268?download=true
* **Key Words**: Hardware Emerging technologies Biology-related information processing Neural systems Integrated circuits 
* **Abstract**: To understand how the human brain works, neuroscientists heavily rely on brain simulations which incorporate the concept of time to their operating model. In the simulations, neurons transmit their signals through synapses whose weights change over time and by the activity of the associated neurons. Such changes in synaptic weights, known as learning, are thought to contribute to memory, and various learning rules exist to model different behaviors of the human brain. Due to the diverse neurons and learning rules, neuroscientists perform the simulations using highly programmable general-purpose processors. Unfortunately, the processors greatly suffer from the high computational overheads of the learning rules. As an alternative, brain simulation accelerators achieve orders of magnitude higher performance; however, they have limited flexibility and cannot support the diverse neurons and learning rules.

---
### ExTensor: An Accelerator for Sparse Tensor Algebra.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358275
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358275?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Special purpose systems 
* **Abstract**: Generalized tensor algebra is a prime candidate for acceleration via customized ASICs. Modern tensors feature a wide range of data sparsity, with the density of non-zero elements ranging from 10-6% to 50%. This paper proposes a novel approach to accelerate tensor kernels based on the principle of hierarchical elimination of computation in the presence of sparsity. This approach relies on rapidly finding intersections---situations where both operands of a multiplication are non-zero---enabling new data fetching mechanisms and avoiding memory latency overheads associated with sparse kernels implemented in software.

---
### GenCache: Leveraging In-Cache Operators for Efficient Sequence Alignment.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358308
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358308?download=true
* **Key Words**: Applied computing Life and medical sciences Computational biology Computational genomics Computer systems organization Architectures Other architectures Special purpose systems 
* **Abstract**: Precision Medicine will rely on frequent genomic analysis, especially for patients undergoing cancer treatments or suffering from rare diseases. Sequence alignment is invoked in multiple stages of the genomic analysis pipeline. Recent projects have introduced accelerators, GenAx and Darwin, for 2nd and 3rd generation sequencers respectively. In this work, we improve upon the GenAx design by increasing its parallelism and reducing its memory bandwidth demands. This is achieved with a combination of hardware and software innovations. We first integrate in-cache operators from prior work into the GenAx memory hierarchy; we then augment the in-cache peripheral circuit to support additional new operators. We then re-structure the sequence alignment algorithm to (i) leverage the many in-cache operators, (ii) exploit the common case in genomic datasets, (iii) use Bloom Filters to reduce futile accesses, and (iv) maximize data reuse within a re-organized memory hierarchy. While the baseline GenAx accelerator processes a batch of reads in 194 seconds while nearly saturating the 153.6 GB/s memory bandwidth, the proposed GenCache architecture processes the same batch of reads in 37 seconds at an improved energy efficiency of 8.6×, while demanding 20 GB/s average memory bandwidth. Our hardware and software techniques thus interact synergistically to target both memory and compute bottlenecks, while not affecting the outputs of the application. We show that the basic principles in GenCache can also be exploited by 3rd generation sequence aligners.

---
### Efficient SpMV Operation for Large and Highly Sparse Matrices using Scalable Multi-way Merge Parallelization.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358330
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358330?download=true
* **Key Words**: 
* **Abstract**: The importance of Sparse Matrix dense Vector multiplication (SpMV) operation in graph analytics and numerous scientific applications has led to development of custom accelerators that are intended to over-come the difficulties of sparse data operations on general purpose architectures. However, efficient SpMV operation on large problem (i.e. working set exceeds on-chip storage) is severely constrained due to strong dependence on limited amount of fast random access memory to scale. Additionally, unstructured matrix with high sparsity pose difficulties as most solutions rely on exploitation of data locality. This work presents an algorithm co-optimized scalable hardware architecture that can efficiently operate on very large (~billion nodes) and/or highly sparse (avg. degree <10) graphs with significantly less on-chip fast memory than existing solutions. A novel parallelization methodology for implementing large and high throughput multi-way merge network is the key enabler of this high performance SpMV accelerator. Additionally, a data compression scheme to reduce off-chip traffic and special computation for nodes with exceptionally large number of edges, commonly found in power-law graphs, are presented. This accelerator is demonstrated with 16-nm fabricated ASIC and Stratix® 10 FPGA platforms. Experimental results show more than an order of magnitude improvement over current custom hardware solutions and more than two orders of magnitude improvement over commercial off-the-shelf (COTS) architectures for both performance and energy efficiency.

---
### Sparse Tensor Core: Algorithm and Hardware Co-Design for Vector-wise Sparse Neural Networks on Modern GPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358269
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358269?download=true
* **Key Words**: Computer systems organization Architectures Parallel architectures Single instruction, multiple data 
* **Abstract**: Deep neural networks have become the compelling solution for the applications such as image classification, object detection, speech recognition, and machine translation. However, the great success comes at the cost of excessive computation due to the over-provisioned parameter space. To improve the computation efficiency of neural networks, many pruning techniques have been proposed to reduce the amount of multiply-accumulate (MAC) operations, which results in high sparsity in the networks.

---
### NVBit: A Dynamic Binary Instrumentation Framework for NVIDIA GPUs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358307
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358307?download=true
* **Key Words**: Computer systems organization Architectures Parallel architectures Single instruction, multiple data Software and its engineering Software notations and tools Compilers Dynamic compilers Just-in-time compilers 
* **Abstract**: Binary instrumentation frameworks are widely used to implement profilers, performance evaluation, error checking, and bug detection tools. While dynamic binary instrumentation tools such as PIN and DynamoRio are supported on CPUs, GPU architectures currently only have limited support for similar capabilities through static compile-time tools, which prohibits instrumentation of dynamically loaded libraries that are foundations for modern high-performance applications. This work presents NVBit, a fast, dynamic, and portable, binary instrumentation framework, that allows users to write instrumentation tools in CUDA/C/C++ and selectively apply that functionality to pre-compiled binaries and libraries executing on NVIDIA GPUs. Using dynamic recompilation at the SASS level, NVBit analyzes GPU kernel register requirements to generate efficient ABI compliant instrumented code without requiring the tool developer to have detailed knowledge of the underlying GPU architecture. NVBit allows basic-block instrumentation, multiple function injections to the same location, inspection of all ISA visible state, dynamic selection of instrumented or uninstrumented code, permanent modification of register state, source code correlation, and instruction removal. NVBit supports all recent NVIDIA GPU architecture families including Kepler, Maxwell, Pascal and Volta and works on any pre-compiled CUDA, OpenACC, OpenCL, or CUDA-Fortran application.

---
### Tangram: Integrated Control of Heterogeneous Computers.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358285
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358285?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Heterogeneous (hybrid) systems Hardware Power and energy Power estimation and optimization Chip-level power issues Platform power issues Thermal issues Temperature control 
* **Abstract**: Resource control in heterogeneous computers built with subsystems from different vendors is challenging. There is a tension between the need to quickly generate local decisions in each subsystem and the desire to coordinate the different subsystems for global optimization. In practice, global coordination among subsystems is considered hard, and current commercial systems use centralized controllers. The result is high response time and high design cost due to lack of modularity.

---
### CoSpec: Compiler Directed Speculative Intermittent Computation.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358279
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358279?download=true
* **Key Words**: 
* **Abstract**: Energy harvesting systems have emerged as an alternative to battery-operated embedded devices. Due to the intermittent nature of energy harvesting, researchers equip the systems with nonvolatile memory (NVM) and crash consistency mechanisms. However, prior works require non-trivial hardware modifications, e.g., a voltage monitor, nonvolatile flip-flops/scratchpad, dependence tracking modules, etc., thereby causing significant area/power/manufacturing costs.

---
### Applying Deep Learning to the Cache Replacement Problem.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358319
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358319?download=true
* **Key Words**: Computer systems organization Architectures Dependable and fault-tolerant systems and networks Processors and memory architectures 
* **Abstract**: Despite its success in many areas, deep learning is a poor fit for use in hardware predictors because these models are impractically large and slow, but this paper shows how we can use deep learning to help design a new cache replacement policy. We first show that for cache replacement, a powerful LSTM learning model can in an offline setting provide better accuracy than current hardware predictors. We then perform analysis to interpret this LSTM model, deriving a key insight that allows us to design a simple online model that matches the offline model's accuracy with orders of magnitude lower cost.

---
### DynaSprint: Microarchitectural Sprints with Dynamic Utility and Thermal Management.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358301
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358301?download=true
* **Key Words**: Computer systems organization Architectures Hardware Power and energy 
* **Abstract**: Sprinting is a class of mechanisms that provides a short but significant performance boost while temporarily exceeding the thermal design point. We propose DynaSprint, a software runtime that manages sprints by dynamically predicting utility and modeling thermal headroom. Moreover, we propose a new sprint mechanism for caches, increasing capacity briefly for enhanced performance. For a system that extends last-level cache capacity from 2MB to 4MB per core and can absorb 10J of heat, DynaSprint-guided cache sprints improve performance by 17% on average and by up to 40% over a non-sprinting system. These performance outcomes, within 95% of an oracular policy, are possible because DynaSprint accurately predicts phase behavior and sprint utility.

---
### Leveraging Caches to Accelerate Hash Tables and Memoization.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358272
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358272?download=true
* **Key Words**: Computer systems organization Architectures Parallel architectures Serial architectures Dependable and fault-tolerant systems and networks Processors and memory architectures 
* **Abstract**: Hash tables are widely used, but they are inefficient in current systems: they use core resources poorly and suffer from limited spatial locality in caches. To address these issues we propose HTA, a technique that accelerates hash table operations via simple ISA extensions and hardware changes. HTA adopts an efficient hash table format that leverages the characteristics of caches. HTA accelerates most operations in hardware, and leaves rare cases to software.

---
### Touché: Towards Ideal and Efficient Cache Compression By Mitigating Tag Area Overheads.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358281
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358281?download=true
* **Key Words**: Hardware Integrated circuits Semiconductor memory Static memory Very large scale integration design On-chip resource management 
* **Abstract**: Compression is seen as a simple technique to increase the effective cache capacity. Unfortunately, compression techniques either incur tag area overheads or restrict cache block placement to only include neighboring addresses. Ideally, we should be able to place compressed cache blocks without any restrictions or overheads.

---
### Distributed Logless Atomic Durability with Persistent Memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358321
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358321?download=true
* **Key Words**: Computer systems organization Dependable and fault-tolerant systems and networks Processors and memory architectures Information systems Information storage systems Information storage technologies Storage class memory Phase change memory 
* **Abstract**: Datacenter operators have started deploying Persistent Memory (PM), leveraging its combination of fast access and persistence for significant performance gains. A key challenge for PM-aware software is to maintain high performance while achieving atomic durability. The latter typically requires the use of logging, which introduces considerable overhead with additional CPU cycles, write traffic, and ordering requirements. In this paper, we exploit the data multiversioning inherent in the memory hierarchy to achieve atomic durability without logging. Our design, LAD, relies on persistent buffering space at the memory controllers (MCs)---already present in modern CPUs---to speculatively accumulate all of a transaction's updates before they are all atomically committed to PM. LAD employs an on-chip distributed commit protocol in hardware to manage the distributed speculative state each transaction accumulates across multiple MCs. We demonstrate that LAD is a practical design relying on modest hardware modifications to provide atomically durable transactions, while delivering up to 80% of ideal---i.e., PM-oblivious software's---performance.

---
### SuperMem: Enabling Application-transparent Secure Persistent Memory with Low Overheads.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358290
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358290?download=true
* **Key Words**: Hardware Integrated circuits Semiconductor memory Non-volatile memory Security and privacy Security in hardware Hardware attacks and countermeasures 
* **Abstract**: Non-volatile memory (NVM) suffers from security vulnerability to physical access based attacks due to non-volatility. To ensure data security in NVM, counter mode encryption is often used by considering its high security level and low decryption latency. However, the counter mode encryption incurs new persistence problem for crash consistency guarantee due to the requirement for atomically persisting both data and its counter. To address this problem, existing work requires a large battery backup or complex modifications on both hardware and software layers due to employing a writeback counter cache. The large battery backup is expensive and software-layer modifications limit the portability of applications from the un-encrypted NVM to the encrypted one. Our paper proposes SuperMem, an application-transparent secure persistent memory by leveraging a write-through counter cache to guarantee the atomicity of data and counter writes without the needs of a large battery backup and software-layer modifications. To reduce the performance overhead of a baseline write-through counter cache, SuperMem leverages a locality-aware counter write coalescing scheme to reduce the number of write requests by exploiting the spatial locality of counter storage and data writes. Moreover, SuperMem leverages a cross-bank counter storage scheme to efficiently distribute data and counter writes to different banks, thus speeding up writes by exploiting bank parallelism. Experimental results demonstrate that SuperMem improves the performance by about 2× compared with an encrypted NVM with a baseline write-through counter cache, and achieves the performance comparable to an ideal secure NVM that exhibits the optimal performance of an encrypted NVM.

---
### Constructing Large, Durable and Fast SSD System via Reprogramming 3D TLC Flash Memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358323
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358323?download=true
* **Key Words**: Computer systems organization Architectures Hardware Emerging technologies Memory and dense storage Robustness Hardware reliability 
* **Abstract**: NAND flash memory based SSDs have been widely studied and adopted. The scaling of SSD has evolved from plannar (2D) to 3D stacking. Compared with 2D SSD, 3D SSD stacks more layers into one block, constructing one block with more flash pages. For reliability and other reasons, technology node in 3D NAND SSD is larger than in 2D, but data density can be increased via increasing bit-per-cell. However, representing multiple bits per cell encounters additional challenges such as endurance and access latency. In this work, we develop a novel reprogramming scheme for TLCs in 3D NAND SSD, such that a cell can be programmed and reprogrammed several times before it is erased. Such reprogramming can reduce the frequency of erases which determines the endurance of a cell, improve the speed of programming, and increase the amount of bits written in a cell per program/erase cycle, i.e., effective capacity. Our work is the first to perform real 3D NAND SSD test to validate the feasibility of the reprogram operation. From the collected data, we derive the restrictions of performing reprogramming due to reliability challenges. Further, a reprogrammable SSD (ReSSD) is designed to structure reprogram operations, and when they should be applied. ReSSD is evaluated in a case study in 3D TLC SSD based RAID 5 system (RSS-RAID). Experimental results show that RSS-RAID can improve the endurance by 30.3%, boost write performance by 16.7%, and increase effective capacity by 7.71%, with negligible overhead compared with conventional 3D SSD based RAID 5 system.

---
### SWQUE: A Mode Switching Issue Queue with Priority-Correcting Circular Queue.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358293
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358293?download=true
* **Key Words**: Computer systems organization Architectures Serial architectures Superscalar architectures 
* **Abstract**: The improvement of single-thread performance is much needed. Among the many structures that comprise a processor, the issue queue (IQ) is one of the most important structures that influences high single-thread performance. Correctly assigning the issue priority and providing high capacity efficiency are key features, but no conventional IQ organizations do not sufficiently have these.

---
### Towards the adoption of Local Branch Predictors in Modern Out-of-Order Superscalar Processors.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358315
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358315?download=true
* **Key Words**: Computer systems organization Architectures Serial architectures Pipeline computing Superscalar architectures 
* **Abstract**: Branch prediction accuracy plays a dominant role in the performance provided by modern Out-of-Order(OOO) superscalar processors. While global history-based branch predictors are more popular, local history-based predictors offer an additional dimension towards enhancing the overall branch prediction accuracy. Integrating the local predictors in modern cores, though, comes with non-trivial challenges associated with managing the local predictor's state and repairing this state on any branch misprediction is essential for the local predictor to operate effectively. Using a highly accurate, industry standard simulator modeling a Skylake-like OOO core and workloads spanning diverse categories including Server, High Performance Computing (HPC) and personal computing suites, besides SPEC, we methodically highlight the issues that need to be tackled, why local predictor repair is non-trivial and the performance opportunity that is lost when the local predictor repair is not handled efficiently. We discuss the issues with prior techniques and quantify their limitations when using them in current OOO cores. Further, we propose three practical, implementable and efficient repair techniques with minimal storage requirements that provide significant performance gains for local predictors. Unlike prior repair techniques that can only attain 50% of the oracular gains, our realistic repair techniques retain about 80% of the oracular gains resulting in significantly better application performance.

---
### DSPatch: Dual Spatial Pattern Prefetcher.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358325
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358325?download=true
* **Key Words**: Computer systems organization Dependable and fault-tolerant systems and networks Processors and memory architectures 
* **Abstract**: High main memory latency continues to limit performance of modern high-performance out-of-order cores. While DRAM latency has remained nearly the same over many generations, DRAM bandwidth has grown significantly due to higher frequencies, newer architectures (DDR4, LPDDR4, GDDR5) and 3D-stacked memory packaging (HBM). Current state-of-the-art prefetchers do not do well in extracting higher performance when higher DRAM bandwidth is available. Prefetchers need the ability to dynamically adapt to available bandwidth, boosting prefetch count and prefetch coverage when headroom exists and throttling down to achieve high accuracy when the bandwidth utilization is close to peak.

---
### CHERIvoke: Characterising Pointer Revocation using CHERI Capabilities for Temporal Memory Safety.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358288
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358288?download=true
* **Key Words**: Computer systems organization Architectures Security and privacy Security in hardware Software and application security Systems security 
* **Abstract**: A lack of temporal safety in low-level languages has led to an epidemic of use-after-free exploits. These have surpassed in number and severity even the infamous buffer-overflow exploits violating spatial safety. Capability addressing can directly enforce spatial safety for the C language by enforcing bounds on pointers and by rendering pointers unforgeable. Nevertheless, an efficient solution for strong temporal memory safety remains elusive.

---
### Practical Byte-Granular Memory Blacklisting using Califorms.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358299
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358299?download=true
* **Key Words**: Computer systems organization Architectures Security and privacy Security in hardware 
* **Abstract**: Recent rapid strides in memory safety tools and hardware have improved software quality and security. While coarse-grained memory safety has improved, achieving memory safety at the granularity of individual objects remains a challenge due to high performance overheads usually between ~1.7x--2.2x. In this paper, we present a novel idea called Califorms, and associated program observations, to obtain a low overhead security solution for practical, byte-granular memory safety.

---
### NDA: Preventing Speculative Execution Attacks at Their Source.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358306
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358306?download=true
* **Key Words**: Computer systems organization Architectures Security and privacy Security in hardware Hardware security implementation 
* **Abstract**: Speculative execution attacks like Meltdown and Spectre work by accessing secret data in wrong-path execution. Secrets are then transmitted and recovered by the attacker via a covert channel. Existing mitigations either require code modifications, address only specific exploit techniques, or block only the cache covert channel. Rather than battling exploit techniques and covert channels one by one, we seek to close off speculative execution attacks at their source. Our key observation is that these attacks require a chain of dependent wrong-path instructions to access and transmit secret data. We propose NDA, a technique to restrict speculative data propagation. NDA breaks the attacks' wrong-path dependence chains while still allowing speculation and dynamic scheduling. We describe a design space of NDA variants that differ in the constraints they place on dynamic scheduling and the classes of speculative execution attacks they prevent. NDA preserves much of the performance advantage of out-of-order execution: on SPEC CPU 2017, NDA variants close 68-96% of the performance gap between in-order and unconstrained (insecure) out-of-order execution.

---
### MEDAL: Scalable DIMM based Near Data Processing Accelerator for DNA Seeding Algorithm.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358329
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358329?download=true
* **Key Words**: 
* **Abstract**: Computational genomics has proven its great potential to support precise and customized health care. However, with the wide adoption of the Next Generation Sequencing (NGS) technology, 'DNA Alignment', as the crucial step in computational genomics, is becoming more and more challenging due to the booming bio-data. Consequently, various hardware approaches have been explored to accelerate DNA seeding - the core and most time consuming step in DNA alignment.

---
### SMASH: Co-designing Software Compression and Hardware-Accelerated Indexing for Efficient Sparse Matrix Operations.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358286
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358286?download=true
* **Key Words**: 
* **Abstract**: Important workloads, such as machine learning and graph analytics applications, heavily involve sparse linear algebra operations. These operations use sparse matrix compression as an effective means to avoid storing zeros and performing unnecessary computation on zero elements. However, compression techniques like Compressed Sparse Row (CSR) that are widely used today introduce significant instruction overhead and expensive pointer-chasing operations to discover the positions of the non-zero elements. In this paper, we identify the discovery of the positions (i.e., indexing) of non-zero elements as a key bottleneck in sparse matrix-based workloads, which greatly reduces the benefits of compression.

---
### Alleviating Irregularity in Graph Analytics Acceleration: a Hardware/Software Co-Design Approach.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358318
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358318?download=true
* **Key Words**: Hardware Very large scale integration design Application-specific VLSI designs Application specific integrated circuits 
* **Abstract**: Graph analytics is an emerging application which extracts insights by processing large volumes of highly connected data, namely graphs. The parallel processing of graphs has been exploited at the algorithm level, which in turn incurs three irregularities onto computing and memory patterns that significantly hinder an efficient architecture design. Certain irregularities can be partially tackled by the prior domain-specific accelerator designs with well-designed scheduling of data access, while others remain unsolved.

---
### Tigris: Architecture and Algorithms for 3D Perception in Point Clouds.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358259
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358259?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Special purpose systems Human-centered computing Human computer interaction (HCI) Interaction paradigms Mixed / augmented reality 
* **Abstract**: Machine perception applications are increasingly moving toward manipulating and processing 3D point cloud. This paper focuses on point cloud registration, a key primitive of 3D data processing widely used in high-level tasks such as odometry, simultaneous localization and mapping, and 3D reconstruction. As these applications are routinely deployed in energy-constrained environments, real-time and energy-efficient point cloud registration is critical.

---
### ASV: Accelerated Stereo Vision System.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358253
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358253?download=true
* **Key Words**: Computing methodologies Artificial intelligence Computer vision Computer vision tasks Hardware Integrated circuits Reconfigurable logic and FPGAs Hardware accelerators Human-centered computing Ubiquitous and mobile computing Ubiquitous and mobile computing theory, concepts and paradigms Mobile computing Ubiquitous and mobile devices Mobile devices 
* **Abstract**: Estimating depth from stereo vision cameras, i.e., "depth from stereo", is critical to emerging intelligent applications deployed in energy- and performance-constrained devices, such as augmented reality headsets and mobile autonomous robots. While existing stereo vision systems make trade-offs between accuracy, performance and energy-efficiency, we describe ASV, an accelerated stereo vision system that simultaneously improves both performance and energy-efficiency while achieving high accuracy.

---
### Distilling the Essence of Raw Video to Reduce Memory Usage and Energy at Edge Devices.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358298
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358298?download=true
* **Key Words**: Computer systems organization Architectures Embedded and cyber-physical systems Human-centered computing Ubiquitous and mobile computing Ubiquitous and mobile devices Mobile devices 
* **Abstract**: Video broadcast and streaming are among the most widely used applications for edge devices. Roughly 82% of the mobile internet traffic is made up of video data. This is likely to worsen with the advent of 5G that will open up new opportunities for high resolution videos, virtual and augmented reality-based applications. The raw video data produced and consumed by edge devices is considerably higher than what is transmitted out of them. This leads to huge memory bandwidth and energy requirements from such edge devices. Therefore, optimizing the memory bandwidth and energy consumption needs is imperative for further improvements in energy efficiency of such edge devices. In this paper, we propose two mechanisms for on-the-fly compression and approximation of raw video data that is generated by the image sensors. The first mechanism, MidVB, performs lossless compression of the video frames coming out of the sensors and stores the compressed format into the memory. The second mechanism, Distill, builds on top of MidVB and further reduces memory consumption by approximating the video frame data. On an average, across 20 raw videos, MidVB and Distill are able to reduce the memory bandwidth by 43% and 72%, respectively, over the raw representation. They outperform a well known memory saving mechanism by 7% and 36%, respectively. Furthermore, MidVB and Distill reduce the energy consumption by 40% and 67%, respectively, over the baseline.

---
### MANIC: A Vector-Dataflow Architecture for Ultra-Low-Power Embedded Systems.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358277
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358277?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Data flow architectures Parallel architectures Single instruction, multiple data 
* **Abstract**: Ultra-low-power sensor nodes enable many new applications and are becoming increasingly pervasive and important. Energy efficiency is the key determinant of the value of these devices: battery-powered nodes want their battery to last, and nodes that harvest energy should minimize their time spent recharging. Unfortunately, current devices are energy-inefficient.

---
### SOSA: Self-Optimizing Learning with Self-Adaptive Control for Hierarchical System-on-Chip Management.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358312
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358312?download=true
* **Key Words**: 
* **Abstract**: Resource management strategies for many-core systems dictate the sharing of resources among applications such as power, processing cores, and memory bandwidth in order to achieve system goals. System goals require consideration of both system constraints (e.g., power envelope) and user demands (e.g., response time, energy-efficiency). Existing approaches use heuristics, control theory, and machine learning for resource management. They all depend on static system models, requiring a priori knowledge of system dynamics, and are therefore too rigid to adapt to emerging workloads or changing system dynamics.

---
### NetDIMM: Low-Latency Near-Memory Network Interface Architecture.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358278
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358278?download=true
* **Key Words**: Computer systems organization Architectures Distributed architectures Client-server architectures Hardware Communication hardware, interfaces and storage Networking hardware Integrated circuits Semiconductor memory Dynamic memory 
* **Abstract**: Optimizing bandwidth was the main focus of designing scale-out networks for several decades and this optimization trend has served well the traditional Internet applications. However, the emergence of datacenters as single computer entities has made latency as important as bandwidth in designing datacenter networks. PCIe interconnect is known to be latency bottleneck in communication networks as its latency overhead can contribute to up to ~90% of the overall communication latency. Despite its overheads, PCIe is the de facto interconnect standard in servers as it has been well established and maintained for more than two decades. In addition to PCIe overhead, data movements in network software stack consume thousands of processor cycles and make ultra-low latency networking more challenging. Tackling PCIe and data movement overheads, we architect NetDIMM, a near-memory network interface card capable of in-memory buffer cloning. NetDIMM places a network interface card chip into the buffer device of a dual in-line memory module and leverages the asynchronous memory access capability of DDR5 to share the memory modules between the host processor and near-memory NIC. Our evaluation shows NetDIMM, on average, improves per packet latency by 49.9% compared with a baseline network deploying PCIe NICs.

---
### GraphQ: Scalable PIM-Based Graph Processing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358256
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358256?download=true
* **Key Words**: Computer systems organization Architectures Parallel architectures Hardware Emerging technologies Analysis and design of emerging devices and systems Emerging architectures Integrated circuits 3D integrated circuits 
* **Abstract**: Processing-In-Memory (PIM) architectures based on recent technology advances (e.g., Hybrid Memory Cube) demonstrate great potential for graph processing. However, existing solutions did not address the key challenge of graph processing---irregular data movements.

---
### Charon: Specialized Near-Memory Processing Architecture for Clearing Dead Objects in Memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358297
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358297?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Heterogeneous (hybrid) systems Special purpose systems 
* **Abstract**: Garbage collection (GC) is a standard feature for high productivity programming, saving a programmer from many nasty memory-related bugs. However, these productivity benefits come with a cost in terms of application throughput, worst-case latency, and energy consumption. Since the first introduction of GC by the Lisp programming language in the 1950s, a myriad of hardware and software techniques have been proposed to reduce this cost. While the idea of accelerating GC in hardware is appealing, its impact has been very limited due to narrow coverage, lack of flexibility, intrusive system changes, and significant hardware cost. Even with specialized hardware GC performance is eventually limited by memory bandwidth bottleneck. Fortunately, emerging 3D stacked DRAM technologies shed new light on this decades-old problem by enabling efficient near-memory processing with ample memory bandwidth. Thus, we propose Charon1, the first 3D stacked memory-based GC accelerator. Through a detailed performance analysis of HotSpot JVM, we derive a set of key algorithmic primitives based on their GC time coverage and implementation complexity in hardware. Then we devise a specialized processing unit to substantially improve their memory-level parallelism and throughput with a low hardware cost. Our evaluation of Charon with the full-production HotSpot JVM running two big data analytics frameworks, Spark and GraphChi, demonstrates a 3.29× geomean speedup and 60.7% energy savings for GC over the baseline 8-core out-of-order processor.

---
### TensorDIMM: A Practical Near-Memory Processing Architecture for Embeddings and Tensor Operations in Deep Learning.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358284
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358284?download=true
* **Key Words**: Computer systems organization Architectures Parallel architectures 
* **Abstract**: Recent studies from several hyperscalars pinpoint to embedding layers as the most memory-intensive deep learning (DL) algorithm being deployed in today's datacenters. This paper addresses the memory capacity and bandwidth challenges of embedding layers and the associated tensor operations. We present our vertically integrated hardware/software co-design, which includes a custom DIMM module enhanced with near-memory processing cores tailored for DL tensor operations. These custom DIMMs are populated inside a GPU-centric system interconnect as a remote memory pool, allowing GPUs to utilize for scalable memory bandwidth and capacity expansion. A prototype implementation of our proposal on real DL systems shows an average 6.2-17.6× performance improvement on state-of-the-art DNN-based recommender systems.

---
### Understanding Reuse, Performance, and Hardware Cost of DNN Dataflow: A Data-Centric Approach.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358252
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358252?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Neural networks Hardware Electronic design automation Modeling and parameter extraction 
* **Abstract**: The data partitioning and scheduling strategies used by DNN accelerators to leverage reuse and perform staging are known as dataflow, which directly impacts the performance and energy efficiency of DNN accelerators. An accelerator micro architecture dictates the dataflow(s) that can be employed to execute layers in a DNN. Selecting a dataflow for a layer can have a large impact on utilization and energy efficiency, but there is a lack of understanding on the choices and consequences of dataflow, and of tools and methodologies to help architects explore the co-optimization design space.

---
### MaxNVM: Maximizing DNN Storage Density and Inference Efficiency with Sparse Encoding and Error Mitigation.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358258
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358258?download=true
* **Key Words**: Hardware Emerging technologies Memory and dense storage 
* **Abstract**: Deeply embedded applications require low-power, low-cost hardware that fits within stringent area constraints. Deep learning has many potential uses in these domains, but introduces significant inefficiencies stemming from off-chip DRAM accesses of model weights. Ideally, models would fit entirely on-chip. However, even with compression, memory requirements for state-of-the-art models make on-chip inference impractical. Due to increased density, emerging eNVMs are one promising solution.

---
### Neuron-Level Fuzzy Memoization in RNNs.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358309
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358309?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Neural networks Computing methodologies Machine learning 
* **Abstract**: Recurrent Neural Networks (RNNs) are a key technology for applications such as automatic speech recognition or machine translation. Unlike conventional feed-forward DNNs, RNNs remember past information to improve the accuracy of future predictions and, therefore, they are very effective for sequence processing problems.

---
### Manna: An Accelerator for Memory-Augmented Neural Networks.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358304
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358304?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Neural networks 
* **Abstract**: Memory-augmented neural networks (MANNs)-- which augment a traditional Deep Neural Network (DNN) with an external, differentiable memory-- are emerging as a promising direction in machine learning. MANNs have been shown to achieve one-shot learning and complex cognitive capabilities that are well beyond those of classical DNNs. We analyze the computational characteristics of MANNs and observe that they present a unique challenge due to soft reads and writes to the differentiable memory, each of which requires access to all the memory locations. This results in poor performance of MANNs on modern CPUs, GPUs, and other accelerators. To address this, we present Manna, a specialized hardware inference accelerator for MANNs. Manna is a memory-centric design that focuses on maximizing performance in an extremely low FLOPS/Byte context. The key architectural features from which Manna derives efficiency are: (i) investing most of the die area and power in highly banked on-chip memories that provide ample bandwidth rather than large matrix-multiply units that would be underutilized due to the low reuse (ii) a hardware-assisted transpose mechanism for accommodating the diverse memory access patterns observed in MANNs, (iii) a specialized processing tile that is equipped to handle the nearly-equal mix of MAC and non-MAC computations present in MANNs, and (iv) methods to map MANNs to Manna that minimize data movement while fully exploiting the little reuse present. We evaluate Manna by developing a detailed architectural simulator with timing and power models calibrated by synthesis to the 15 nm Nangate Open Cell library. Across a suite of 10 benchmarks, Manna demonstrates average speedups of 39x with average energy improvements of 122x over an NVIDIA 1080-Ti Pascal GPU and average speedups of 24x with average energy improvements of 86x over a state-of-the-art NVIDIA 2080-Ti Turing GPU.

---
### Binary Star: Coordinated Reliability in Heterogeneous Memory Systems for High Performance and Scalability.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358262
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358262?download=true
* **Key Words**: 
* **Abstract**: As memory capacity scales, traditional cache and memory hierarchy designs are facing increasingly difficult challenges in ensuring high reliability with low storage and performance cost. Recent developments in 3D die-stacked DRAM caches and nonvolatile memories (NVRAMs) introduce promising opportunities in tackling the reliability, performance, and capacity challenges, due to the diverse reliability characteristics of the technologies. However, simply replacing DRAM with NVRAM does not solve the reliability issues of the memory system, as conventional memory system designs maintain separate reliability schemes across caches and main memory. Our goal in this paper is to enable a reliable and high-performance memory hierarchy design, as memory capacity scales. To this end, we propose Binary Star, which coordinates the reliability schemes and consistent cache writeback between 3D-stacked DRAM last-level cache and NVRAM main memory to maintain the reliability of the cache and the memory hierarchy. Binary Star significantly reduces the performance and storage overhead of consistent cache writeback by coordinating it with NVRAM wear leveling. As a result, Binary Star is much more reliable and offers better performance than state-of-the-art memory systems with error correction. On a set of memory-intensive workloads, we show that Binary Star reduces memory failures in time (FIT) by 92.9% compared to state-of-the-art error correction schemes, while retaining 99% of the performance of a conventional DRAM design that provides no error correction.

---
### Quantifying Memory Underutilization in HPC Systems and Using it to Improve Performance via Architecture Support.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358267
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358267?download=true
* **Key Words**: Computer systems organization Architectures Distributed architectures Grid computing Hardware Integrated circuits Semiconductor memory Dynamic memory Software and its engineering Software organization and properties Contextual software domains Operating systems Memory management Main memory 
* **Abstract**: A system's memory size is often dictated by worst-case workloads with highest memory requirements; this causes memory to be underutilized in the common case when the system is not running its worst-case workloads. Cognizant of this memory underutilization problem, many prior works have studied memory utilization and explored how to improve it in the context of cloud.

---
### SSP: Eliminating Redundant Writes in Failure-Atomic NVRAMs via Shadow Sub-Paging.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358326
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358326?download=true
* **Key Words**: Computer systems organization Dependable and fault-tolerant systems and networks Reliability Information systems Information storage systems Information storage technologies Storage class memory Phase change memory 
* **Abstract**: Non-Volatile Random Access Memory (NVRAM) technologies are closing the performance gap between traditional storage and memory. However, the integrity of persistent data structures after an unclean shutdown remains a major concern. Logging is commonly used to ensure consistency of NVRAM systems, but it imposes significant performance overhead and causes additional wear out by writing extra data into NVRAM. Our goal is to eliminate the extra writes that are needed to achieve consistency. SSP (i) exploits a novel cache-line-level remapping mechanism to eliminate redundant data copies in NVRAM, (ii) minimizes the storage overheads using page consolidation and (iii) removes failure-atomicity overheads from the critical path, significantly improving the performance of NVRAM systems. Our evaluation results demonstrate that SSP reduces overall write traffic by up to 1.8×, reduces extra NVRAM writes in the critical path by up to 10× and improves transaction throughput by up to 1.6×, compared to a state-of-the-art logging design.

---
### Towards Efficient NVDIMM-based Heterogeneous Storage Hierarchy Management for Big Data Workloads.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358266
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358266?download=true
* **Key Words**: Computer systems organization Dependable and fault-tolerant systems and networks Secondary storage organization Hardware Emerging technologies Memory and dense storage 
* **Abstract**: In this paper, we propose a holistic solution to address several important and challenging issues in storage data management in light of emerging NVDIMM-based architecture: namely, new performance modeling, NVDIMM-based migration, and architectural support for NVDIMMs on migration optimization. In particular, a novel NVDIMM-based heterogeneous storage performance model is proposed to effectively address bus contention issues caused by placing NVDIMMs on the memory bus. We also develop an NVDIMM-based lazy migration scheme to effectively minimize adverse effects caused by memory traffic interferences during storage data management processes. Finally, the NVDIMM-based architectural support for migration optimization is proposed to increase channel parallelism in the destination NVDIMMs and bypass buffer caches in the source NVDIMMs, so that the impact of memory traffic can be alleviated. We present detailed evaluation and analysis to quantify how well our techniques can enhance the I/O performances of big workloads via efficient heterogeneous storage hierarchy management. Our experimental results show that overall the proposed techniques yield up to 98% performance improvement over the state-of-the-art techniques.

---
### Adding Tightly-Integrated Task Scheduling Acceleration to a RISC-V Multi-core Processor.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358271
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358271?download=true
* **Key Words**: General and reference Cross-computing tools and techniques Performance 
* **Abstract**: Task Parallelism is a parallel programming model that provides code annotation constructs to outline tasks and describe how their pointer parameters are accessed so that they might be executed in parallel, and asynchronously, by a runtime capable of inferring and honoring their data dependence relationships. It is supported by several parallelization frameworks, as OpenMP and StarSs.

---
### SWAP: Synchronized Weaving of Adjacent Packets for Network Deadlock Resolution.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358255
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358255?download=true
* **Key Words**: 
* **Abstract**: An interconnection network forms the communication backbone in both on-chip and off-chip systems. In networks, congestion causes packets to be blocked. Indefinite blocking can occur if cyclic dependencies exist, leading to deadlock. All modern networks devote resources to either avoid deadlock by eliminating cyclic dependences or to detect and recover from it.

---
### PUSh: Data Race Detection Based on Hardware-Supported Prevention of Unintended Sharing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358317
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358317?download=true
* **Key Words**: Software and its engineering Software creation and management Software verification and validation Software defect analysis Software testing and debugging Software organization and properties Contextual software domains Operating systems Memory management Virtual memory Software functional properties Correctness Synchronization 
* **Abstract**: Some of the most difficult to find bugs in multi-threaded programs are caused by unintended sharing, leading to data races. The detection of data races can be facilitated by requiring programmers to explicitly specify any intended sharing and then verifying compliance with these intentions. We present a novel dynamic checker based on this approach, called PUSh.

---
### EMI Architectural Model and Core Hopping.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358289
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358289?download=true
* **Key Words**: Computer systems organization Architectures Parallel architectures Multicore architectures Computing methodologies Modeling and simulation Model development and analysis Simulation evaluation 
* **Abstract**: Processors radiate electromagnetic interference (EMI), which affects wireless communication technologies. However, despite the fact that the EMI generated by a processor is deterministic, architecturally modeling the EMI has proven to be a complex challenge. Moreover, EMI depends on the physical layout of the processor and on the binary being executed (both the application and its compilation options).

---
### FPGA-Accelerated Optimistic Concurrency Control for Transactional Memory.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358270
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358270?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Reconfigurable computing Computing methodologies Parallel computing methodologies Parallel programming languages Hardware Integrated circuits Reconfigurable logic and FPGAs Hardware accelerators 
* **Abstract**: Transactional Memory (TM) has been considered as a promising alternative to existing synchronization operations, which are often the largest stumbling block to unleashing parallelism of applications. Efficient implementations of TM, however, are challenging due to the tension between lowering performance overhead and avoiding unnecessary aborts.

---
### Towards General Purpose Acceleration by Exploiting Common Data-Dependence Forms.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358276
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358276?download=true
* **Key Words**: Computer systems organization Architectures Other architectures Data flow architectures Heterogeneous (hybrid) systems Reconfigurable computing 
* **Abstract**: With slowing technology scaling, specialized accelerators are increasingly attractive solutions to continue expected generational scaling of performance. However, in order to accelerate more advanced algorithms or those from challenging domains, supporting data-dependence becomes necessary. This manifests as either data-dependent control (eg. join two sparse lists), or data-dependent memory accesses (eg. hash-table access). These forms of data-dependence inherently couple compute with memory, and also preclude efficient vectorization -- defeating the traditional mechanisms of programmable accelerators (eg. GPUs).

---
### μIR -An intermediate representation for transforming and optimizing the microarchitecture of application accelerators.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358292
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358292?download=true
* **Key Words**: 
* **Abstract**: Creating high quality application-specific accelerators requires us to make iterative changes to both algorithm behavior and microarchitecture, and this is a tedious and error-prone process. High-Level Synthesis (HLS) tools [5, 10] generate RTL for application accelerators from annotated software. Unfortunately, the generated RTL is challenging to change and optimize. The primary limitation of HLS is that the functionality and microarchitecture are conflated together in a single language (such as C++). Making changes to the accelerator design may require code restructuring, and microarchitecture optimizations are tied with program correctness.

---
### Speculative Taint Tracking (STT): A Comprehensive Protection for Speculatively Accessed Data.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358274
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358274?download=true
* **Key Words**: Security and privacy Security in hardware Hardware attacks and countermeasures Side-channel analysis and countermeasures 
* **Abstract**: Speculative execution attacks present an enormous security threat, capable of reading arbitrary program data under malicious speculation, and later exfiltrating that data over microarchitectural covert channels. Since these attacks first rely on being able to read arbitrary data (potential secrets), a conservative approach to defeat all attacks is to delay the execution of instructions that read those secrets, until those instructions become non-speculative.

---
### LATCH: A Locality-Aware Taint CHecker.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358327
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358327?download=true
* **Key Words**: Security and privacy Intrusion/anomaly detection and malware mitigation Intrusion detection systems Security in hardware Systems security Information flow control 
* **Abstract**: We present LATCH (short for Locality-Aware Taint CHecker), a generalizable architecture for optimizing dynamic information flow tracking (DIFT). LATCH exploits the observation that information flows under DIFT exhibit strong temporal locality, with typical applications manipulating sensitive data during limited phases of computation. This property allows LATCH to monitor significant spans of execution using lightweight, coarse-grained checks, invoking precise, computationally intensive tracking logic only during periods of execution that involve sensitive data. LATCH implements this policy without sacrificing the accuracy of DIFT.

---
### EMMA: Hardware/Software Attestation Framework for Embedded Systems Using Electromagnetic Signals.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358261
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358261?download=true
* **Key Words**: Security and privacy Security in hardware Embedded systems security 
* **Abstract**: Establishing trust for an execution environment is an important problem, and practical solutions for it rely on attestation, where an untrusted system (prover) computes a response to a challenge sent by the trusted system (verifier). The response typically is a checksum of the prover's program, which the verifier checks against expected values for a "clean" (trustworthy) system. The main challenge in attestation is that, in addition to checking the response, the verifier also needs to verify the integrity of the response computation. On higher-end processors, this integrity is verified cryptographically, using dedicated trusted hardware. On embedded systems, however, constraints prevent the use of such hardware support. Instead, a popular approach is to use the request-to-response time as a way to establish confidence. However, the overall request-to-response time provides only one coarse-grained measurement from which the integrity of the attestation is to be inferred, and even that is noisy because it includes the network latency and/or variations due to micro-architectural events. Thus, the attestation is vulnerable to attacks where the adversary has tampered with response computation, but the resulting additional computation time is small relative to the overall request-to-response time.

---
### Temporal Prefetching Without the Off-Chip Metadata.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358300
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358300?download=true
* **Key Words**: Computer systems organization Dependable and fault-tolerant systems and networks Processors and memory architectures 
* **Abstract**: Temporal prefetching offers great potential, but this potential is difficult to achieve because of the need to store large amounts of prefetcher metadata off chip. To reduce the latency and traffic of off-chip metadata accesses, recent advances in temporal prefetching have proposed increasingly complex mechanisms that cache and prefetch this off-chip metadata. This paper suggests a return to simplicity: We present a temporal prefetcher whose metadata resides entirely on chip. The key insights are (1) only a small portion of prefetcher metadata is important, and (2) for most workloads with irregular accesses, the benefits of an effective prefetcher outweigh the marginal benefits of a larger data cache. Thus, our solution, the Triage prefetcher, identifies important metadata and uses a portion of the LLC to store this metadata, and it dynamically partitions the LLC between data and metadata.

---
### PHI: Architectural Support for Synchronization- and Bandwidth-Efficient Commutative Scatter Updates.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358254
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358254?download=true
* **Key Words**: Computer systems organization Architectures Parallel architectures Multicore architectures 
* **Abstract**: Many applications perform frequent scatter update operations to large data structures. For example, in push-style graph algorithms, processing each vertex requires updating the data of all its neighbors. Neighbors are often scattered over the whole graph, so these scatter updates have poor spatial and temporal locality. In current systems, scatter updates suffer high synchronization costs and high memory traffic. These drawbacks make push-style execution unattractive, and, when algorithms allow it, programmers gravitate towards pull-style implementations based on gather reads instead.

---
### Prefetched Address Translation.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358294
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358294?download=true
* **Key Words**: Computer systems organization Architectures Serial architectures Software and its engineering Software organization and properties Contextual software domains Operating systems Memory management Allocation / deallocation strategies Virtual memory 
* **Abstract**: With explosive growth in dataset sizes and increasing machine memory capacities, per-application memory footprints are commonly reaching into hundreds of GBs. Such huge datasets pressure the TLB, resulting in frequent misses that must be resolved through a page walk -- a long-latency pointer chase through multiple levels of the in-memory radix tree-based page table.

---
### Directed Statistical Warming through Time Traveling.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358264
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358264?download=true
* **Key Words**: Computer systems organization Architectures Serial architectures Computing methodologies Modeling and simulation Hardware Emerging technologies Analysis and design of emerging devices and systems 
* **Abstract**: Improving the speed of computer architecture evaluation is of paramount importance to shorten the time-to-market when developing new platforms. Sampling is a widely used methodology to speed up workload analysis and performance evaluation by extrapolating from a set of representative detailed regions. Installing an accurate cache state for each detailed region is critical to achieving high accuracy. Prior work requires either huge amounts of storage (checkpoint-based warming), an excessive number of memory accesses to warm up the cache (functional warming), or the collection of a large number of reuse distances (randomized statistical warming) to accurately predict cache warm-up effects.

---
### Simmani: Runtime Power Modeling for Arbitrary RTL with Automatic Signal Selection.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358322
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358322?download=true
* **Key Words**: 
* **Abstract**: This paper presents a novel runtime power modeling methodology which automatically identifies key signals for power dissipation of any RTL design. The toggle-pattern matrix is constructed with the VCD dumps from a training set, where each signal is represented as a high-dimensional point. By clustering signals showing similar switching activities, a small number of signals are automatically selected, and then the design-specific but workload-independent activity-based power model is constructed using regression against cycle-accurate power traces obtained from industry-standard CAD tools. We can also automatically instrument an FPGA-accelerated RTL simulation with runtime activity counters to obtain power traces of realistic workloads at speed. Our methodology is demonstrated with a heterogeneous processor composed of an in-order core and a custom vector accelerator, running not only microbenchmarks but also real-world machine-learning applications.

---
### Architectural Implications of Function-as-a-Service Computing.
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3358296
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3358296?download=true
* **Key Words**: Computer systems organization Architectures Information systems Information systems applications Computing platforms Enterprise information systems Enterprise resource planning 
* **Abstract**: Serverless computing is a rapidly growing cloud application model, popularized by Amazon's Lambda platform. Serverless cloud services provide fine-grained provisioning of resources, which scale automatically with user demand. Function-as-a-Service (FaaS) applications follow this serverless model, with the developer providing their application as a set of functions which are executed in response to a user- or system-generated event. Functions are designed to be short-lived and execute inside containers or virtual machines, introducing a range of system-level overheads. This paper studies the architectural implications of this emerging paradigm. Using the commercial-grade Apache OpenWhisk FaaS platform on real servers, this work investigates and identifies the architectural implications of FaaS serverless computing. The workloads, along with the way that FaaS inherently interleaves short functions from many tenants frustrates many of the locality-preserving architectural structures common in modern processors. In particular, we find that: FaaS containerization brings up to 20x slowdown compared to native execution, cold-start can be over 10x a short function's execution time, branch mispredictions per kilo-instruction are 20x higher for short functions, memory bandwidth increases by 6x due to the invocation pattern, and IPC decreases by as much as 35% due to inter-function interference. We open-source FaaSProfiler, the FaaS testing and profiling platform that we developed for this work.

---
### InvisiSpec: Making Speculative Execution Invisible in the Cache Hierarchy (Corrigendum).
* **Publisher**: ACM
* **DOI**: https://doi.org/10.1145/3352460.3361129
* **PDF**: https://dl.acm.org/doi/pdf/10.1145/3352460.3361129?download=true
* **Key Words**: 
* **Abstract**: No abstract available.
