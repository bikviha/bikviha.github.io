![banner pic](/public/images/banana.jpg "banner pic")

# Linux 操作命令

    列出所有版本信息
>lsb_release -a

    ubuntu 系统更新
>sudo apt-get update<br/>
>sudo apt-get upgrade<br/>
>sudo apt-get dist-upgrade

    查看当前服务和监听端口
>netstat

>-a ：all，表示列出所有的连接，服务监听，Socket资料<br/>
>-t ：tcp，列出tcp协议的服务<br/>
>-u ：udp，列出udp协议的服务<br/>
>-n ：port number， 用端口号来显示<br/>
>-l ：listening，列出当前监听服务<br/>
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
>wget -r -p -np -k<br/>
>-r：在本机建立服务器端目录结构；<br/>
>-p: 下载显示HTML文件的所有图片；<br/>
>-np：只下载目标站点指定目录及其子目录的内容；<br/>
>-k: 转换非相对链接为相对链接。<br/>

    查看已经安装了哪些包
>dpkg -l


    参考网址：http://www.jb51.net/os/Ubuntu/56362.html

```C
#include <stdio.h>
void main(int argc, char** argv)
{
    printf(“Hello World”);
}
```
