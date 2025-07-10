---
permalink: /
title: "Hang Lu"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<p style="text-align:justify; text-justify:inter-ideograph;">
Hang Lu is currently an Associate Professor and Master Tutor with the State Key Laboratory of Processors, Institute of Computing Technology (ICT), Chinese Academy of Sciences (CAS). He is a member of the Youth Innovation Promotion Association of CAS, and the New Best Star of ICT. He is also serving as the guest master supervisor with ShanghaiTech University and University of Electronic Science and Technology of China (UESTC). He is an Associate Professor with the Zhongguancun Laboratory. He received the BS degree and MS degree of Beihang University (major: Electronic and Information Engineering) at 2008 and 2011 respectively, and received the Ph.d of the University of Chinese Acedemy of Sciences (major: Computer Architecture). </p>
<p style="text-align:justify; text-justify:inter-ideograph;">
His research interest is Homomorphic Processing Unit (HPU), which is an emerging and cutting-edge research area regarding the software/hardware co-design for the fully homomorphic encryption (FHE). He and his teammates have developed the high-performance HPUs - ZhangJiang No.1, and Yangtse, the FHE computing library – Poseidon, the communication-and-computation co-optimized Privacy Set Intersection (PSI) based on FHE, Trusted Execution Environment (TEE) for RISC-V, etc. The researches have been published on various international leading conferences and journals like MICRO、HPCA、DAC、ICCAD、TCAD、TVLSI、ICPP、ICCD、ASPDAC, and awarded as the best paper candidate once. He owns 8 PCTs, authorized by China, USA, EU, Japan, South Korea. Within the past 10 years, he directly presides or participates multiple NSFC projects as well as the collaborative projects with Huawei and OPPO. Besides, he has published one monograph and one translation respectively, and serves as the young associate editor (JCST), reviewer and session chair of many top conferences in his research area. He was awarded by CAS and ICT as Ph.d candidate as well.</p>
<p style="text-align:justify; text-justify:inter-ideograph;">
<b>路航，现任中国科学院计算技术研究所处理器芯片全国重点实验室副研究员、硕士生导师，中国科学院青年创新促进会成员，计算所新百星，上海科技大学合作硕士生导师，电子科技大学客座研究生导师，中关村实验室副研究员。</b>路航分别于2008年和2011年获得北京航空航天大学工学学士和工学硕士学位（专业：电子信息工程），2015年获得中国科学院大学工学博士学位（中国科学院计算技术研究所，专业：计算机系统结构）。</p>
<p style="text-align:justify; text-justify:inter-ideograph;">
<b>路航的主要研究方向为全同态处理器（HPU），涉及针对全同态加密（FHE）软硬件协同设计关键技术的新兴和前沿研究领域。</b>路航带领团队研发出多款高性能HPU——<b>“张江壹号”</b>和<b>“扬子江”</b>、全同态计算库——<b>Poseidon</b>、基于FHE的通信和计算优化的隐私求交（PSI）、面向RISC-V的全国产可信执行环境（TEE）等。相关研究成果发表在MICRO、HPCA、DAC、ICCAD、TCAD、TVLSI、ICPP、ICCD、ASPDAC等领域内国际权威期刊和会议，并获最佳论文奖提名1次。路航拥有8项“国际发明专利”，授权国家包括中国、美国、欧盟、日本、韩国。近十年来，路航负责或参与多项国家自然科学基金项目以及华为、oppo等企事业单位合作研究项目。此外，他还出版1部专著和1部译著，担任领域内权威学术期刊JCST的青年副编辑以及国际顶级会议的审稿人和session主席。在学期间他曾获得国家奖学金提名，中国科学院“朱李月华”优秀博士生奖，中科院计算所“所长特别奖”等荣誉。</p>

## Homomorphic Processing Unit (HPU) Laboratory
<p style="text-align:justify; text-justify:inter-ideograph;">
The researches in this Lab focus on the acceleration strategies for the "Fully Homomorphic Encryption (FHE)", in the form of the Homomorphic Processing Unit (HPU). To represent its accurate definition, I intend to cite the statements from an article on the IEEE Spectrum – <a href="https://spectrum.ieee.org/homomorphic-encryption"><b>“CHIPS TO COMPUTE WITH ENCRYPTED DATA ARE COMING. Fully homomorphic encryption could make data unhackable”</b></a>. It says “TRUST NO ONE. It’s not just a throwaway line from TV thrillers. It’s becoming the goal of computer security, and a technology that can make it a reality has arrived. Called fully homomorphic encryption, or FHE, it allows software to compute on encrypted data without ever decrypting it. Although FHE software has made some inroads in protecting financial and health care data, it’s been held back by the fact that it can take as much as a millionfold more effort on today’s computers. But in 2024, at least six companies will be testing or even commercializing the first chips that accelerate FHE to the point where computing on encrypted data is nearly as quick as computing on unencrypted data. Computing with numbers that might require more than a hundred bits to describe is not something today’s CPUs and GPUs are inherently good at. If anything, GPUs have been going in the opposite direction, focusing on less precise math done using smaller and smaller floating-point numbers. The FHE accelerator chips, by contrast, can stream huge volumes of data through hardware that does integer math on numbers that are thousands of bits long to accommodate encryption’s precision needs. Each accelerator has its own way of dealing with these streams of huge numbers. But they’re all after the same goal — making FHE as fast as today’s unencrypted computing. The quest for hardware that can accelerate FHE got its biggest boost in 2021, when the U.S. Defense Advanced Research Projects Agency (DARPA) began a project called <a href="https://www.darpa.mil/program/data-protection-in-virtual-environments"><b>DPRIVE</b></a>. The goal was to build hardware that could radically reduce the time it took for FHE computing tasks, from weeks to just seconds or even milliseconds. Three participating teams — led by Duality Technologies, Galois, and Intel — are on track to deliver chips designed to make FHE perform within a factor of 10 of traditional computing or even better in 2024.”</p>
<p style="text-align:justify; text-justify:inter-ideograph;">
<b>We consider this hot topic from both the software and hardware perspective, and seek to find an appropriate way to <span style="color:#953734;">design the HPUs to serve the intelligent and secure systems</span>. Our research interests include:</b></p>

  * **Homomorphic Processing Unit (HPU),** including HPU micro-architecture design on FPGA and ASIC, specialized FHE library (Poseidon), driver and runtime development for the HPU. 
  * **Complier for HPU,** we are designing a highly optimized compiler for HPU, termed as Apollo. 
  * **TEE for RISC-V,**  for constructing the highly scalable, high security and high performance TEE on XiangShan RISC-V cores. 
  * **Software Framework & User Application Development,** for integrating the HPU technology stack (“张江壹号” and “扬子江”, Poseidon, Apollo) with the mainstream privacy computing frameworks (i.e. SecretFlow, Primihub, etc.) and developing privacy enhanced applications based on FHE (i.e. PSI, PIR, secure deep learning, federated learning, etc.) and their deployment on the HPU.

## Services
* 2025.7, IEEE International Symposium on High-Performance Computer Architecture (HPCA), Program Committee <img src='/images/HPCA2026_logo.png' height=30 width=146>
* 2025.6, IEEE Transactions on Information Forensics and Security (TIFS), Reviewer <img src='/images/TIFS.jpg' height=30 width=146>
* 2025.3, the 58th IEEE/ACM International Symposium on Microarchitecture (MICRO), Program Committee <img src='/images/micro-red.png' height=30 width=37>
* 2024.11, the 52nd International Symposium on Computer Architecture (ISCA), Program Committee <img src='/images/ISCA_2025.png' height=30 width=49>
* 2024.11, IEEE Transactions on Computers (TC), Reviewer <img src='/images/TC.png' height=30 width=81>
* 2024.7，CCF Chip 2024，中国计算机学会芯片大会，组委会 <img src='/images/ccfchip2024-logo.png' height=22 width=126>
* 2024.5, IEEE Transactions on Circuits and Systems I (TCAS-I), Reviewer <img src='/images/TCAS-I.jpg' height=35 width=28>
* 2023.12, IEEE Transactions on Very Large Scale Integration Systems (TVLSI), Reviewer <img src='/images/TVLSI.jpg' height=35 width=26>
* 2023.11，隐私计算全球发展报告，编委 **<span style="color:#953734;">\[</span>[<span style="color:#953734;">PDF</span>](/files/《2023全球隐私计算报告》.pdf)<span style="color:#953734;">\]</span>** <img src='/images/mpcLogo.png' height=37 width=120>
* 2023.11, the 51st International Symposium on Computer Architecture (ISCA), External Review Committee <img src='/images/ISCA_2024_v2.png' height=30 width=49>
* 2023.8, IEEE Transactions on Circuits and Systems II (TCAS-II), Reviewer <img src='/images/TCAS-II.png' height=22 width=81>
* 2023.8，中国科学院青年创新促进会信息与管理分会2023年学术年会，网络计算与信息安全论坛，演讲嘉宾，演讲题目——“全同态处理器和算子库的设计探索” <img src='/images/CAS.webp' height=35 width=35> <img src='/images/youth.png' height=34 width=34>
* 2023.8，CCFSys 2023，隐私计算软硬协同加速技术论坛，论坛主席&演讲嘉宾，演讲题目——“全同态处理器和算子库的设计探索” **<span style="color:#953734;">\[</span>[<span style="color:#953734;">PDF</span>](/files/CCFSys2023-HANGLU.pdf)<span style="color:#953734;">\]</span>** <img src='/images/ccfsys_logo.jpg' height=22 width=120>
* 2022.12，受邀参加新浪2022科技风云榜年度盛典，并做报告——[**“数字经济中的隐私计算技术与芯片”**](https://finance.sina.cn/tech/2022-12-16/detail-imxwwaqr1918441.d.html) <img src='/images/sinatech.jfif' height=35 width=35>
* 2022.12，HPC China 2022，第二届超大规模HPC系统研制论坛，演讲嘉宾，演讲题目——“领域应用的定制化硬件加速方法” **<span style="color:#953734;">\[</span>[<span style="color:#953734;">PDF</span>](/files/HPCChina2022-HANGLU.pdf)<span style="color:#953734;">\]</span>** <img src='/images/hpcchina2022logo.png' height=30 width=60>
* 2022.11，受邀参加OPPO TALK，并做报告——“重塑计算系统——服务于深度学习和隐私保护计算的软硬件协同设计方法” <img src='/images/oppo.jpg' height=25 width=50>
* 2022.06，受邀在《中国计算机学会通讯》(CCCF)第18卷第6期发表文章——“MICRO 2021——拥抱更广阔的未来” **<span style="color:#953734;">\[</span>[<span style="color:#953734;">PDF</span>](/files/MICRO-CCCF-LU.pdf)<span style="color:#953734;">\]</span>** <img src='/images/CCF.png' height=30 width=41>
* 2022.01，华为诺亚方舟实验室访问，演讲题目——“Re-architecting the Computation System for Deep Learning Applications: software and hardware approach” <img src='/images/noahark.jfif' height=30 width=115>
* 2022.01，第4届计算机体系结构国家重点实验室前沿高峰论坛，演讲嘉宾，演讲题目——“端侧视频画质增强的软硬件设计方法研究” **<span style="color:#953734;">\[</span>[<span style="color:#953734;">PDF</span>](/files/carch_summit22.pdf)<span style="color:#953734;">\]</span>** <img src='/images/carch_submit2022.png' height=23 width=54>
* 2021.12, the 20th ACM SIGOPS ChinaSys, session speaker, title: "Distilling Bit-level Sparsity Parallelism for General Purpose Deep Learning Acceleration" **<span style="color:#953734;">\[</span>[<span style="color:#953734;">PDF</span>](/files/bitlet-chinasys-v3.pdf)<span style="color:#953734;">\]</span>** <img src='/images/chinasys2021.png' height=27 width=148>
* 2020，第57届国际设计自动化会议DAC（CCF A类）程序委员会，审稿人
* 2019，第56届国际设计自动化会议DAC（CCF A类）程序委员会，审稿人
* 2019，IEEE网络、体系结构与存储国际会议（NAS）组委会，session主席
* 2019，IEEE网络、体系结构与存储国际会议（NAS）程序委员会，审稿人

## Recruiting （招生）
<p style="text-align:justify; text-justify:inter-ideograph;"><b>我们都非常年轻，有激情，是个充满活力的团队！</b>大家来自五湖四海有缘相聚在一起，为共同的事业努力，一起学习共同进步。</p>
<p style="text-align:justify; text-justify:inter-ideograph;"><b>很多同学不清楚HPU是什么，这是一个冉冉升起的新型领域专用处理器！</b>一些大厂例如华为、蚂蚁集团、各大云服务提供商都在试图通过全同态加密以及可信执行环境的方式保护敏感数据安全，让数据直接在密态下进行计算（不暴露明文），而我们要做的就是用专用处理器加速这一过程。我们研究从硬件架构设计==>算子库==>编译器==>框架==>应用程序的整个链条，取得了国内外瞩目的学术成果并研制出两款商用HPU系统原型。我们也和蚂蚁集团、华为、飞腾、亚信等头部企业建立了广泛合作，in other words，从事这个领域的研究，你就业能去大厂！</p>
<p style="text-align:justify; text-justify:inter-ideograph;"><b>我们还在中关村实验室的支持下大力推进HPU的学术研究和工程研制。</b>我的学生全部以“访问学生”身份在中关村实验室开展工作，每月除计算所发放的基本RA外，还可额外领取中关村实验室发放的5000+RMB的研究补助，三餐自助且免费！你读研期间会过得很爽！</p>
<p style="text-align:justify; text-justify:inter-ideograph;"><b>我团队有6名博士，优秀的硕士生可以在第二或第三学年转博。</b>其他信息请去我主页projects、life和feats页面详细了解。我每年只有1个保研名额，提前联系会更有优势。</p>
<p style="text-align:justify; text-justify:inter-ideograph;"><b>我们希望你（包括但不局限于）：</b>出身于电子工程或者计算机科学与技术相关专业，有一定的动手能力，最好参加过处理器设计相关项目如<span style="color:#953734;"><b>“一生一芯”，“龙芯杯”</b></span>或FPGA设计相关比赛如<span style="color:#953734;"><b>CCF/Xilinx定制计算大赛（CCC）</b></span>或隐私计算相关比赛如<span style="color:#953734;"><b>国际隐私计算大赛（iDASH），隐私计算Hackathon，“星河杯”隐私计算大赛</b></span>并拿到过名次（以上非硬性要求）。</p>
<!--<p style="text-align:justify; text-justify:inter-ideograph;"><span style="color:#953734;"><b>我还有1个2024年“考研”招生名额（明年我在暑期班或者九推就会用掉名额），欢迎优秀的你联系我！</b></span><img src='/images/onshore.jpg' height=70 width=120></p>-->

**Other useful links:**<br>
[**中国科学院大学个人主页**](https://people.ucas.edu.cn/~luhang)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[**中国科学院计算技术研究所个人主页**](http://www.ict.ac.cn/sourcedb/cn/jssrck/201912/t20191210_5451510.html)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
[**上海科技大学信息科学与技术学院**](https://sist.shanghaitech.edu.cn/)<br>

[**中国科学院计算技术研究所2025年“计算未来”全国大学生暑期研修班招生简章**](http://www.ict.ac.cn/xwgg/tzgg/202506/t20250630_7876973.html)已经公布，暑期班期间的推免生面试时间预计在8月11日左右，具体形式为线下面试。<br>

<img src='/images/HPU-lab-BJ.jpg'><br>
<img src='/images/HPU-lab-SH.jpg'><br><br>
**We need you here and welcome on board!**