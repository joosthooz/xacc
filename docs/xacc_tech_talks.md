# XACC Tech Talk series

The talks will be hosted as Zoom webinars and are free to attend. The format for each session will be two 30-minute talks on topics related to Adaptive Compute. 

If you would like to present your work at an XACC Tech Talk, please contact [xup@xilinx.com](xup@xilinx.com) with an outline of your proposal. 

## XACC Tech Talk 2

24 June 2021, 17:00-18:00 (CET/GMT+2)

 ![](./images/zoom_30.png)   Register for the [XACC Tech Talk 2 Zoom webinar](https://xilinx.zoom.us/webinar/register/WN_Ahay1EpVRTenPFxskNxdFQ)

### VNx and EasyNet

Dr. Mario Ruiz, Xilinx University Program; Zhenhao He, Doctoral Student, Systems Group, ETH Zurich 

This presentation will introduce *VNx* which adds 100Gbps UDP/IP support to Vitis designs. *EasyNet* extends VNx to support 100Gbps TCP/IP from HLS. 
Both VNx and EasyNet are open-source and supported from Vitis and can be used to add high-speed networking interfaces to Alveo platforms. 

Vnx: https://github.com/Xilinx/xup_vitis_network_example

EasyNet: https://github.com/fpgasystems/Vitis_with_100Gbps_TCP-IP


### Elastic-DF: Scaling Performance of DNN Inference in FPGA Clouds through Automatic Partitioning

Dr. Lucian Petrica, Xilinx Research Labs 

Customized compute acceleration in the datacenter is key to the wider roll-out of applications based on deep neural network (DNN) inference.

In this presentation we discuss how to maximize the performance and scalability of FPGA-based pipeline dataflow DNN inference accelerators (DFAs) automatically on computing infrastructures consisting of multi-die, network-connected FPGAs. We present *Elastic-DF*, a novel resource partitioning tool which integrates with the [DNN compiler FINN](https://github.com/Xilinx/finn) and utilizes 100Gbps Ethernet FPGA infrastructure, to achieve low-latency model-parallel inference without host involvement. Elastic-DF was applied to popular image classifiers ResNet50 and MobileNetV1 at XACC and provides significant throughput increase with no adverse impact on latency.


# Past talks

## XACC Tech Talk 1: Coyote and DaCe

10 June 2021


 [![](./images/youtube_social_circle_white.png)](https://www.youtube.com/watch?v=un7wck0IkGs)  View the recording [XACC Tech Talk 1 recording](https://www.youtube.com/watch?v=un7wck0IkGs)

### Coyote: Do OS abstractions make sense in FPGAs?

Dario Korolija, Doctoral Student, Systems Group, ETH Zurich

Hybrid computing systems, consisting of a CPU server coupled with a Field-Programmable Gate Array (FPGA) for application acceleration, are today a common facility in datacenters and clouds. FPGAs can deliver tremendous improvements in performance and energy efficiency for a range or workloads, but development and deployment of FPGA-based applications remains cumbersome, leading to recent work which replicates subsets of the traditional OS execution environment (virtual memory, processes, etc.) on the FPGA.

We ask a different question: to what extent do traditional OS abstractions make sense in the context of an FPGA as part of a hybrid system, particularly when taken as a complete package, as they would be in an OS? To answer this, we built and evaluated *Coyote*, an open source, portable, configurable “shell” for FPGAs which provides a full suite of OS abstractions, working with the host OS. Coyote supports secure spatial and temporal multiplexing of the FPGA between tenants, virtual memory, communication, and memory management inside a uniform execution environment. The overhead of Coyote is small and the performance benefit is significant, but more importantly it allows us to reflect on whether importing OS abstractions wholesale to FPGAs is the best way forward.

Coyote: [https://github.com/fpgasystems/Coyote](https://github.com/fpgasystems/Coyote)

### Data-Centric FPGA Programming with Multi-Level Design

Johannes de Fine Licht, Doctoral Student, Scalable Parallel Computing Laboratory, ETH Zurich

Although high-level synthesis (HLS) tools have significantly improved programmer productivity over hardware description languages, developing for FPGAs remains tedious and error prone. Programmers must learn and implement a large set of vendor-specific syntax, patterns, and tricks to optimize (or even successfully compile) their applications, while dealing with ever-changing toolflows from the FPGA vendors. We propose a new way to develop, optimize, and compile FPGA programs. The Data-Centric parallel programming (*DaCe*) framework allows applications to be defined by their dataflow and control flow through the Stateful DataFlow multiGraph (SDFG) representation, capturing the abstract program characteristics, and exposing a plethora of optimization opportunities. SDFGs are extended by multi-level library nodes, which incorporate both domain-specific and platform-specific optimizations into the design flow, enabling knowledge transfer across application domains and FPGA vendors. We show how the powerful code-generating backend of DaCe emits efficient HLS code that is structured and annotated to implement the desired architectures and achieve high performance in practice.

DaCe: [https://github.com/spcl/dace](https://github.com/spcl/dace)




---------------------------------------
<p align="center">Copyright&copy; 2021 Xilinx</p>