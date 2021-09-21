---
permalink: /current-projects/
toc: true
---
## Current Projects

### Agile Hardware/Software Design Methodology

#### Agile Hardware (AHA!)
Although an agile approach is standard for software design, how to properly adapt this method to hardware is still an open question. This work addresses this question while building a system on chip (SoC) with specialized accelerators. Rather than using a traditional waterfall design flow, which starts by studying the application to be accelerated, we begin by constructing a complete flow from an application expressed in a high-level domain-specific language (DSL), in our case Halide, to a generic coarse-grained reconfigurable array (CGRA). As our understanding of the application grows, the CGRA design evolves, and we have developed a suite of tools that tune application code, the compiler, and the CGRA to increase the efficiency of the resulting implementation. To meet our continued need to update parts of the system while maintaining the end-to-end flow, we have created DSL-based hardware generators that not only provide the Verilog needed for the implementation of the CGRA, but also create the collateral that the compiler/mapper/place and route system needs to configure its operation. This work provides a systematic approach for designing and evolving high-performance and energy-efficient hardware-software systems for any application domain.

**Code:** [Stanford AHA! Github](https://github.com/StanfordAHA)

**Publications:**

**Creating an Agile Hardware Design Flow**  
R. Bahr, C. Barrett, N. Bhagdikar, A. Carsello, R. Daly, C. Donovick, D. Durst, K. Fatahalian, K. Feng, P. Hanrahan, T. Hofstee, M. Horowitz, D. Huff, F. Kjolstad, T. Kong, Q. Liu, M. Mann, J. Melchert, A. Nayak, A. Niemetz, G. Nyengele, P. Raina, S. Richardson, R. Setaluri, J. Setter, K. Sreedhar, M. Strange, J. Thomas, C. Torng, L. Truong, N. Tsiskaridze, K. Zhang  
*Design Automation Conference (DAC)*, July 2020. [Paper](https://stanford.box.com/s/lieh7jsdzhovw2e0j7amdre7sy8scp5j), [Video](https://stanford.box.com/s/6tv07vdy1s3ne2x6lrcj150m3fhubsaf), [Slides](https://stanford.box.com/s/crmvsvgtoser2oqvykex9t70g6ckpsdc)

**Automated Codesign of Domain-Specific Hardware Accelerators and Compilers**  
P. Raina, F. Kjolstad, M. Horowitz, P. Hanrahan, C. Barrett, K. Fatahalian  
*ASCR Workshop on Reimagining Codesign*, March 2021. [Paper](https://custom.cvent.com/DCBD4ADAAD004096B1E4AD96F3C8049E/files/event/f64a4f28b4734808924cc8c3d9a2af63/d03b30a559d14c909dab4c8096d2f191.pdf) 

**Compiling Halide Programs to Push-Memory Accelerators**  
Q. Liu, D. Huff, J. Setter, M. Strange, K. Feng, K. Sreedhar, Z. Wang, K. Zhang, M. Horowitz, P. Raina, F. Kjolstad  
*arXiv*, May 2021. [Paper](https://arxiv.org/abs/2105.12858)  

**A Framework for Adding Low-Overhead, Fine-Grained Power Domains to CGRAs**  
A. Nayak, K. Zhang, R. Setaluri, A. Carsello, M. Mann, S. Richardson, R. Bahr, P. Hanrahan, M. Horowitz, P. Raina  
*Design, Automation and Test in Europe Conference (DATE)*, March 2020. **([Best Paper Award Nominee](https://www.date-conference.com))** [Paper](https://ieeexplore.ieee.org/document/9116477/authors#authors)

* * *

#### Design Space Exploration of CGRA Processing Elements using Peak DSL
**Jackson Melchert, Kathleen Feng**  
Modern AI applications, that typically use neural networks (NNs), have a very diverse set layers and connections. Many networks combine traditional image and video processing operators with convolutional (CONV) and fully-connected (FC) layers to achieve state of the art accuracies. Existing NN accelerators have limited configurability and are optimized to only run CONV and FC layers, and cannot support this growing space of hybrid applications. Coarse-grained reconfigurable arrays (CGRAs) offer an excellent alternative for accelerating these applications. However, coming up with an optimal CGRA design requires a large amount of manual effort. This work creates a framework for automatic design space exploration of processing elements (PEs) in CGRAs. To find interesting PEs, we feed a dataflow graph representation of the application into a frequent subgraph mining algorithm. We then use subgraph merging techniques to allow for the acceleration of multiple subgraphs from the same application or different applications. By tuning which subgraphs are merged, we can explore the design space between more specialized and more general CGRA PEs. Finally, we leverage [PEak DSL](https://github.com/cdonovick/peak) to generate the PE hardware and a set of rewrite rules that map operators in the dataflow IR to the hardware PEs. This allows the AHA! compiler toolchain to map applications to a CGRA with these new PEs and evaluate efficiency.

**Publications:**

**Automated Design Space Exploration of CGRA Processing Element Architectures using Frequent Subgraph Analysis**  
J. Melchert, K. Feng, C. Donovick, R. Daly, C. Barrett, M. Horowitz, P. Hanrahan, P. Raina  
*arXiv*, April 2021. [Paper](https://arxiv.org/abs/2104.14155)

* * *

#### HLS-Based Framework for Generating Deep Neural Network Accelerators
**Xuan Yang, Kartik Prabhu**  
Deep neural networks require custom accelerators in order to run with high performance and energy efficiency. Several DNN accelerators that have been proposed have very similar properties, with some form of a systolic array and a hierarchy of on-chip buffers. However, designing accelerators from scratch is very expensive in terms of time and resources. To get around this, we have created a generator framework using high-level synthesis that can create DNN accelerator designs with different parameters. In addition to this, we have a tool that performs design space exploration and finds the optimal set of parameters such as array and memory sizes in terms of energy and performance. The tool also finds the best scheduling (loop tiling and ordering) of any neural network layer on the accelerator. In other words, the system doesn't just generate the accelerator hardware, but also the compiler for it. We are using this system as a class project in EE272, our chip design bootcamp class.

**Code:** [Accelerator Generator](https://github.com/priyanka-raina/dnn-accelerator), [Compiler](https://github.com/xuanyoya/CNN-blocking/tree/dev)

**Publications:**

**Using Halide’s Scheduling Language to Analyze DNN Accelerators**  
X. Yang, M. Gao, Q. Liu, J. Pu, A. Nayak, J. Setter, S. Bell, K. Cao, H. Ha, P. Raina, C. Kozyrakis, M. Horowitz  
*International Conference on Architectural Support for Programming Languages and Operating Systems (ASPLOS)*, March 2020. [Paper](https://dl.acm.org/doi/10.1145/3373376.3378514), [Video](https://youtu.be/vy3s6VZr8TQ), [Abstract](https://asplos.hosting2.acm.org/wp/wp-content/uploads/2020/abstracts/paper_4_0.html)

* * *

### Accelerator Architectures Leveraging Emerging Technologies

#### 3D CGRA Architecture with Hybrid RRAM-NEMS-Based Interconnect
**Akash Levy, Michael Oduoza, Akhilesh Balasingam**  
Programmable logic architectures such as FPGAs and CGRAs are extensively used in place of specialized ASICs to accelerate computationally-intensive algorithms. However, when compared with ASICs performing the same function, FPGAs typically have 10-40x lower logic density, 3-4x higher delay, and 5-12x higher dynamic power dissipation. Most of this overhead comes from the configurable interconnect. This work reduces this overhead by using RRAM-based configuration memory that actuates NEMS-based interconnect multiplexers, both of which can be integrated in 3D on top of silicon CMOS logic. This work also enables “normally off, instantly on” operation, which is critical for IoT devices with unreliable power sources. FPGAs need to load their configuration from off-chip memory on startup, which incurs a significant energy cost. This work leverages the non-volatility of RRAM to enable intermittent computing.

**Publications:**

**Efficient Routing for Coarse-Grained Reconfigurable Arrays using Multi-Pole NEM Relays**  
A. Levy, M. Oduoza, A. Balasingam, R. T. Howe, P. Raina  
To appear in *IEEE/ACM Asia and South Pacific Design Automation Conference (ASP-DAC)*, January 2022.    

* * *

#### One-Shot Learning using RRAM-Based Associative Memory
**Haitong Li, Hongjie Wang, Denisse Ventura**  
Real-time learning from a few examples (one/few-shot learning) is a key challenge for machine learning systems today. When never-seen-before data is encountered, conventional parametric models like DNNs need to re-learn their parameters via gradient-based learning, often requiring huge amount of data coupled with slow learning iterations. Non-parametric models (like nearest neighbours) do not require any training, but have lower accuracy. Recent research has combined the two to create "memory-augmented" neural networks (MANNs) that can rapidly learn new examples while still performing well on common examples. MANNs consist of a frontend, which is a traditional CNN or RNN, that extracts features from new classes, and a backend associative memory that stores a hashed version of these features. During learning, new features are stored in the memory, and during inference, the feature computed on input data is compared with all the features stored in the memory, and the closest match determines the classification result. This work implements an associative memory with an RRAM-based content addressable memory for area-efficient feature storage and fast feature matching. 

**Publications:**

**One-Shot Learning with Memory-Augmented Neural Networks Using a 64-kbit, 118 GOPS/W RRAM-Based Non-Volatile Associative Memory**  
H. Li, W.-C. Chen, A. Levy, C.-H. Wang, H. Wang, P. Chen, W. Wan, H.-S. P. Wong, P. Raina  
*Symposium on VLSI Technology (VLSI)*, June 2021. [Paper](https://ieeexplore.ieee.org/abstract/document/9508761) 

**SAPIENS: A 64-Kbit RRAM-Based Non-Volatile Associative Memory for One-Shot Learning and Inference at the Edge**   
H. Li, W.-C. Chen, A. Levy, C.-H. Wang, H. Wang, P. Chen, W. Wan, W.-S. Khwa, H. Chuang, Y.-D. Chih, M.-F. Chang, H.-S. P. Wong, P. Raina  
*IEEE Transactions on Electron Devices (T-ED)*, September 2021. [Paper](https://ieeexplore.ieee.org/document/9535369)  

* * *

#### Chimera: Compute (Immersed) in Memory with Embedded Resistive Arrays
**Kartik Prabhu, Kalhan Koul**  
CHIMERA is the first non-volatile deep neural network (DNN) chip for edge AI training and inference using foundry on-chip resistive RAM (RRAM) macros and no off-chip memory. CHIMERA achieves 0.92 TOPS peak performance and 2.2 TOPS/W. We scale inference to 6x larger DNNs by connecting 6 CHIMERAs with just 4% execution time and 5% energy costs, enabled by communication-sparse DNN mappings that exploit RRAM non-volatility through quick chip wakeup/shutdown. We demonstrate the first incremental edge AI training which overcomes RRAM write energy, speed, and endurance challenges. Our training achieves the same accuracy as traditional algorithms with up to 283x fewer RRAM weight update steps and 340x better energy-delay product. We thus demonstrate 10 years of 20 samples/minute incremental edge AI training on CHIMERA.

**Publications:**

**CHIMERA: A 0.92 TOPS, 2.2 TOPS/W Edge AI Accelerator with 2 MByte On-Chip Foundry Resistive RAM for Efficient Training and Inference**  
M. Giordano, K. Prabhu, K. Koul, R. M. Radway, A. Gural, R. Doshi, Z. F. Khan, J. W. Kustin, T. Liu, G. B. Lopes, V. Turbiner, W.-S. Khwa, Y.-D. Chih, M.-F. Chang, G. Lallement, B. Murmann, S. Mitra, P. Raina  
*Symposium on VLSI Circuits (VLSI)*, June 2021. [Paper](https://ieeexplore.ieee.org/abstract/document/9492347) 

**In the News:**

* New ‘AI-at-the-edge’ smartphone chip lives, and learns, close to home. ([Stanford Engineering](https://engineering.stanford.edu/magazine/article/new-ai-edge-smartphone-chip-lives-and-learns-close-home))

* * *

#### RRAM-Based In-Memory Computing Architecture for Probabilistic Graphical Models
**Weier Wan**  
![](/assets/images/weier_rram.png){: .align-right .width-fifteen-percent}
Many powerful neural networks such as probabilistic graphical models and recurrent neural networks require flexibility in dataflow and weight access patterns. This work implements an in-memory computing architecture in a 130-nm CMOS/RRAM process, that offers dataflow reconfigurability to address the limitations of previous designs. It acheives this with in-situ access to RRAM array and its transpose for efficient access to neural network weights and a voltage sensing stochastic analog neuron.

**Publications:**

**A Voltage-Mode Sensing Scheme with Differential-Row Weight Mapping For Energy-Efficient RRAM-Based In-Memory Computing**  
W. Wan, R. Kubendran, B. Gao, S. Joshi, P. Raina, H. Wu, G. Cauwenberghs, H.-S. P. Wong  
*Symposium on VLSI Circuits (VLSI)*, June 2020. [Video](https://stanford.box.com/s/n3pcrulsookozhpnxqwpkkbjhlaea1m3), [Slides](https://stanford.box.com/s/igmr2okv8ewdc4u4z1j92asb9fpozx56), [Demo](https://stanford.box.com/s/jgwhx5vszvxgijkh0xyen7q8dfmx7jue)

**A 74TMACS/W CMOS-ReRAM Neurosynaptic Core with Dynamically Reconfigurable Dataflow and In-Situ Transposable Weights for Probabilistic Graphical Models**  
W. Wan, R. Kubendran, S. B. Eryilmaz, W. Zhang, Y. Liao, D. Wu, S. Deiss, B. Gao, P. Raina, S. Joshi, H. Wu, G. Cauwenberghs, H.-S.P. Wong  
*International Solid-State Circuits Conference (ISSCC)*, February 2020. [Paper](https://ieeexplore.ieee.org/document/9062979)

**Edge AI without Compromise: Efficient, Versatile and Accurate Neurocomputing in Resistive Random-Access Memory**   
W. Wan, R. Kubendran, C. Schaefer, S. B. Eryilmaz, W. Zhang, D. Wu, S. Deiss, P. Raina, H. Qian, B. Gao, S. Joshi, H. Wu, H.-S. P. Wong, G. Cauwenberghs  
*arXiv*, August 2021. [Paper](https://arxiv.org/abs/2108.07879)  
