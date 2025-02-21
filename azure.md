Microsoft Azure VM Types Comparison
Jay Chapel
FAUN — Developer Community 🐾
Jay Chapel

·
Follow

Published in
FAUN — Developer Community 🐾

·
10 min read
·
Jun 23, 2020
85







There is a wide range of Microsoft Azure VM types that are optimized to meet various needs. Machine types are specialized, and vary by virtual CPU (vCPU), disk capability, and memory size, offering a number of options to match any workload.

With so many options available, finding the right machine type for your workload can be confusing — which is why we’ve created this overview of Azure VM types (as we’ve done with EC2 instance types, and Google Cloud machine types). Note that while AWS EC2 instance types have names associated with their purpose, Azure instance type names are simply in a series from A to N. The chart below and written descriptions are a brief and easy reference, but remember that finding the right machine type for your workload will always depend on your needs.


General Purpose
General-purpose VMs have a balanced CPU and memory, making them a great option for testing and development, smaller to medium databases, and web servers with low to medium traffic:

DCsv2-series
The newest size recommendation in the DC-series, the DCsv2, stands out because of the data protection and code confidentiality it provides while it’s being processed in the cloud. SGX technology and the latest generation of Intel XEON E-2288G Processor back these machines — these VMs can go up to 5.0GHz.

Av2 Series
A-series VMs have a CPU-to-memory ratio that works best for entry-level workloads, like those for development and testing. Sizing is throttled for consistent processor performance to run the instance. Av2-series has the option to be deployed on a number of hardware types and processors. To figure out which hardware the size should be deployed on, users must query the virtual hardware in the VM.

Dv2 and Dsv2-series
Dv2 VMs boast powerful CPUs — roughly 35% faster than D-series VMs — and optimized memory, great for production workloads. They have the same memory and disk configurations as the D-series, based upon either a 2.1 GHz, 2.3 GHz, or 2.4 GHz processor and Intel Boost Technology.

Dsv2-series sizes run on the same Dv2 processors with Intel Turbo Boost Technology 2.0 and also use premium storage.

Dv3-series
With expanded memory (from ~3.5 GiB/vCPU to 4 GiB/vCPU) and adjustments for disk and network limits, the Dv3 series Azure VM type offers the most value to general-purpose workloads. The sizes in this series offer a combination of memory, temporary storage, and vCPU that best fits best for enterprise applications, relational databases, in-memory caching, and analytics. It’s important to note that the Dv3-series no longer has the high memory VM sizes of the D/Dv2-series.

Dsv3-series
This series’ sizes feature premium storage disks and run on 2.1, 2.3, or 2.4 GHz Intel Xeon processors with Intel Turbo Boost Technology 2.0, the Dsv3-series is best suited for most production workloads.

B-series
Similar to the AWS t-series machine type family, B-series burstable VMs and ideal for workloads that do not rely on full and continuous CPU performance. Use cases for this series’ VM types include small databases, dev and test environments and low-traffic web servers, microservices, and more. Thanks to the B-series, customers can purchase a VM size that builds up credits when underutilized compared to its base performance, and the accumulated credits can be used as bursts. Spikes in compute power allow the VM to burst above the base performance if for higher CPU performance when needed.

Dav4 and Dasv4-series
Dav4-series are one of the new sizes that utilize a 2.35Ghz AMD EPYCTM 7452 processor and can reach a max frequency of 3.35GHz. The combination of memory, temporary storage, and vCPU makes these VMs suitable for most production workloads. For premium SSD, Dasv4-series sizes are the best option.

Ddv4 and Ddsv4-series
Similar to other VMs in the D-series, these sizes utilize a combination of memory, temporary disk storage, and vCPU that provides a better value for most general-purpose workloads. These new VM sizes have faster and 50% larger local storage (up to 2,400 GiB) and are designed for applications that benefit from low latency, high-speed local storage. The Ddv4-series processors run in a hyper-threaded configuration making them a great option for enterprise-grade applications, relational databases, in-memory caching, and analytics.

The major difference between the two series is that the Ddsv4-series supports Premium Storage and premium Storage caching, while Ddv4-series does not.

Dv4 and Dsv4-series
Both of these new series are currently in preview. The Dv4-series is optimal for general purpose workloads since they run on processors in a hyper-threaded configuration. It features a sustained all core Turbo clock speed of 3.4 GHz.

The Dsv4-series runs on the same processors as the Dv4-series, and even has the same features. The major difference between the two series is that the Dsv4-series supports Premium Storage and premium Storage caching, while Dv4-series does not.

Compute Optimized
Compute-optimized Azure VM types offer a high CPU-to-memory ratio. They’re suitable for medium traffic web servers, network appliances, batch processing, and application servers.

Fsv2-series
With a base core frequency of 3.4 GHz and a maximum single-core turbo frequency of 3.7 GHz, Fsv2 series VM types offer up to twice the performance boost for vector processing workloads. Not only do they offer great speed for any workload, but the Fsv2 also offers the best value for its price based on the ratio of Azure Compute Unit (ACU) per vCPU.

Memory-Optimized
Memory-optimized VM types are higher in memory as opposed to CPU, and best suited for relational database services, analytics, and larger caches.

M-Series
Enterprise applications and large databases will benefit most from the M-series for having the most memory (up to 3.8 TiB) and the highest vCPU count (up to 128) of any VM in the cloud.

Mv2-series
The VMs in this series offer the highest vCPU count (up to 416 vCPUs) and the largest memory (up to 11.4 TiB) of any VM. Because of these features, It’s ideal for extremely large databases or applications that benefit from high vCPU counts and large amounts of memory. The Mv2-series runs on an Intel® Xeon® processor with an all-core base frequency of 2.5 GHz and a max turbo frequency of 3.8 GHz.

Dv2 and DSv2-series 11–15
The Dv2 and DSv2-series 11–15 follow in the footsteps of the original D-series, the main differentiation is a more powerful CPU. For applications that require fast vCPUs, reliable temporary storage, and demand more memory, the Dv2 and DSv2-series all fit the bill for enterprise applications. The Dv2 series offers speed and power with a CPU about 35% faster than that of the D-series. Based on the 2.1, 2.3, and 2.4 GHz Intel Xeon® processors and with Intel Turbo Boost Technology 2.0, they can reach up to 3.1 GHz. The Dv2-series also has the same memory and disk configurations as the D-series.

Ev3-series and Esv3-series
The Ev3 follows in the footsteps of the high memory VM sizes originating from the D/Dv2 families. This Azure VM types provide excellent value for general-purpose workloads, boasting expanded memory (from 7 GiB/vCPU to 8 GiB/vCPU) with adjustments to disk and network limits per core basis in alignment with the move to hyperthreading.

The Esv3-series is the optimal choice for memory-intensive enterprise applications. If you want premium storage disks, the Esv3-series sizes are the perfect ones. A difference between the two series is that the Esv3-series supports Premium Storage and premium Storage caching, while Ev3-series does not.

Eav4 and Easv4-series
The Eav4 and Easv4-series utilize the processors they run on in a multi-threaded configuration increasing options for running memory optimized workloads. Though the Eav4-series and Easv4-series have the same memory and disk configurations as the Ev3 & Esv3-series, the Eav4-series sizes are ideal for memory-intensive enterprise applications.

Use the Easv4-series sizes for premium SSD. The Easv4-series sizes are ideal for memory-intensive enterprise applications. Easv4-series sizes can achieve a boosted maximum frequency of 3.35GHz.

Edv4 and Edsv4-series
High vCPU counts and large amounts of memory make Edv4 and Edsv4-series the ideal option for extremely large databases and other applications that benefit from these features. It features a sustained all core Turbo clock speed of 3.4 GHz and many new technology features. Unlike the Ev3/Esv3 sizes with Gen2 VMs, these new VM sizes will have 50% larger local storage, as well as better local disk IOPS for both, read and write.

The Edv4 and Edsv4 virtual machine sizes feature up to 504 GiB of RAM, in addition to fast and large local SSD storage (up to 2,400 GiB). These virtual machines are ideal for memory-intensive enterprise applications and applications that benefit from low latency, high-speed local storage. You can attach Standard SSDs and Standard HDDs disk storage to the Edv4 VMs.

Ev4 and Esv4-series
These new sizes are currently under Public Preview Only — you can signup to access them here.

The Ev4 and Esv4-series are ideal for various memory-intensive enterprise applications. They run in a hyper-threaded configuration on 2nd Generation Intel® Xeon® processors and feature up to 504 GiB of RAM.

Storage Optimized
For big data, data warehousing, large transactional databases, SQL, and NoSQL databases, storage optimized VMs are the best type for their high disk throughput and IO.

Lsv2-series
Lsv2-series VMs provide high throughput, low latency, directly mapped local NVMe making it these VMs ideal for NoSQL stores such as Apache Cassandra and MongoDB. The Lsv2-series comes in sizes 8 to 80 vCPU and each vCPU has 8 GiB of memory. VMs in this series are optimized and use the local disk on the node that is attached directly to the VM.

GPU
GPU VM types, specialized with single or multiple NVIDIA GPUs, work best for video editing and heavy graphics rendering — as in compute-intensive, graphics-intensive, and visualization workloads.

NC, NCv2 and NCv3-series
The sizes in these series are optimized for compute-intensive and network-intensive applications and algorithms. The NCv2-series is powered by NVIDIA Tesla P100 GPUs and provides more than double the computational performance of the NC-series. The NCv3-series is powered by NVIDIA Tesla V100 GPUs and can provide 1.5x the computational performance of the NCv2-series.

NV and NVv3-series
These sizes were made and optimized for remote visualization, streaming, gaming, encoding, and VDI scenarios. These VMs are targeted for GPU accelerated graphics applications and virtual desktops where customers want to visualize their data, simulate results to view, work on CAD, or render and stream content.

ND and NDv2-series
These series are focused on training and inference scenarios for deep learning. The ND-series VMs are a new addition to the GPU family and offer excellent performance for training and inference making them ideal for Deep Learning workloads and AI. The ND-series is also enabled to fit much larger neural net models thanks to the much larger GPU memory size (24 GB).

The NDv2-series is another new addition to the GPU family and with its excellent performance, it meets the needs of the most demanding machine learning, GPU-accelerated AI, HPC workloads, and simulation.

NVv4-series
The NVv4-series VMs are optimized and designed for remote visualization and VDI. With partitioned GPUs, NVv4 offers the right size for workloads requiring smaller GPU resources. With separated GPUs, this series offers the perfect size VMs for workloads that require smaller GPU resources.

High-Performance Compute
For the fastest and most powerful virtual machines, high performance computing is the best choice with optional high-throughput network interfaces (RDMA).

H-series
The H-series VMs were built for handling batch workloads, analytics, molecular modeling, and fluid dynamics. These 8 or 16 vCPU VMs are built on the Intel Haswell E5–2667 v3 processor technology and up to 14 GB of RAM per CPU core, and no hyperthreading.

Besides sizable CPU power, the H-series provides options for low latency RDMA networking with FDR InfiniBand and different memory configurations for supporting memory-intensive computing requirements.

HB-series
Applications driven by memory bandwidth, such as explicit finite element analysis, fluid dynamics, and weather modeling are the best fit for HB-series VMs. These VMs feature 4 GB of RAM per CPU core and no simultaneous multithreading.

HC-series
For applications driven by dense computation, like implicit finite element analysis, molecular dynamics, and computational chemistry HC-series VMs are the best fit. HC VMs feature 8 GB of RAM per CPU core, and no hyperthreading.

HBv2-series
Similar to other VMs in the High Performance compute family, HBv2-series VMs are optimized for applications driven by memory bandwidth, such as fluid dynamics, finite element analysis, and reservoir simulation. HBv2 VMs feature 4 GB of RAM per CPU core, and no simultaneous multithreading. These VMs enhance application performance, scalability, and consistency.

What Azure VM type is right for your workload?
The good news is that with this many options VM types, you’re bound to find the right type to meet your computing needs — as long as you know what those needs are. With good insight into your workload, usage trends, and business needs, you’ll be able to find the Azure VM type that’s right for your workloads.

Originally published at www.parkmycloud.com on June 19, 2020.

