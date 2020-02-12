# Linux远程桌面环境
一键安装桌面环境，RDP，Windows支持，用于Linux的Office工具。

作者: https://tech.cxthhhhh.com （网站打不开了 !2020/02/12）

![image](https://raw.githubusercontent.com/ciweiin/Linux-Remote-Desktop/master/Download/Image/Demo_Picture.jpg)

特点:
1. 一键安装Linux（CentOS / Debian / Ubuntu）的桌面环境和RDP远程桌面连接。

   （您需要新安装的Linux系统，推荐的硬件要求是：CPU内核≥1，内存≥1GB，磁盘空间≥15GB。硬件配置越高，效果越好。您也可以尝试以较低的硬件配置运行Debian， 但它可能运行缓慢。）

    推荐系统：[原装]网络一键式重新安装CentOS 7（正式，纯净，安全，高效） 
    网址失效 自己百度找 

2. Windows应用程序支持。 (via Wine)

    （安装Wine X64和X86，现在您可以在Linux上运行Windows应用程序。）

3. 创建一个3GB交换内存。 避免由于内存不足而导致的错误。

    (Swap 位置: /var/swapd)

4. 安装中文输入环境，中文支持。

    （在没有中文环境的情况下，您将无法查看中文字体。这会导致编码混乱。）

5. 安装大家推荐的软件，例如浏览器，Office工具和输入法。

    (作者在这里 https://www.hostloc.com/thread-466449-1-1.html 和 https://www.hostloc.com/thread-473982-1-1.html 发布了一项调查。 尊重调查结果，已安装Chrome，Firefox，WPS International，FileZilla。)

6. 安装远程桌面客户端。 （Remmina允许您连接和管理其他计算机或服务器。）
    （支持RDP / SSH / NX / SFTP / VNC / XDMCP协议）

让我们开始吧 (via root user)

    wget --no-check-certificate -qO ~/Linux-Remote-Desktop-Environment.sh 'https://raw.githubusercontent.com/ciweiin/Linux-Remote-Desktop/master/Linux-Remote-Desktop-Environment.bash' && chmod a+x ~/Linux-Remote-Desktop-Environment.sh
    (CentOS 7+)			bash ~/Linux-Remote-Desktop-Environment.sh -CentOS
    (Debian 9+)			bash ~/Linux-Remote-Desktop-Environment.sh -Debian
    (Ubuntu 18.04+)		bash ~/Linux-Remote-Desktop-Environment.sh -Ubuntu

国内加速版 (via root user)
    wget --no-check-certificate -qO ~/Linux-Remote-Desktop-Environment.sh 'https://cdn.jsdelivr.net/gh/ciweiin/Linux-Remote-Desktop@latest/CN-Linux-Remote-Desktop-Environment.bash' && chmod a+x ~/Linux-Remote-Desktop-Environment.sh
    (CentOS 7+)			bash ~/Linux-Remote-Desktop-Environment.sh -CentOS
    (Debian 9+)			bash ~/Linux-Remote-Desktop-Environment.sh -Debian
    (Ubuntu 18.04+)		bash ~/Linux-Remote-Desktop-Environment.sh -Ubuntu

现在，您已经可以通过RDP连接（IP：3389）

    （请注意，通常不建议使用root用户，因此将自动使用密码[cxthhhhhh.com]创建用户[RdpUser]，并且您应尽快更改默认密码。）

您应该查看我的教程，以了解需要注意的内容。

    教程名称：[原始]一键安装桌面环境，RDP，Windows对Linux的支持
    URL : https://tech.cxthhhhh.com/linux/2018/08/07/original-one-click-installation-of-desktop-environment-rdp-windows-support-for-linux-en.html （网站打不开了 !2020/02/12）

版本: 2.0.2版（稳定版）
2018年9月11日更新