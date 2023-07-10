---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

## 全同态处理器 (in progress)
**This project is sponsored by <span style="color:#953734;">CCF-Huawei Populus Grove Fund（CCF-华为胡杨林基金）<img src='/images/huawei.jpg' height=35 width=35></span>**<br>
<img src="/images/HPU.png" align="left" width="360" hspace="9" vspace="5" />同态加密计算技术作为一种新型数据安全计算技术，受到了越来越多的关注。首先，同态加密技术可以降低计算供应商数据安全方面的成本。由于同态加密技术允许应用对密文数据直接进行计算，算力提供方无需接触明文数据，即使发生数据泄露，难以给用户造成重大损失。这一特性降低了算力提供方在用户数据安全方面的压力，可以帮助云计算供应商显著降低数据安全维护方面的运营成本。第二，同态加密技术可以吸引更多用户将数据和计算迁移至云端，降低用户的计算成本。由于同态加密计算技术可以直接对密文数据进行处理，算力提供方无需对加密数据进行解密，这将从根本上解决由于数据所有方与算力提供方分离所导致的数据安全风险问题。<img src="/images/poseidon.jfif" align="right" width="127" hspace="9" vspace="5" />
**虽然同态加密在隐私计算领域有着重要的作用，但是巨大的计算开销阻碍了它的实际应用。如何在保证密文计算结果正确性的前提下，提高计算性能和能效是当前业界公认的难题。**本项目拟通过软硬件协同设计和优化方法，对同态加密进行计算加速，并设计专用加速器原型系统提高其计算性能**（命名为“Poseidon”，波塞冬）**。<span style="color:#953734;">**This project is in progress,**</span> and we have published 2 papers regarding this project **<span style="color:#953734;">\[</span>[<span style="color:#953734;">HPCA'23</span>](/files/Poseidon-HPCA2023.pdf)<span style="color:#953734;">\]</span><span style="color:#953734;">\[</span>[<span style="color:#953734;">TCAD'23</span>](/files/Poseidon-NDP-TCAD2023.pdf)<span style="color:#953734;">\]</span>**.<br>
**商用版全同态处理器加速卡产品<span style="color:#953734;">“张江壹号”</span>已经成功部署到[原语科技](https://primihub.com/#/home)隐私计算一体机<img src='/images/primihub.png' height=30 width=70>**<br>
<img src="/images/ZJ-1.png" align="left" />
<video width="981" height="601" controls autoplay muted>  
    <source src="/videos/primihub_machine.mp4" type="video/mp4">
</video>

## Sparsity-aware Deep Learning Accelerator (in progress)
**This project is also collaborated with <span style="color:#953734;">Huawei Technologies Co., Ltd <img src='/images/huawei.jpg' height=35 width=35></span>**<br>
This project focuses on improving the performance and energy-efficiency for the general-purpose deep learning accelerators. The proposed schemes leverage the bit-level sparsity parallelism and eliminiate the unnecessary operations at the more fine-grained bit level. <img src="/images/bitlet.png" align="left" width="360" hspace="8" vspace="5" />We are prototyping the design on a high-end Xilinx FPGA for now. <span style="color:#953734;">**This project is in progress.**</span> We have published 3 papers regarding this project **<span style="color:#953734;">\[</span>[<span style="color:#953734;">TCAD'20</span>](/files/TETRIS-TCAD.pdf)<span style="color:#953734;">\]</span><span style="color:#953734;">\[[<span style="color:#953734;">ICPP'21</span>](/files/bitX-ICPP21.pdf)</span><span style="color:#953734;">\]</span><span style="color:#953734;">\[</span>[<span style="color:#953734;">MICRO'21</span>](/files/bitlet-MICRO21.pdf)<span style="color:#953734;">\]</span>**.<br>
我们正在打造一款异构AI加速系统**（命名为“bitlet”）**，CPU部分使用RISC-V开源处理器及其配套的敏捷开发工具。通过扩展RISC-V指令集，使用ROCC与AI加速部分连接。整个工程采用高端FPGA作为硬件平台，力求使AI性能相对于基线提高2\~3倍。
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