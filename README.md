简介：这是一个用ai(DeepSeek)基于HTML写的一个视频展台软件，实现了基本功能，用于替代希沃视频展台

1.目前已有视频展台软件可用，为什么还要用AI写这么一个东西？

因为希沃视频展台适配了linux,去年底我在学校教室电脑上安装了linux系统，但是......linux版本的希沃视频展台是electron浏览器套壳，占地800MB，比Edge都大；1024*768小分辨率下界面显示不全；冻结画面会意外解冻（在反馈bug后，此问题已在3月3日的希沃视频展台2.0.5.2006版本修复）；拍照保存存不了整个画面，而是仅屏幕内，总之一言难尽，导致每次老师要使用展台时我都得重启回Windows以免挨骂......

2.基本功能

输出摄像头画面

单指拖动，双指缩放，也可以用鼠标

将老师最常用的旋转和锁定功能放到了一级菜单（搞不懂希沃为什么要把这些东西放二级菜单）

保存：画面锁定后右键另存图片

批注功能可以用edge浏览器截图批注凑合用


4.优点
单文件html，仅14kb，比希沃展台小多了

网页，Windows、linux平台都能用


5.缺点：对一些chromium内核浏览器，每次都需要手动允许摄像头权限，全屏也需要手动点，不过有解决方案：


安装python，在系统开机启动目录中添加一个开机启动项：


python3 -m http.server 8000

然后访问127.0.0.1:8000,翻到html文件，复制网址


在桌面新建快捷方式指向你的浏览器，在路径后空格加参数--start-fullscreen,再空格加复制的网址

下载文件列表中的”视频展台.html”或在release栏下载
