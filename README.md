简介：这是一个用ai(DeepSeek)基于HTML写的一个视频展台软件，实现了基本功能，用于替代希沃视频展台

首先不要指望这个HTML能有多好，仅仅实现了基本功能，足够老师用
代码Deepseek写的，我只是一个基本上没学过编程（仅信息课学了一点python，HTML是完全没学过）的高三学生

1.我为什么要用AI写这么一个东西？
因为希沃视频展台适配了linux,去年底我在学校教室电脑上安装了linux系统
但linux版本的希沃视频展台：electron浏览器套壳，占地800MB，比Edge都大；1024*768小分辨率下界面显示不全；冻结画面会意外解冻（我反馈bug后，此问题已在3月3日的希沃视频展台2.0.5.2006版本修复）；拍照保存存不了整个画面，而是仅屏幕内，总之一言难尽，导致每次老师要使用展台时我都得重启回Windows以免挨骂......
年初Deepseek爆火，于是我就用Deepseek，采用和希沃一样的网页路线做了这个尝试

2.基本功能
输出摄像头画面
单指拖动，双指缩放，也可以用鼠标
将老师最常用的旋转和锁定功能放到了一级菜单（搞不懂希沃为什么要把这些东西放二级菜单）
保存：画面锁定后右键另存图片
以上功能足够老师用了

3.没有做的功能
扫码：难度较大，且一年用不到几次
批注：难度较大，ai处理不好多图层，可以用edge浏览器截图批注代替
对比教学/延时拍照等功能应该不重要，没几个老师用

4.优点
单文件html，仅14kb，比希沃展台小多了(Windows版100m，附带一堆Support Files,Linux版800m)
就是一网页，Windows、linux平台都能用
仅核心功能，比较简洁（简陋）

5.由于设备原因，这个软件没有用不同型号的电脑摄像头测试过，文件中有一行写了”2592*1944”，但我修改这个数值好像不影响正常使用，如果有问题你可以尝试用记事本打开文件改一下这个值试试

下载文件列表中的”视频展台.html”或在release栏下载
