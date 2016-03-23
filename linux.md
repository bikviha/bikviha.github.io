![banner pic](/public/images/banana.jpg "banner pic")

# Linux 操作命令

    列出所有版本信息
>lsb_release -a

    ubuntu 系统更新
>sudo apt-get update

    查看当前服务和监听端口
>netstat

>-a ：all，表示列出所有的连接，服务监听，Socket资料

>-t ：tcp，列出tcp协议的服务

>-u ：udp，列出udp协议的服务

>-n ：port number， 用端口号来显示

>-l ：listening，列出当前监听服务

>-p ：program，列出服务程序的PID

    查看当前有哪些进程
>ps -A

    查看硬盘剩余空间
>df -h

    查看当前的内存使用情况
>free -m

    显示xxx文件倒数6行的内容
>tail -n 6 xxx

    下载网站文档
>wget -r -p -np -k

>r：在本机建立服务器端目录结构；

>-p: 下载显示HTML文件的所有图片；

>-np：只下载目标站点指定目录及其子目录的内容；

>-k: 转换非相对链接为相对链接。

    查看已经安装了哪些包
>dpkg -l

```C
#include <stdio.h>
void main(int argc, char** argv)
{
    printf(“Hello World”);
}
```
