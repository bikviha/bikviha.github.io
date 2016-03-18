![banner pic](/public/images/banana.jpg "banner pic")

# Linux 操作命令

    列出所有版本信息
>lsb_release -a

    查看当前服务和监听端口
>netstat

>-a ：all，表示列出所有的连接，服务监听，Socket资料

>-t ：tcp，列出tcp协议的服务

>-u ：udp，列出udp协议的服务

>-n ：port number， 用端口号来显示

>-l ：listening，列出当前监听服务

>-p ：program，列出服务程序的PID




```C
#include <stdio.h>
void main(int argc, char** argv)
{
    printf(“Hello World”);
}
```
