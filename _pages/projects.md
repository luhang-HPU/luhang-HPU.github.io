---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

## 全同态处理器 (in progress)
**This project is sponsored by <span style="color:#953734;">CCF-Huawei Populus Grove Fund（CCF-华为胡杨林基金）<img src='/images/huawei.jpg' height=35 width=35></span> and <span style="color:#953734;">CCF-Ant Research Fund（CCF-蚂蚁基金）<img src='/images/ant_group_logo.jpg' height=35 width=108></span> and <span style="color:#953734;">CCF-Phytium Fund（CCF-飞腾基金）<img src='/images/phytium_logo.png' height=35 width=195></span>**<br>
**This project is also sponsored by <span style="color:#953734;">Zhongguancun Laboratory（中关村实验室）<img src='/images/ZGC_logo.jpg' height=35 width=35></span>**<br>
<img src="/images/HPU.png" align="left" width="360" hspace="9" vspace="5" /><b>全同态加密（Fully Homomorphic Encryption, 简称“FHE”）</b>作为一种新型数据安全计算技术，受到了越来越多的关注。首先，全同态加密可以降低算力提供方在数据安全方面的运维成本。由于全同态加密允许应用对密文数据直接进行计算，算力提供方无需接触明文数据，即使发生数据泄露，难以给用户造成重大损失。第二，全同态加密可以吸引更多用户将数据和计算迁移至云端，降低用户的算力成本，并从根本上解决由于数据所有方与算力提供方分离所导致的数据安全风险问题。<b>虽然全同态加密在数据安全领域有着重要的作用，但是巨大的计算开销阻碍了它的实际应用。如何在保证密文计算结果正确性的前提下，提高计算性能和能效是当前业界公认的难题。</b><img src="/images/poseidon.jfif" align="right" width="127" hspace="9" vspace="5" />本项目拟通过软硬件协同设计和优化方法，构建<b>全同态处理器（HPU）</b>提高其计算性能。我们已经研制出两代HPU原型：第一代 - <b>“张江壹号”</b>，第二代 - <b>“扬子江”</b>。<br>
**<span style="color:#953734;">“张江壹号”</span>已经成功部署到[原语科技](https://primihub.com/#/home)隐私计算一体机 <img src='/images/primihub.png' height=30 width=70>**<br>
**我们开发了适配HPU的全同态计算库，请见[Poseidon在线文档](https://poseidon-hpu.rtfd.io/) <img src='/images/poseidon-logo.jpg' height=70 width=70>**<br>
<img src="/images/ZJ-1.png" align="left" />
<video width="981" height="601" controls autoplay muted>  
    <source src="/videos/primihub_machine.mp4" type="video/mp4">
</video><br>
<img src="/images/信江HPU.png" align="left" width="360" hspace="9" vspace="5" /><b>第三代“信江”架构是我们团队在全同态处理器方向的最新成果，定位为一款面向FHE的专用ASIC芯片。</b>与前代基于FPGA的原型系统相比，“信江”在架构层面实现了全面升级，致力于在大规模密态计算场景下提供更高的能效与性能。<br>
“信江”采用12nm工艺制程，以国产开源RISC-V处理器“香山”南湖架构为核心，<b>通过FHE专用指令扩展（包括计算指令、访存指令与控制指令），实现了软硬件协同的密态计算加速。</b>在微架构设计上，它支持CKKS、BFV、TFHE等多种主流全同态加密方案，核心计算单元针对数论变换（NTT）、自同构（Automorphism）等全同态加密关键算子进行了深度定制与流水线优化。同时，“信江”延续了多项式级指令集与多项式粒度内存管理单元的协同设计与存储架构，通过专用指令与硬件定制相结合，有效减少了大规模密态计算中的非必要数据搬移。<br>
“信江”具有广阔的应用前景，可广泛应用于金融、政务、医疗等数据高度敏感领域的隐私保护计算场景，为这些行业在数据共享与联合建模过程中提供安全的密态计算能力。

## TEE for RISC-V (in progress)
**This project is sponsored by <span style="color:#953734;">Zhongguancun Laboratory（中关村实验室）<img src='/images/ZGC_logo.jpg' height=35 width=35></span>**<br>
<img src="/images/TEE.jpg" align="left" width="480" hspace="9" vspace="5" /><b>可信执行环境（TEE）是一种具有运算和储存功能，能提供安全性和完整性保护的独立处理环境。</b>其基本思想是：在硬件中为敏感数据单独分配一块隔离的内存，所有敏感数据的计算均在这块内存中进行，除了经过授权的接口外，应用程序不能访问这块隔离内存中的信息，以此来实现敏感数据的隐私计算。TEE能够保护运行在其中的代码和数据免受外部攻击，包括来自操作系统、硬件和其他应用程序的攻击。TEE的用途非常广泛，例如提供安全的支付环境，保证支付过程中的安全性和隐私性，Apple Pay等移动支付服务就使用了TEE技术。TEE还可以提供安全的身份验证环境，防止身份被盗用或伪造，例如银行使用TEE技术来保护客户的账户安全。
<b>我们团队研制了一款基于RISC-V架构的全国产可信执行环境，已完成芯片流片验证，命名为“翠湖”处理器。</b>该处理器以国产开源RISC-V处理器“香山”南湖架构为核心，在兼容RISC-V标准指令集的基础上，进行了面向可信执行环境的安全增强设计。芯片采用28nm工艺制程，主频达到1.5GHz，SPEC2006跑分达到9.6分/GHz，整体性能对标ARM Cortex-A76。<br>
<video width="981" height="601" controls autoplay muted>  
    <source src="/videos/翠湖.mp4" type="video/mp4">
</video><br>
在安全架构方面，处理器基于蓬莱（Penglai）可信执行环境框架，构建了多层次硬件安全防护体系：通过PMP（物理内存保护）与SPMP（S模式物理内存保护）实现CPU侧内存资源的细粒度隔离与访问控制；同时引入IOPMP（I/O物理内存保护）机制，对外设DMA访问内存进行严格检查，有效防御恶意外设发起的物理内存攻击与DMA攻击。在中断管理方面，处理器引入专用的安全中断机制，通过新增CSR（控制状态寄存器） 对中断来源进行安全世界与非安全世界的标注与路由，确保安全飞地的实时响应不受非安全世界中断干扰，进一步增强了系统的确定性与安全性。三重硬件保护机制与安全中断路由协同工作，为每个安全飞地（Enclave）提供从CPU到外设的全路径安全隔离。<b>芯片最高可同时启动256个安全飞地，每个飞地均可独立运行敏感计算任务，互不干扰，</b>为多租户机密计算场景提供了坚实的硬件级隔离基础。<br>
<video width="981" height="601" controls autoplay muted>  
    <source src="/videos/翠湖TEE.mp4" type="video/mp4">
</video><br>
<b>在软件层面，团队自主研发了TEEOS（可信执行环境操作系统）</b>，运行于安全飞地之上，负责飞地的生命周期管理、安全服务调度、密钥管理等核心功能，为上层应用提供标准化的安全服务接口，进一步丰富了可信执行环境的软件生态。
<b>该处理器已成功流片并完成硅后验证</b>，功能与性能均达到设计预期，可为政务数据、金融数据、医疗数据等敏感信息处理场景提供全国产、高性能、高安全的可信执行环境解决方案。
<!--
## Sparsity-aware Deep Learning Accelerator (in progress)
**This project is also collaborated with <span style="color:#953734;">Huawei Technologies Co., Ltd <img src='/images/huawei.jpg' height=35 width=35></span>**<br>
This project focuses on improving the performance and energy-efficiency for the general-purpose deep learning accelerators. The proposed schemes leverage the bit-level sparsity parallelism and eliminiate the unnecessary operations at the more fine-grained bit level. <img src="/images/bitlet.png" align="left" width="360" hspace="8" vspace="5" />We are prototyping the design on a high-end Xilinx FPGA for now. <span style="color:#953734;">**This project is in progress.**</span> We have published 3 papers regarding this project **<span style="color:#953734;">\[</span>[<span style="color:#953734;">TCAD'20</span>](/files/TETRIS-TCAD.pdf)<span style="color:#953734;">\]</span><span style="color:#953734;">\[[<span style="color:#953734;">ICPP'21</span>](/files/bitX-ICPP21.pdf)</span><span style="color:#953734;">\]</span><span style="color:#953734;">\[</span>[<span style="color:#953734;">MICRO'21</span>](/files/bitlet-MICRO21.pdf)<span style="color:#953734;">\]</span>**.<br>
我们正在打造一款异构AI加速系统（命名为<b>“bitlet”</b>），CPU部分使用RISC-V开源处理器及其配套的敏捷开发工具。通过扩展RISC-V指令集，使用ROCC与AI加速部分连接。整个工程采用高端FPGA作为硬件平台，力求使AI性能相对于基线提高2\~3倍。


<br><br><br>

## 视频画质增强
**This project is collaborated with <span style="color:#953734;">Guangdong OPPO Mobile Telecommunications Corp., Ltd <img src='/images/oppo.jpg' height=25 width=50></span>**<br>
随着移动通信技术的高速发展和手机娱乐时代的来临，手游，视频应用遍布人类使用手机生活的方方面面，视频的内容和质量也越来越受到手机用户的关注，其中帧率、分辨率和码率是影响视频质量的height="200" width="200"最主要因素。高分辨率的视频能提供更多的细节、更清晰的画面和更好的观看体验，因此提升视频分辨率，对于提升视频质量和用户体验有很大的帮助。
<br>根据oppo公司对手机显示效果的迫切需求，这个project研究基于深度学习的图像增强技术，通过软硬件结合的方法提高图像或视频帧的分辨率，并保证帧率。通过一系列低质量图像获取到高质量图像的增强过程，增加游戏视频的表现力，提升用户体验。我们力求使用超分辨率等图像增强技术，充分利用视频前后帧的相关性、帧内内容的自相似性，重构出分辨率更高的超分辨率视频图像，使获得的图像在物理分辨率、视觉效果及客观评价指标上均超过原始视频源，使oppo手机用户在2K屏上获得更高清的观看体验。<br>
**这里有高通平台的实测效果<span style="color:#953734;">\[</span>[<span style="color:#953734;">PDF</span>](/files/ISR.pdf)<span style="color:#953734;">\]</span>。**

<video width="640" height="360" controls autoplay muted>  
    <source src="/videos/system.mp4" type="video/mp4">
</video>
<video width="640" height="480" controls autoplay muted>  
    <source src="/videos/football.mp4" type="video/mp4">
</video>
<video width="640" height="480" controls autoplay muted>  
    <source src="/videos/bbjx.mp4" type="video/mp4">
</video>

## 超微空中机器人
设计“世界最小”的空中机器人并将神经网络模型以无人机为载体进行部署，实现人工智能赋能终端设备以及未来智能空中机器人“swarm”。超微空中机器人可用于单兵作战、反狙击手、战场侦查、定点打击、特工隐秘侦查等实战场景。我们设计了无人机原理图、硬件SoC和视觉定位模块，可以在室内无GPS的情况下辅助空中机器人实现精准定点，悬停精度误差小于15cm。我们还设计了一个高精度室内定位系统：使用UWB技术实现机器人“指哪飞哪”，定位精度误差小于5cm。<br>

<img src='/images/drone.jpg'>
-->