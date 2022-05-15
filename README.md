<h1 align="center">FPGA Tutorial </h1>

本项目旨在**帮助大家进行FPGA的入门，分享FPGA相关的优秀文章，优秀项目**。

[一起为本项目作出贡献](#github)

<h2 align="center">零、镜像下载</h2>

- [Vivado 多版本安装包 百度网盘](https://pan.baidu.com/s/1op98YUPNqSfqAN2UeywlNA)（提取码：DZKR）
- [Vivado License](https://github.com/LeiWang1999/FPGA/tree/master/license)
- [PetaLinux 2017.4](https://pan.baidu.com/s/1xZVsQVMPowDfQhBysLQ-1A)(提取码：rlcv)
- [pynq_rootfs-arm_v2.4-2.5](https://pan.baidu.com/s/1JFgg0Pezk0mBub8zMdcYyA)（提取码：rn0h）
- [Ubuntu-16.04.2-minimal-armhf-2017-06-18](https://pan.baidu.com/s/1mMWF8H2xEtbE5ayJ7pdGTw)(提取码：nckh)

<h2 align="center">一、入门资料</h2>

<h3>FPGA相关门户网站</h3>

- [Xilinx](https://www.xilinx.com/)
- [Xilinx Wiki](https://xilinx-wiki.atlassian.net/wiki/spaces/A/overview)
- [Xilinx Forums](https://forums.xilinx.com/)
- [Xilinx Open Hardware](http://www.openhw.org/)
- [电子创新网Xilinx社区](http://xilinx.eetrend.com/)
- [Altera](https://www.intel.cn/content/www/cn/zh/products/programmable.html)
- [Digilent 中国](http://www.digilent.com.cn/)
- [米联客](https://www.uisrc.com/portal.php)
- [opencores 开源硬件IP站](https://opencores.org/)
- [FPGA FOR FUN](https://www.fpga4fun.com/CrossClockDomain.html)
- [HDLBits](https://hdlbits.01xz.net/wiki/Main_Page)

<h3 id="github">每个人都应该会使用GitHub</h3>

- [廖雪峰的Git教程]( https://www.liaoxuefeng.com/wiki/896043488029600 )
- [Github Guides](https://guides.github.com/activities/hello-world/)
- [如何参与到本项目的建设](docs/HowContribute.md)

<h3>数字电路</h3>

数字电路是学习FPGA的前提。

如果没有学习过数字电路，先选择一本数字电路教程(下面的数字电路课本中选一本，或者用手头的数字电路课本),再选择一本Verilog教程。用Verilog实现一遍数字电路里的加法器等等，是很好的入门经历。

- [电子技术基础 数字部分 (康华光.第5版)](http://leiblog.wang/static/FPGA/books/电子技术基础.数字部分.(康华光.第5版).pdf)

<h3>Verilog HDL入门</h3>

> HDL是硬件描述语言(Hardware Design Language)，使用这门语言的时候我们像是在**建模**，这点区别于编程语言，这往往是新手首先需要绕过来的难关！
>
> Xilinx和Altera是我们主要使用到的FPGA芯片厂商，此外还有国产的紫光、安陆等。对我们用户来说，他们的区别主要在于EDA软件的不同，比如Xilinx使用的是Vivado、Altera使用的是Quatus...
>
> 我个人认为Vivado的功能最强大，最好用，但缺点在于综合、生成等步骤的速度慢，你需要一台好的电脑！
>
> 虽然对于学习Verilog来说他们没有差别，但学习FPGA的时候手上最好要有一块板卡，上板验证会有更多的成就感。所以，用什么家的板卡，就用什么软件。

- 经典图书
  - [搭建你的数字积木](https://book.douban.com/subject/30242443/)
    - Xilinx大学计划书目，比较推荐，但是没找到PDF,并且还有配套的Basys3/EGO1例程([仓库地址](https://github.com/xupsh/Digital-Design-Lab))
  - [Verilog数字系统设计教程 夏宇闻](http://leiblog.wang/static/FPGA/books/Verilog数字系统设计教程夏宇闻.pdf)
  - [Verilog经典教程 夏宇闻](http://leiblog.wang/static/FPGA/books/夏宇闻-Verilog经典教程.pdf)
  - [深入浅出FPGA](http://leiblog.wang/static/FPGA/books/深入浅出FPGA.pdf)
  - [Vivado使用误区与进阶](https://leiblog.wang/static/FPGA/books/Vivado使用误区与进阶.pdf)
  - [Xilinx应用进阶 调用IP核详解和设计开发](https://leiblog.wang/static/FPGA/books/Xilinx%20FPGA%E5%BA%94%E7%94%A8%E8%BF%9B%E9%98%B6%20%20%E9%80%9A%E7%94%A8IP%E6%A0%B8%E8%AF%A6%E8%A7%A3%E5%92%8C%E8%AE%BE%E8%AE%A1%E5%BC%80%E5%8F%91%20[%E9%BB%84%E4%B8%87%E4%BC%9F%E7%BC%96%E8%91%97][%E7%94%B5%E5%AD%90%E5%B7%A5%E4%B8%9A%E5%87%BA%E7%89%88%E7%A4%BE][2014.08][274%E9%A1%B5].pdf)
  
- 网路上生动的大神教程
  - [Artix7修炼秘籍](http://leiblog.wang/static/FPGA/books/00《Artix7修炼秘籍》-MIA701第一季.pdf)
  - [Verilog那些事儿](http://leiblog.wang/static/FPGA/books/Verilog那些事儿/)
    - [驱动篇](http://leiblog.wang/static/FPGA/books/Verilog那些事儿/02Veilog那些事儿-驱动篇I.pdf)
    - [时续篇](http://leiblog.wang/static/FPGA/books/Verilog那些事儿/03Verilog_HDL_那些事儿_时序篇v2.pdf)
    - [建模篇](http://leiblog.wang/static/FPGA/books/Verilog那些事儿/04VerilogHDL那些事儿_建模篇.pdf)
    - [整合篇](http://leiblog.wang/static/FPGA/books/Verilog那些事儿/05VerilogHDL那些事儿-整合篇.pdf)
  - [Xilinx原语的使用方法](http://leiblog.wang/static/FPGA/books/xilinx原语的使用方法.pdf)
  - [FPGA自学笔记-设计与验证](http://leiblog.wang/static/FPGA/books/FPGA自学笔记——设计与验证公开版.pdf)
  - [Verilog开发经验总结](http://leiblog.wang/static/FPGA/books/Verilog开发经验总结.pdf)
  - [猫叔的FPGA时序约束教程](https://leiblog.wang/static/FPGA/books/%E7%8C%AB%E5%8F%94%E7%9A%84FPGA%E6%97%B6%E5%BA%8F%E7%BA%A6%E6%9D%9F%E6%95%99%E7%A8%8B.pdf)
  - [Xilinx系列FPGA芯片IP核详解](https://leiblog.wang/static/FPGA/books/Xilinx%E7%B3%BB%E5%88%97FPGA%E8%8A%AF%E7%89%87IP%E6%A0%B8%E8%AF%A6%E8%A7%A3_%E5%88%98%E4%B8%9C%E5%8D%8E%E7%BC%96%E8%91%97.pdf)
  - [数字集成电路静态时序分析基础](https://www.bilibili.com/video/BV1if4y1p7Dq)
  - [综合与Design Compiler](http://leiblog.wang/static/FPGA/books/综合与DesignCompiler.pdf)
- 官方pdf文档
  - [Vivado从此开始](http://leiblog.wang/static/FPGA/books/Vivado从此开始/)
  - [Verilog HDL程序设计与实践 Xilinx大学计划](http://leiblog.wang/static/FPGA/books/VerilogHDL程序设计与实践.pdf)
- Xilinx 入门视频
  - [Digilent Basys3 手把手教学](https://space.bilibili.com/511019924/channel/detail?cid=134957)
    - 顺便学一下Vivado如何使用
  - [Vivado SDK工程移植到Vitis](https://forums.xilinx.com/t5/Xilinx-%E4%BA%A7%E5%93%81%E8%AE%BE%E8%AE%A1%E4%B8%8E%E5%8A%9F%E8%83%BD%E8%B0%83%E8%AF%95%E6%8A%80%E5%B7%A7/%E5%B0%86%E8%B5%9B%E7%81%B5%E6%80%9D-SDK-%E5%B7%A5%E7%A8%8B%E7%A7%BB%E6%A4%8D%E5%88%B0-Vitis-%E7%9A%84%E5%88%86%E6%AD%A5%E6%8C%87%E5%8D%97/ba-p/1066332)
- Altera 入门视频
  - [正点原子 FPGA教学](https://www.bilibili.com/video/BV1Mb411E7gd?from=search&seid=11737352508875302131)
    - 如果买的是正点原子家的FPGA，可以白嫖很多项目。
    - 别家的FPGA，学习语法、驱动，也是没问题的。
  - [芯航线 FPGA从零到入门](https://www.bilibili.com/video/BV1tW411v78j?from=search&seid=11737352508875302131)

<h3>飞速提升开发效率✈️</h3>

- [VsCode取代Vivado自带编辑器](https://editor.csdn.net/md/?articleId=84668833)
- [使用板卡文件自动配置环境(板卡芯片、DDR等)](https://www.bilibili.com/s/video/BV1zg4y1q7Jd)
  - [EGO1板卡文件]( https://github.com/LeiWang1999/FPGA/boards)
  - [Digilent Boards 全家桶]( https://github.com/Digilent/vivado-boards)
- [ModelSim与Matlab搭建图像仿真环境(无需上板即可验证Verilog算法!)](http://leiblog.wang/technicaldetail/5e397c7937a947e1fa893314)
- [Python实现Vivado和ModelSim仿真自动化](https://mp.weixin.qq.com/s/LvmzGJt4ywOUXO7TfyPtcg)
- [SystemVerilog与功能验证](https://leiblog.wang/static/FPGA/books/SystemVerilog%E4%B8%8E%E5%8A%9F%E8%83%BD%E9%AA%8C%E8%AF%81%C2%81.pdf)

<h3>规范你的工程🌟</h3>

- [华为verilog编程规范](http://leiblog.wang/static/FPGA/books/standard/华为verilog编程规范.pdf)
- [IEEE_Verilog](http://leiblog.wang/static/FPGA/books/standard/IEEE_Verilog.pdf)

<h3>商业报告</h3>

- [电子设备-电子行业专题报告：国产FPGA研究框架-方正证券](https://leiblog.wang/static/FPGA/books/%E7%94%B5%E5%AD%90%E8%AE%BE%E5%A4%87-%E7%94%B5%E5%AD%90%E8%A1%8C%E4%B8%9A%E4%B8%93%E9%A2%98%E6%8A%A5%E5%91%8A%EF%BC%9A%E5%9B%BD%E4%BA%A7FPGA%E7%A0%94%E7%A9%B6%E6%A1%86%E6%9E%B6-%E6%96%B9%E6%AD%A3%E8%AF%81%E5%88%B8[%E9%99%88%E6%9D%AD]-20201018%E3%80%90113%E9%A1%B5%E3%80%91.pdf)

<h2 align="center">二、进阶资料</h2>
<h3>SOC System on Chip</h3>

> Xilinx系列最全最详细的文档其实是官方提供的 [Xilinx Docnav](https://china.xilinx.com/support/documentation-navigation/overview.html)
>
> https://www.zhihu.com/question/56596019

- [MicroBlaze](https://china.xilinx.com/products/design-tools/microblaze.html)

- ZYNQ
  - [UG 585 最权威的官方文档](https://www.xilinx.com/support/documentation/user_guides/ug585-Zynq-7000-TRM.pdf)
  - [The ZYNQ Book](http://www.zynqbook.com/)
  - [The ZYNQ Book 中文版](http://leiblog.wang/static/FPGA/books/The_Zynq_Book_ebook_chinese.pdf)
  - [MicroZed 300多篇教学博客](http://adiuvoengineering.com/microzed-chronicles/?tdsourcetag=s_pctim_aiomsg)
  - [米联客 SOC 修炼秘籍](http://leiblog.wang/static/FPGA/books/ZYNQ/%E7%B1%B3%E8%81%94%E3%80%8AZYNQ%20SOC%E4%BF%AE%E7%82%BC%E7%A7%98%E7%B1%8D%E3%80%8B.pdf)

- [PYNQ](http://www.pynq.io/)
  - [Github](https://github.com/Xilinx/Pynq)
  - [xupsh pynqdoc](https://github.com/xupsh/pynqdoc)
  - [Docs](https://pynq.readthedocs.io/en/v2.5.1/)
  - [DIscuss](https://discuss.pynq.io/)
  - [PYNQ Z1 Digilent 中文指导手册](https://digilent-china.gitbook.io/)
  - [PYNQ 镜像制作](https://pynq.readthedocs.io/en/latest/pynq_sd_card.html#prepare-the-building-environment)

<h3>HLS 高层次综合</h3>

- [Xilinx 官方教程](http://xilinx.eetop.cn/list-83-1.html)

- [FPGA 并行编程](https://github.com/xupsh/pp4fpgas-cn)

- [Vivado HLS 基本应用与图像处理](https://www.bilibili.com/video/BV11b411e7m3)


<h3>计算机体系结构</h3>

- [Chisel 学习路线](https://blog.csdn.net/qq_34291505/article/details/86744581)

- [Chisel Book Chinese](http://www.imm.dtu.dk/~masca/chisel-book-chinese.pdf)

- [Chisel 入门资料](https://zhuanlan.zhihu.com/p/98097268)

- [CPU自制入门](http://leiblog.wang/static/FPGA/books/CPU自制入门.pdf)

- [手把手教你设计CPU——RISC-V处理器篇](https://leiblog.wang/static/FPGA/books/%E3%80%8A%E6%89%8B%E6%8A%8A%E6%89%8B%E6%95%99%E4%BD%A0%E8%AE%BE%E8%AE%A1CPU%E2%80%94%E2%80%94RISC-V%E5%A4%84%E7%90%86%E5%99%A8%E7%AF%87%E3%80%8B.pdf)

- [riscv-soc-book](https://github.com/cnrv/riscv-soc-book)

- [RISC-V 2020 Digilent](http://www.digilent.com.cn/community/697.html)

<h3>深度神经网络加速器</h3>

- [PYNQ_Classification](https://leiblog.wang/static/FPGA/books/Accelerator/PYNQ_CLASSIFICATION.pdf)

- [深度学习加速器设计与实验](https://www.bilibili.com/video/BV1ih411o7Yy?from=search&seid=3168767736458572847)

- [NVDLA](http://nvdla.org/)

- [VTA](https://tvm.apache.org/docs/vta/)

<h3>硬件驱动</h3>

- [AC620以太网驱动 芯航线](http://leiblog.wang/static/FPGA/books/HardwareDriver/AC620以太网设计与应用教程V1.0.pdf)

- [Video Series 教你如何搭建视频通路](https://forums.xilinx.com/t5/Video-and-Audio/Xilinx-Video-Series/td-p/849583)

- [UART](https://mp.weixin.qq.com/s?__biz=MzI4NjE3MzUwMA==&mid=2652138569&idx=1&sn=0fd5b6a75dd563bcc0a4480c8d095179&chksm=f0003c1ac777b50cff872bb53840fdc52a6f53bcef523cb5ecdf94aa3371fc398edfdf1b7807&token=1263105418&lang=zh_CN&scene=21#wechat_redirect)

- [IIC](https://mp.weixin.qq.com/s?__biz=MzI4NjE3MzUwMA==&mid=2652139704&idx=1&sn=817b2e70e4dc7ac3dd20db5306271ccd&chksm=f00020ebc777a9fda8234e95fd00d1c1fdc64fbbac4af9b03b63dbb2df8573fb8ac40a189810&scene=21#wechat_redirect)

- [SPI](https://mp.weixin.qq.com/s?__biz=MzI4NjE3MzUwMA==&mid=2652139702&idx=1&sn=c4b450e0913083e6e4d5db29a410924f&chksm=f00020e5c777a9f356ebd73fe9c0699c606f346d8c82d54e67e036d94a57f90edbce37fa5039&scene=21#wechat_redirect)

- [CAN](https://mp.weixin.qq.com/s?__biz=MzI4NjE3MzUwMA==&mid=2652138778&idx=1&sn=144a45d6f49f51613a399eac5ff7a257&chksm=f0003d49c777b45fa9dc06810638906f5fead6acc311b450c96d541f3cd44f35869809d722fd&token=272554766&lang=zh_CN&scene=21#wechat_redirect)

<h3>操作系统</h3>

- [Petalinux 中文文档](https://china.xilinx.com/support/documentation/sw_manuals/xilinx2019_1/c_ug1144-petalinux-tools-reference-guide.pdf)

### 还得是B站

- [数字集成电路静态时序分析基础](https://www.bilibili.com/video/av290295377)

  想知道电路运行的最大频率吗？

- [数字芯片设计基础](https://www.bilibili.com/video/BV12V411r7BD/)

### 还得是知乎

- [为什么ASIC的频率可以达到GHz，而FPGA只能达到几百MHz？](https://www.zhihu.com/question/51179323/answer/124680433)
- [Github 上有哪些优秀的 Verilog/FPGA 项目？](https://www.zhihu.com/question/348990787/answer/2486699396)

### 还得是steam

- [SHENZHEN I/O](https://store.steampowered.com/app/504210/SHENZHEN_IO/?l=tchinese)


<h2 align="center">三、优秀项目</h2>
<h3>官方开源项目</h3>

- [ADI 超多开源HDL库](https://github.com/analogdevicesinc/hdl)

- [ALINX 黑金 官方仓库 (包含OV系列摄像头驱动、DDR驱动等)](https://github.com/alinxalinx)
  - [AC616](https://github.com/alinxalinx/AC616)
  - [AX4010](https://github.com/alinxalinx/AX4010)
  - [AX7035](https://github.com/alinxalinx/AX7035)
  - [AX309](https://github.com/alinxalinx/AX309)
  - [AX7101](https://github.com/alinxalinx/AX7101)
  - [AX7102](https://github.com/alinxalinx/AX7102)
  - [AX7103](https://github.com/alinxalinx/AX7103)
  - [AX7021](https://github.com/alinxalinx/AX7021)
  - [AX7010](https://github.com/alinxalinx/AX7010)
  - [AX301](https://github.com/alinxalinx/AX301)
  - [AX7020](https://github.com/alinxalinx/AX7020)
  - [AX7015](https://github.com/alinxalinx/AX7015)
- [Digilent 官方仓库](https://github.com/Digilent)
  - [vivado-library 很多好用的IP-VGA、HDMI等](https://github.com/Digilent/vivado-library)
  - [vivado-boards Digilent开发板的板卡文件](https://github.com/Digilent/vivado-boards)
    - [使用板卡文件，让你的设计事半功倍](https://www.bilibili.com/s/video/BV1zg4y1q7Jd)
  - [Digilent 大神用户们的项目](http://www.digilent.com.cn/project/all/open.html)
- [赛灵思中文学习资料和开源设计](https://github.com/xupsh)
  - [74LSXX 芯片IP](https://github.com/xupsh/Digital-Design-Reference-Design/tree/dd239f50d5117917479b7a3b51eeb8a0d6945cc9/Library/74LSXX_Lib)

<h3>优秀开源项目 - 初级</h3>

- [Verilog Practice](https://github.com/xiaop1/Verilog-Practice)
  - Verilog训练

- [带闹钟功能的计数器](https://github.com/LeiWang1999/DigitalAlarmClock)
  - 板卡:`Nexys4 DDR`
  - 功能
    - 支持I2S协议驱动的音响，接入耳机播放闹钟
    - 支持VGA显示剩余时间
    - 支持闹钟计数时钟变速(一倍速和五倍速)
- [搭建你的数字积木 配套工程](https://github.com/xupsh/Digital-Design-Lab)
  - 板卡:`Basys3`|`EGO-1`
  - 配套图书:[搭建你的数字积木](https://book.douban.com/subject/30242443/)

<h3>优秀开源项目 - 中级</h3>

- [基于FPGA的机器博弈五子棋游戏](https://github.com/Starrynightzyq/ZYNQ-PYNQ-Z2-Gobang)
  - 板卡:`PYNQ-Z2`
  - 2018全国大学生FPGA创新设计邀请赛一等奖、最佳创意奖
- [CM3软核 FPGA 车牌识别系统](https://github.com/Starrynightzyq/Nexys4DDR-ARM-M3-Plate-Recognition)
  - 板卡:`Nexys4 DDR`
  - 全国大学生集成电路创新创业大赛参赛作品
- [Yolov2加速器设计](https://github.com/dhm2013724/yolov2_xilinx_fpga)
  - 板卡:`PYNQ-Z2|ZedBoard|ZCU102`
  - 很不错的加速器设计方案
- [Pynq Accelerator](https://github.com/LeiWang1999/Pynq-Accelerator)
  - 板卡:`PYNQ-Z1`
- [ZYNQ NVDLA](https://github.com/LeiWang1999/ZYNQ-NVDLA)
  - 板卡：`ZYNQ 7045 | ZCU 102`
  - 开源加速器的解决方案、**可以跑任意网络！**
- [FPGA Support for Vscode](https://github.com/Bestduan/fpga_support_plug)
  - 北邮的一个大佬开源的Vscode写FPGA的项目

<h3>优秀开源项目 - 高级</h3>

- [PYNQ集群 类脑计算](https://github.com/OpenHEC/SNN-simulator-on-PYNQcluster)
  - 板卡:`PYNQ`
  - 全国大学生FPGA创新设计作品
- [basicmi/AI Chip](https://github.com/basicmi/AI-Chip)
  - 关于 AI 芯片的跟踪report仓库

<h2 align="center">四、推荐群组</h2>

1. <OpnFPGA/IC攻城狮>
- 类型：QQ群
- 群号：915880054
- 备注：碎碎思大佬的群，主要是分享资料的，进群可以转微信群，那边很活跃。

2. <Verilog编程艺术>
- 类型：QQ群
- 群号：361820636
- 备注：群主几百年没有出现过了，也没有管理员，时常有广告

3. <verilog vhdl fpga入门进阶>
- 类型：QQ群
- 群号：1140582958
- 备注：1000人大群

4. <摸鱼范式-2022届数字IC>
- 类型：QQ群
- 群号：1060380138
- 备注：“摸鱼范式”公众号的群，2000人群
