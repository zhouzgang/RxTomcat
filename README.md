## RxTomcat

为了理解 Tomcat 内部原理，在阅读源码的过程中，尽可能的使用简洁的代码，来模拟实现核心模块的处理流程。基础源码版本使用的是 6.0.53，因为这个版本没有过多的抽象，理解起来比较简单直观。

## rxtomcat-net

 - 实现 NIO 模型的核心处理流程
 - 编写了一个简单的回显服务进行测试

**测试**

运行 TestNioEndpoint 的 main 方法，使用 telnet 命令进行测试，在 windows 下记得打开回显（ctrl+] -> set localecho -> Enter）

```bash
==========================================
  Tomcat NIO Test - EchoProcessor
  Author: wskwbog
  Git: http://github.com/tonwu/rxtomcat
  Support: Ctrl+c Backspace
==========================================
NIO> Hello World!
Hello World!
NIO>
```

## rxtomcat-utils

 - 简单实现 Digester 解析 xml 的功能
