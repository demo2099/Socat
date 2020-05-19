Socat一键安装脚本
-----------
系统要求：支持CentOS 6+ 、Debian 7+、Ubuntu 14+

脚本说明：脚本默认开启`UDP`、`TCP`转发，带开机自启功能，且一次只能转发单个端口，如果想转发多个端口请重复运行本脚本。

使用`root`运行以下命令：

    wget https://raw.githubusercontent.com/demo2099/Socat/master/socat.sh && bash socat.sh

按要求输入本地服务器端口，要转发的目标端口和服务器IP即可！

停止转发

ps -ef | grep socat

输入上面的命令找到socat程序的PID，然后用下面的命令KILL掉这个PID进程（PID是个数字，自己替换下面的”pid”）。
​

kill -9 pid

Socat卸载

Centos系统：
yum remove socat


Debian/Ubuntu系统：
sudo apt-get remove socat
sudo apt-get autoremove


