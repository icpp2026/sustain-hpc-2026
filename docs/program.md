## Workshop Program

SUSTAIN-HPC 2026 is a **half-day workshop** held on the morning of **September 28, 2026**, in conjunction with [ICPP 2026](https://icpp2026.github.io/){:target="_blank"} in Singapore. The programme combines two keynote talks, two invited talks, and four peer-reviewed paper presentations, with an emphasis on technical depth, interaction, and community building.

### Morning Programme (09:00–12:30)

<div class="program-table" markdown>

| Time | Session | Title / Speaker |
|------|---------|-----------------|
| 09:00–09:05 | Opening | **Welcome & Opening Remarks** |
| 09:05–09:35 | Keynote 1 | **High-Performance Indexing on Memory-Disaggregated Systems: When a Compiler Can Optimize, Why Burn LLM Tokens?**<br>Prof. Eric Chi Lik Lo · The Chinese University of Hong Kong (CUHK) |
| 09:35–10:00 | Invited Talk 1 | **Approximate Computing for AI Accelerator Design**<br>Prof. Xinyu Chen · HKUST(GZ) · Microelectronics Thrust |
| 10:00–10:15 | Paper Sharing | **Execution-Driven Auto-Tuning of Static Schedules for Resource-Efficient HPC** |
| 10:15–10:30 | Paper Sharing | **Portable to Efficient: Auto-Tuning Hardware-Agnostic GPU Kernels in Julia** |
| 10:30–11:00 | Break | **Tea Break** |
| 11:00–11:30 | Keynote 2 | **Sustainable AI Serving Through Resource-Aware Scheduling**<br>Prof. Haiying Shen · University of Virginia |
| 11:30–11:55 | Invited Talk 2 | **Title to be announced (quantum computing)**<br>Dr. Kong Jian Feng · A\*STAR Institute of Advanced Intelligence and Computing |
| 11:55–12:10 | Paper Sharing | **Spatiotemporal Load Balancing for Near-Memory Accelerated Databases by Partial Resharding** |
| 12:10–12:25 | Paper Sharing | **Energy Efficiency in Actor Systems: A Comparative Study of Akka and Elixir** |
| 12:25–12:30 | Closing | **Closing Remarks** |

</div>

Each paper sharing slot consists of a **10-minute talk** followed by **5 minutes of Q&A**.

!!! note
    The title of Dr. Kong Jian Feng's invited talk and abstracts for the invited talks will be added as they become available.

### Keynote Speakers

#### Prof. Eric Chi Lik Lo — The Chinese University of Hong Kong (CUHK)

**Talk title:** High-Performance Indexing on Memory-Disaggregated Systems: When a Compiler Can Optimize, Why Burn LLM Tokens?

**Abstract:** Deploying high-performance index structures on memory-disaggregated systems such as CXL and RDMA often requires painstaking tuning and code adaptation. Recent proposals advocate LLM-assisted auto-optimization; however, for this task, such approaches are often overkill. They incur substantial token and GPU costs, require many iterations, and depend on carefully crafted human specifications to guide the LLM.

In this talk, I present a compiler-driven alternative that eliminates both LLM involvement and the need for human-provided specifications. Our system takes existing, battle-tested index implementations as input, analyzes their access patterns, and automatically derives far-memory placement and access strategies. It operates fully automatically, without manual tuning or prompt engineering.

We show that this approach can robustly optimize industrial-strength index structures (including B+ trees, hash tables, and skip lists), matching or even surpassing hand-optimized designs such as DEX and SepHash across both RDMA- and CXL-based systems. By avoiding LLMs entirely, it removes token and GPU overhead, reduces complexity, and delivers a solution that is more predictable, easier to deploy, and significantly more sustainable in terms of energy and carbon footprint. I will present the key techniques and experimental results, and argue that, for many modern memory-disaggregated systems, a well-designed compiler is a more practical and efficient solution than LLM-based optimization.

**Biography:** Eric Lo is currently an Associate Professor in the Department of Computer Science and Engineering at the Chinese University of Hong Kong (CUHK). He earned his PhD in Computer Science from ETH Zurich and has previously worked at both Google and Microsoft. His recent research focuses on vector databases, serving systems for AI agents, and AI auto-research on system components. He is currently the PC Chair of ACM SoCC 2026 and an Associate Editor of The VLDB Journal. His work has received recognition in the form of awards and honorable mentions at conferences such as VLDB 2005 and ICDE 2012. In 2020, he received the ACM SIGMOD Research Highlight Award.

#### Prof. Haiying Shen — University of Virginia

**Talk title:** Sustainable AI Serving Through Resource-Aware Scheduling

**Abstract:** Generative AI is placing growing demands on computing infrastructure as models grow larger and services reach more users. Interactive applications must meet latency targets while using compute, memory, and energy efficiently. Agentic applications add long sequences of model and tool calls, making resource scheduling across tasks increasingly important.

This talk presents a vision for resource-aware AI serving across several scales. Drawing on our recent work, I will discuss scheduling at the cluster and request levels, coordinating retraining and inference, and managing KV caches for agentic workloads. These examples motivate future research on scheduling under uncertain demand and coordinating compute and memory across distributed infrastructure. The goal is to make AI serving more sustainable and scalable while preserving performance and application quality.

**Biography:** Dr. Haiying Shen is an Associate Professor in the Department of Computer Science at the University of Virginia. During her 2024 sabbatical, she served as a Consulting Researcher at Microsoft in Redmond, WA, where she focused on LLM systems. Her research area is distributed systems, with a focus on ML/LLM systems, cloud computing, edge computing, and cyber-physical systems (CPS). Dr. Shen has made significant contributions to her field, with an H-index of 53 and over 380 publications in top conferences and journals such as SIGCOMM, OSDI, EuroSys, SoCC, ASPLOS, CoNext, Infocom, IEEE/ACM Transactions on Networking (TON), IEEE Transactions on Parallel and Distributed Systems (TPDS), and IEEE Transactions on Mobile Computing (TMC). Her work has received the George N. Saridis Best Transactions Paper Award (2021), best paper awards at CloudCom (2016) and NAS (2018), a best paper runner-up award at ICCCN (2015), best paper award nominations at ICPP (2021), MASS (2011), and CCGrid (2009), and a best-in-session presentation award at INFOCOM (2017). She has also received several prestigious awards, including the Microsoft Faculty Fellowship Award (2010), IEEE TCSC Mid-Career Award (2015), IBM Faculty Award (2015), NSF CAREER Award (2013), and Sigma Xi Clemson Chapter Young Investigator Award (2013). Dr. Shen serves as an Associate Editor for TON, TMC, and IEEE Networking Letters (NL). She also has served as program co-chair and general co-chair for several international conferences and has participated in the program committees of numerous leading conferences.

### Invited Speakers

#### Prof. Xinyu Chen — The Hong Kong University of Science and Technology (Guangzhou)

**Talk title:** Approximate Computing for AI Accelerator Design

**Biography:** Xinyu Chen is an Assistant Professor of the Microelectronics Thrust at the Hong Kong University of Science and Technology (Guangzhou). Before joining HKUST(GZ), he held the position of Principal Engineer at Hisilicon, where he worked on hardware accelerator design for the next-generation DPU. He received his Ph.D. degree in Computer Science from National University of Singapore in 2022. His research aims to build sustainable computing solutions by harnessing the potential of hardware acceleration and system optimization. His research results are published in top venues such as MICRO, ISCA, FPGA, DAC, and ATC.

#### Dr. Kong Jian Feng — A\*STAR Institute of Advanced Intelligence and Computing

**Talk title:** To be announced (quantum computing)

**Biography:** Jian Feng is Senior Scientist at the A\*STAR Institute of Advanced Intelligence and Computing (IAIC) and serves as Deputy Head of the High Performance Computing (HPC) Chapter. He obtained his Ph.D. in Physics from the Massachusetts Institute of Technology (MIT), where he conducted research in condensed matter theory. His current research interests span quantum machine learning, hybrid quantum algorithms for applications such as combinatorial optimization, and simulation of quantum many-body systems.

### Accepted Papers

- Execution-Driven Auto-Tuning of Static Schedules for Resource-Efficient HPC
- Portable to Efficient: Auto-Tuning Hardware-Agnostic GPU Kernels in Julia
- Spatiotemporal Load Balancing for Near-Memory Accelerated Databases by Partial Resharding
- Energy Efficiency in Actor Systems: A Comparative Study of Akka and Elixir
