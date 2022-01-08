---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

## Sparsity-aware Deep Learning Accelerator (in progress)
This project focuses on improving the performance and energy-efficiency for the general-purpose deep learning accelerators. The proposed schemes leverage the bit-level sparsity parallelism and eliminiate the unnecessary operations at the more fine-grained bit level. <img src="/images/bitlet.png" align="left" width="360" hspace="8" vspace="5" />We are prototyping the design on a high-end Xilinx FPGA for now. <span style="color:#953734;">**This project is in progress**</span>, collaborated with Prof. Mingzhe Zhang (IIE, CAS) and Prof. Liang Chang (UESTC), and is Partially funded by NSFC (No. 62172387, 62002339 and 62104025), the Strategic Priority Research Program of the Chinese Academy of Sciences (No. XDB44030200), the NSAF (No. U2030204) and the Key Research Program of State Key Laboratory of Computer Architecture (No. CARCH5301 and CARCH4506). We have published 3 papers regarding this project **<span style="color:#953734;">\[</span>[<span style="color:#953734;">TCAD'20</span>](/files/TETRIS-TCAD.pdf)<span style="color:#953734;">\]</span><span style="color:#953734;">\[[<span style="color:#953734;">ICPP'21</span>](/files/bitX-ICPP21.pdf)</span><span style="color:#953734;">\]</span><span style="color:#953734;">\[</span>[<span style="color:#953734;">MICRO'21</span>](/files/bitlet-MICRO21.pdf)<span style="color:#953734;">\]</span>**.<br>

## 视频画质增强 (in progress)
**This project is collaborated with <span style="color:#953734;">Guangdong OPPO Mobile Telecommunications Corp., Ltd <img src='/images/oppo.jpg' height=25 width=50></span>**<br>
随着移动通信技术的高速发展和手机娱乐时代的来临，手游，视频应用遍布人类使用手机生活的方方面面，视频的内容和质量也越来越受到手机用户的关注，其中帧率、分辨率和码率是影响视频质量的height="200" width="200"最主要因素。高分辨率的视频能提供更多的细节、更清晰的画面和更好的观看体验，因此提升视频分辨率，对于提升视频质量和用户体验有很大的帮助。
<br>根据oppo公司对手机显示效果的迫切需求，这个project研究基于深度学习的图像增强技术，通过软硬件结合的方法提高图像或视频帧的分辨率，并保证帧率。通过一系列低质量图像获取到高质量图像的增强过程，增加游戏视频的表现力，提升用户体验。我们力求使用超分辨率等图像增强技术，充分利用视频前后帧的相关性、帧内内容的自相似性，重构出分辨率更高的超分辨率视频图像，使获得的图像在物理分辨率、视觉效果及客观评价指标上均超过原始视频源，使oppo手机用户在2K屏上获得更高清的观看体验。

<video width="640" height="480" controls autoplay muted>  
    <source src="/videos/football.mp4" type="video/mp4">
</video>
<video width="640" height="480" controls autoplay muted>  
    <source src="/videos/bbjx.mp4" type="video/mp4">
</video>

## 超微空中机器人
设计“世界最小”的空中机器人并将神经网络模型以无人机为载体进行部署，实现人工智能赋能终端设备以及未来智能空中机器人“swarm”。超微空中机器人可用于单兵作战、反狙击手、战场侦查、定点打击、特工隐秘侦查等实战场景。我们设计了无人机原理图、硬件SoC和视觉定位模块，可以在室内无GPS的情况下辅助空中机器人实现精准定点，悬停精度误差小于15cm。我们还设计了一个高精度室内定位系统：使用UWB技术实现机器人“指哪飞哪”，定位精度误差小于5cm。<br>

<img src='/images/drone.jpg'>