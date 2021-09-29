**此 for-osee-pre 代码库仅仅为个人服务，没有打算共享出去，拒绝一切空谈废话**


目前准备考取 OSEP，正在做准备工作，此库将不定时更新，直至取到 OSEE


需要取得 3 个认证，才能自动获取 OSEE 认证 

第一、OSEP  

    主要学习防火墙规避,杀软绕过，域名诈骗，AD域等知识

第二、OSWE  

    专门针对于web应用攻击得高阶课程

第三、OSED  

    主要是针对windows的攻击课程，包括BoF, Reserver Engineering。具体不知道


# OSEP 目录

```
1  规避技术和突破防御：一般课程信息
    1.1  关于PEN-300 课程
    1.2  提供的材料
        1.2.1  PEN-300 课程材料
        1.2.2  访问内部 VPN 实验室网络
        1.2.3  offensive security 学生论坛
        1.2.4  在线支持和 RocketChat
        1.2.5  OSEP 考试尝试
    1.3  课程实施策略
        1.3.1  欢迎和课程信息邮件
        1.3.2  课程资料
        1.3.3  课程练习
    1.4  关于 PEN-300 VPN 实验室
        1.4.1  控制面板
        1.4.2  机器重置
        1.4.3  客户端机器
        1.4.4  kali 虚拟机
        1.4.5  实验室行为和实验室限制
    1.5  关于OSEP 考试
    1.6 收尾
2  操作系统和编程理论
    2.1  编程理论
        2.1.1  程序语言级别
        2.1.2  编程概念
    2.2 windows 概念
        2.2.1  Windows 的窗口
        2.2.2  Win32 API
        2.2.3  注册表
    2.3 收尾
3  office客户端代码执行
    3.1  Dropper 病毒
        3.1.1  Staged vs Non-staged Payloads
        3.1.2  建立我们自己的 Droppers
        3.1.3  通过 HTML 投毒
    3.2  利用 Office 投毒
        3.2.1  安装office
        3.2.2  介绍 VBA
        3.2.3  让 powershell 帮助我们
    3.3  装腔作势（伪装）
        3.3.1  网络钓鱼托词
        3.3.2  切换身份（?）
    3.4  在 word 内存中执行 shellcode
        3.4.1  从VBA 中调用 win32 API
        3.4.2  VBA shellcode 运行器
    3.5  powershell shellcode 运行器
        3.5.1  从 powershell 中调用 win32 api
        3.5.2  移植 shellcode 运行器到 powershell
    3.6  在内存中维持 powershell
        3.6.1  Add-Type 编译
        3.6.2  利用 UnsafeNativeMethods
        3.6.3  反射 DelegateType
        3.6.4  反射 shellcode 运行器在 PowerShell
    3.7  与代理通信
        3.7.1  Powershell Proxy-Aware 通信
        3.7.2  玩弄 User-Agent 头信息
        3.7.3  给我一个 SYSTEM 代理
    3.8  收尾
4  客户端代码执行 和 Windows Script Host
    4.1  在 Jscript 中 创建一个基本 Dropper
        4.1.1  Jscript 在 windows 的执行
        4.1.2  Jscript Meterpreter Dropper
    4.2  Jscript 和 C#
        4.2.1  介绍 Visual Studio
        4.2.2  DotNetToJscript
        4.2.3  从 C# 调用 Win32 API
        4.2.4  C# 里的 shellcode 运行器
        4.2.5  Jscript shellcode 运行器
        4.2.6  用 SharpShooter 生成 payload
    4.3  重新访问内存中 powershell
        4.3.1  Reflective Load
    4.4  收尾
5 Process 注入和迁移
    5.1  为 shellcode 找一个宿主
        5.1.1  进程注入和迁移理论
        5.1.2  在 C# 中进程注入
    5.2  DLL 注入
        5.2.1  DLl 注入理论
        5.2.2  使用C# 进行 Dll 注入
    5.3  反射DLL注入
        5.3.1  反射DLL注入理论
        5.3.2  反射DLL注入在 Powershell
    5.4  进程空心(?)
        5.4.1  进程空心理论
        5.4.2  进程空心在 C#
    5.5  收尾
6 防病毒软件规避介绍
    6.1  杀毒软件概览
    6.2  模拟目标环境
    6.3  在文件中查找签名
    6.4  使用 metasploit 绕过杀毒软件
        6.4.1  metasploit 编码器
        6.4.2  metasploit 加密器
    6.5  使用C#绕过杀毒软件
        6.5.1  C# shellcode 运行器 对决杀软
        6.5.2  加密C# shellcode 运行器
    6.6  扰乱我们的行为
        6.6.1  简单定时睡眠
        6.6.2  Non-emulated APIs
    6.7  办公室请绕开杀入软件
        6.7.1  绕过杀软在VBA中
        6.7.2  踩在 Microsoft Word 头上绕
    6.8  在VBA中隐藏 Powershell
        6.8.1  检测Powershell shellcode 运行器
        6.8.2  使用wmi 解锁
        6.8.3  混淆 VBA
    6.9  收尾
7  高级防病毒软件规避
    7.1  Intel 体系结构和win10
        7.1.1  WinDbg 介绍
    7.2  反恶意软件扫描接口
        7.2.1  理解AMSI
        7.2.2  钩子和 Frida
    7.3  在powershell中反射绕过 SAMSI
        7.3.1  妈的Context 是什么？
        7.3.2  攻击初始化
    7.4  在PowerShell中破坏AMSI
        7.4.1  理解分配流程
        7.4.2  内部修补
    7.5  UAC 绕过对决windows自带防火墙
        7.5.1  FodHelper UAC 绕过
        7.5.2  改进 FodHelper
    7.6  在 JScript中绕过AMSI
        7.6.1  检测 AMSI API 流程
        7.6.2  那是你的注册Key 吗？
        7.6.3  我是我自己的可执行文件
    7.7  收尾
8 应用程序白名单
    8.1  应用程序白名单理论和设置
        8.1.1  应用程序白名单理论
        8.1.2  AppLocker 设置和规则
    8.2  基本绕过
        8.2.1  信任的文件夹
        8.2.2  使用 dll 绕过
        8.2.3  修改数据流
        8.2.4  第三方执行
    8.3  使用Powershell 绕过 AppLocker
        8.3.1  Powershell 约束语言模式
        8.3.2  自定义运行空间
        8.3.3  Powershell CLM 绕过
        8.3.4  反射注入返回
    8.4  使用 C# 绕过AppLocker
        8.4.1  定位一个地址
        8.4.2  逆向加载过程
        8.4.3  给我一个代码执行
        8.4.4  调用地址部分1
        8.4.5  调用地址部分2
    8.5  绕过AppLocker 使用JScript
        8.5.1  Jscript 和 MSHTA
        8.5.2  XSL 转换
    8.6 收尾
9  绕过网络拦截
        9.1  DNS 拦截
            9.1.2  处理DNS过滤
        9.2  web 代理
            9.2.1  绕过web代理
        9.3  IDS 和 IPS 传感器
            9.3.1  案例学习：自定义证书绕过诺顿 HIPS
        9.4  抓包设备
        9.5  HTTPS 查看
        9.6  域名(前域)Domain Fronting
            9.6.1  使用Azure CDN前域
            9.6.2  域名前域在实验室
        9.7  DNS 隧道
            9.7.1  DNS 隧道是怎么工作的
            9.7.2  使用 dnscat2 进行隧道
        9.8  收尾
10 linux Post-Exploitation
        10.1  用户配置文件
            10.1.1  vim 配置简单后门
            10.1.2  vim 配置简单键盘记录器
        10.2  绕过AV
            10.2.1  卡巴斯基端点安全
            10.2.2  antiscan.me
        10.3  共享库
            10.3.1  共享库在linux是怎么工作的
            10.3.2  通过 LD_LIBRARY_PATH进行注入
            10.3.3  通过 LD_PRELOAD 溢出
        10.4  收尾
11  绕过kiosk 浏览器
        11.1  kiosk 枚举
            11.1.1  kiosk 浏览器枚举
        11.2  命令执行
            11.2.1  探索文件系统
            11.2.2  利用Firefox 配置
            11.2.3  枚举系统信息
            11.2.4  继续深入
        11.3  发送溢出
            11.3.1  模拟交互式外壳
        11.4  权限提升
            11.4.1  思考跳出盒子
            11.4.2  RootShell 在一个小时以上
            11.4.3  获取到root终端访问
        11.5  Windows kiosk 突破技术
        11.6 收尾
12 windows 认证
        12.1  本地windows认证
            12.1.1 SAM 数据库
            12.1.2  强化本地管理员账户
        12.2  Tokens 访问
            12.2.1  AccessToken 理论
            12.2.2  假冒提升
            12.2.3  无痕访问的乐趣
        12.3  Kerberos 和域认证
            12.3.1  Kerberos 认证
            12.3.2  mimikatz
        12.4  离线处理认证
            12.4.1  内存导出
            12.4.2  miniDumpWriteDump
        12.5  收尾
13  windows 横向移动
        13.1  远程桌面协议
            13.1.1  使用RDP横向移动
            13.1.2  使用metasploit 端口映射RDP协议
            13.1.3  使用chisel端口映射RDP
            13.1.4  RDP 作为一个控制台
            13.1.5  从RDP中窃取明文文本
        13.2  无文件横向移动
            13.2.1  认证和执行理论
            13.2.2  在C#中实现无文件移动
        13.3  收尾
14  linux 横向移动
        14.1  用ssh横向移动
            14.1.1  ssh keys
            14.1.2  ssh 持久化
            14.1.3  ssh 劫持 ControlMaster
            14.1.4  使用SSH-agent和SSh agent转发劫持SSH
        14.2  DevOps
            14.2.1  Ansible 介绍
            14.2.2  Ansible 枚举 
            14.2.3  Ad-hoc 命令
            14.2.4  Ansible PlayBooks
            14.2.5  为Ansible用户认证，溢出PlayBooks
            14.2.6  Ansible Playbooks 的弱权限
            14.2.7  通过Ansible模块泄露敏感数据
            14.2.8  介绍 Artifactory
            14.2.9  Artifactory 枚举
            14.2.10 破坏 Artifactory 备份
            14.2.11 破坏 Artifactory’s 数据库
            14.2.12 添加一次次要的 Artifactory 管理员账户
15  微软sql server 攻击
        15.1  域里面的sqlserver攻击
            15.1.1 sqlserver 枚举
            15.1.1 sqlserver 认证
            15.1.1 UNC 路径注入
            15.1.1 延迟我的hash
        15.2  sqlserver 权限提升
            15.2.1  权限提升
            15.2.2  获取代码执行
            15.2.3  自定义资源
        15.3  链接的sqlserver
            15.3.1  跟踪一个链接
            15.3.2  回到我家
        15.4  收尾
16  域溢出
        16.1  AD 对象安全权限
            16.1.1 对象权限理论
            16.1.2 滥用 GenericAll
            16.1.3 滥用 WriteDACL
        16.2  Kerberos 委派
            16.2.1  不受约束的委派
            16.2.2  我是一个域控制器
            16.2.3  受约束的授权
            16.2.4  基于资源的受限委派
        16.3  活动目录森林理论
            16.3.1  在目录森林受信任的域目录
            16.3.2  枚举目录森林
        16.4  烧毁目录森林
            16.4.1  拥有额外的目录森林和扩展 SIDs
            16.4.2  打印我们的目录森林
        16.5  越过森林
            16.5.1  在目录森林中信任的域目录
            16.5.2  枚举森林之外
        16.6  追加一个额外的目录森林
            16.6.1  向我展示你的扩展SID
            16.6.2  链接后的 sql server在目录森林中
        16.7  收尾
17  组合拼凑
        17.1  枚举和shell
            17.1.1 初始化枚举
            17.1.2 获得最初的立足点
            17.1.3 Post Exploitation 枚举
        17.2  攻击委派
            17.2.1  在 web01 中权限升级
            17.2.2  获取到 hash
            17.2.3  委派我的票据
        17.3  拥有域
            17.3.1  横向移动
            17.3.2  成为一个域管理
        17.4  收尾
18  在lab 中更努力
        18.1  模拟真实生活
        18.2  收尾
```