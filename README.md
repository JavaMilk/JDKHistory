# JDKHistory
记录Java版本的更新历史，主要是对以下文章的结合：
* [《Java - JCP、JSR等名词介绍》](http://blog.csdn.net/u010297957/article/details/50915631)
* [《从java1到java9每个版本都有什么新特性？》](https://www.cnblogs.com/rese-t/p/7823378.html)
* [《Java 9正式发布》](http://blog.csdn.net/postnull/article/details/78068060?locationNum=2&fps=1)
* [《JDK 10 本周将进入候选发布阶段，新特性抢先看》](https://www.oschina.net/news/93123/jdk10-release-candidate-phase)
* [《Java 老矣，尚能饭否？》](http://www.infoq.com/cn/articles/is-java-out-of-date)

# 一些术语
* [JCP](https://www.jcp.org/en/home/index) 是 Java Community Process（Java社区进程）的简称，社会各界Java组成的社区，规划和领导Java的发展。
* [JEP](http://openjdk.java.net/jeps/0) 是 JDK Enhancement Proposals （Java 增强提案）的简称，JDK的版本变化将从这些提案中选取。
* JSR 是 Java Specification Requests（Java规范请求）的简称，是 JCP 成员向委员会提交的 Java 发展议案，经过一系列流程后，如果通过会成为 JEP，最终会体现在未来的Java中。
* TCK 是 Technology Compatibility Kit（技术兼容性测试）的简称， 如果一个平台型程序想要宣称自己兼容Java，就必须通过TCK测试

# JDK 11
[JDK 11](http://openjdk.java.net/projects/jdk/11/) 目前出现了4个JEP，计划于 2018 年 9 月发布。
* [JEP 309](http://openjdk.java.net/jeps/309): 动态类文件常量。
* [JEP 318](http://openjdk.java.net/jeps/318): 低开销垃圾收集器 Epsilon。
* [JEP 320](http://openjdk.java.net/jeps/320): 移除 Java EE 和 CORBA 模块。
* [JEP 323](http://openjdk.java.net/jeps/323): Lambda 参数的本地变量语法。

# JDK 10
[JDK 10](http://openjdk.java.net/projects/jdk/10/) 按计划将于2018年3月20日发布。新特性有：
* [JEP 286](http://openjdk.java.net/jeps/286): 局部变量的类型推导。该特性在社区讨论了很久并做了调查，可查看 JEP 286 调查结果。
* [JEP 296](http://openjdk.java.net/jeps/296): 将 JDK 的多个代码仓库合并到一个储存库中。
* [JEP 304](http://openjdk.java.net/jeps/304): 垃圾收集器接口。通过引入一个干净的垃圾收集器（GC）接口，改善不同垃圾收集器的源码隔离性。
* [JEP 307](http://openjdk.java.net/jeps/307): 向 G1 引入并行 Full GC。
* [JEP 310](http://openjdk.java.net/jeps/310): 应用类数据共享。为改善启动和占用空间，在现有的类数据共享（“CDS”）功能上再次拓展，以允许应用类放置在共享存档中。
* [JEP 312](http://openjdk.java.net/jeps/312): 线程局部管控。允许停止单个线程，而不是只能启用或停止所有线程。
* [JEP 313](http://openjdk.java.net/jeps/313): 移除 Native-Header Generation Tool (javah)
* [JEP 314](http://openjdk.java.net/jeps/314): 额外的 Unicode 语言标签扩展。包括：cu (货币类型)、fw (每周第一天为星期几)、rg (区域覆盖)、tz (时区) 等。
* [JEP 316](http://openjdk.java.net/jeps/316): 在备用内存设备上分配堆内存。允许 HotSpot 虚拟机在备用内存设备上分配 Java 对象堆。
* [JEP 317](http://openjdk.java.net/jeps/317): 基于 Java 的 JIT 编译器（试验版本）。
* [JEP 319](http://openjdk.java.net/jeps/319): 根证书。开源 Java SE Root CA 程序中的根证书。
* [JEP 322](http://openjdk.java.net/jeps/322): 基于时间的版本发布模式。“Feature releases” 版本将包含新特性，“Update releases” 版本仅修复 Bug 。

# JDK 9
[JDK 9](http://openjdk.java.net/projects/jdk9/) 于2017年9月21日发布。新特性有：
* 模块化 —— Jigsaw
* 交互式命令行 —— JShell
* 默认的垃圾回收器 —— G1
* 进程操作改进
* 竞争锁的性能优化
* 分段代码缓存
* 优化字符串占用空间

这个版本中最引人注目的时候模块化，通过这个工作，可以构建更小的运行时环境，只需要包括Java平台中任务依赖的部分。这可以更好地适应云端的开发。

具体的特性包括：
* [JEP 102](http://openjdk.java.net/jeps/102): 改善了控制和管理操作系统进程的 API。
* [JEP 110](http://openjdk.java.net/jeps/110): 定义了一个新的 Http 客户端 API，它实现了 `HTTP/2` 和 `WebSocket`，并且可以替代遗留的 ` HttpURLConnection` API。该 API 将会以一个 incubator 模块的形式进行交付。
* [JEP 143](http://openjdk.java.net/jeps/143): 提高竞争 Java 对象的监视性能。
* [JEP 158](http://openjdk.java.net/jeps/158): 统一 JVM 的日志。
* [JEP 165](http://openjdk.java.net/jeps/165): 通过支持运行时管理来增加对 JVM 编译器的管理。
* [JEP 193](http://openjdk.java.net/jeps/193): 对变量处理的改进。
* [JEP 197](http://openjdk.java.net/jeps/197): 将代码缓存划分成不同的段。
* [JEP 200](http://openjdk.java.net/jeps/200): 采用 Java 平台模块化系统（Java Platform Module System，JPMS）对JDK进行模块化。
* [JEP 201](http://openjdk.java.net/jeps/201): 源代码模块化。
* [JEP 211](http://openjdk.java.net/jeps/211): 在 import 语句中 省略 `deprecation` 的警告。
* [JEP 212](http://openjdk.java.net/jeps/212): 解决 lint 和 doclint 警告。
* [JEP 213](http://openjdk.java.net/jeps/213): Project Coin 的改变
* [JEP 214](http://openjdk.java.net/jeps/214): 移除 JDK 8 中 GC 组合器的废弃说明。
* [JEP 215](http://openjdk.java.net/jeps/215): 在 javac 中实现了一个新的类型检测策略。
* [JEP 216](http://openjdk.java.net/jeps/216): 正确地处理导入声明。
* [JEP 217](http://openjdk.java.net/jeps/217): 注解流水线 2.0。
* [JEP 219](http://openjdk.java.net/jeps/219): 定义了数据传输层安全（Datagram Transport Layer Security, DTLS）API。
* [JEP 220](http://openjdk.java.net/jeps/220): 模块化运行时镜像。
* [JEP 221](http://openjdk.java.net/jeps/221): 简化 `Doclet` API。
* [JEP 222](http://openjdk.java.net/jeps/222): jshell - Java 中的交互式命令行。
* [JEP 223](http://openjdk.java.net/jeps/223): 新的版本字符串模式。
* [JEP 224](http://openjdk.java.net/jeps/224): 增强了 javadoc 工具来生成 HTML5 标记。
* [JEP 225](http://openjdk.java.net/jeps/225): 增加了 javadoc 搜索。
* [JEP 226](http://openjdk.java.net/jeps/226): UTF-8 属性文件资源的Bundle相关变化。
* [JEP 227](http://openjdk.java.net/jeps/227): Unicode 7.0。
* [JEP 228](http://openjdk.java.net/jeps/228): 增加更多可诊断的命令。
* [JEP 229](http://openjdk.java.net/jeps/229): 将默认的秘钥库从 JKS 替换为 PKCS12。
* [JEP 231](http://openjdk.java.net/jeps/231): 移除运行时 JRE 版本选择。
* [JEP 232](http://openjdk.java.net/jeps/232): 增强了安全相关应用的性能。
* [JEP 233](http://openjdk.java.net/jeps/233): 开发了一个工具来自动测试运行时编译器。
* [JEP 235](http://openjdk.java.net/jeps/235): 增加关于 javac 生成类文件属性的 测试。
* [JEP 236](http://openjdk.java.net/jeps/236): 定义了解析 API 来支持 Nashorn 的 ECMAScript 抽象语法树。
* [JEP 237](http://openjdk.java.net/jeps/237): Linux/AArch64 端口相关。
* [JEP 238](http://openjdk.java.net/jeps/238): 多版本 JAR 文件。
* [JEP 240](http://openjdk.java.net/jeps/240): 移除 JVM 的 TI hprof 客户端。
* [JEP 241](http://openjdk.java.net/jeps/241): 移除 jhat 工具。
* [JEP 243](http://openjdk.java.net/jeps/243): 提供 Java 语言级的 JVM 编译接口。
* [JEP 244](http://openjdk.java.net/jeps/244): TLS 应用层协议协商。
* [JEP 245](http://openjdk.java.net/jeps/245): 验证 JVM 命令行标志参数。
* [JEP 246](http://openjdk.java.net/jeps/246): 利用 CPU 指令提升 GHASH 和 RSAd 的性能。
* [JEP 247](http://openjdk.java.net/jeps/247): 对老平台版本的编译支持。
* [JEP 248](http://openjdk.java.net/jeps/248): G1 作为默认的垃圾回收器。
* [JEP 249](http://openjdk.java.net/jeps/249): 基于 TLS 实现 OCSP Stapling。
* [JEP 250](http://openjdk.java.net/jeps/250): 在类数据分享（CDS）归档中存储 interned 字符串。
* [JEP 251](http://openjdk.java.net/jeps/251): 多方案镜像。
* [JEP 252](http://openjdk.java.net/jeps/252): 默认使用 CLDR Locale Data。
* [JEP 253](http://openjdk.java.net/jeps/253): 为 JavaFX UI 控制 和 CSS API 的模块化做准备。
* [JEP 254](http://openjdk.java.net/jeps/254): 采用一个空间更加高效的 String 内部表示。
* [JEP 255](http://openjdk.java.net/jeps/255): 合并 Xerces 2.11.0 中的更新。
* [JEP 256](http://openjdk.java.net/jeps/256): BeanInfo 注解调整。
* [JEP 257](http://openjdk.java.net/jeps/257): 更新 JavaFX/Media 中 GStreamer 的版本。
* [JEP 258](http://openjdk.java.net/jeps/258): 使用 HarfBuzz 作为字体布局引擎。
* [JEP 259](http://openjdk.java.net/jeps/259): 定义了一个高效标准的 Stack-Walking API。
* [JEP 260](http://openjdk.java.net/jeps/260): 封装大部分的内部 API。
* [JEP 261](http://openjdk.java.net/jeps/261): 实现模块化系统。
* [JEP 262](http://openjdk.java.net/jeps/262): 支持 TIFF 图像 I/O。
* [JEP 263](http://openjdk.java.net/jeps/263): 实现 Windows 和 Linux 高分辨率图像接口。
* [JEP 264](http://openjdk.java.net/jeps/264): 平台日志 API 和 服务。
* [JEP 265](http://openjdk.java.net/jeps/265): Java 2D 使用 Marlin Graphics Renderer。
* [JEP 266](http://openjdk.java.net/jeps/266): 并发相关的一些更新。
* [JEP 267](http://openjdk.java.net/jeps/267): 支持 Unicode 8.0。
* [JEP 268](http://openjdk.java.net/jeps/268): 支持 XML 目录。
* [JEP 269](http://openjdk.java.net/jeps/269): 增加一些集合类创建的工厂方法。
* [JEP 270](http://openjdk.java.net/jeps/270): 为临界区预留栈的某些区域。
* [JEP 271](http://openjdk.java.net/jeps/271): 统一 GC 日志。
* [JEP 272](http://openjdk.java.net/jeps/272): 增加特定平台的桌面特性。
* [JEP 273](http://openjdk.java.net/jeps/273): Deterministic Random Bit Generator (DRBG) 的实现。
* [JEP 274](http://openjdk.java.net/jeps/274): 增强方法处理器。
* [JEP 275](http://openjdk.java.net/jeps/275): Java 应用模块化打包。
* [JEP 276](http://openjdk.java.net/jeps/276): 语言定义对象模型的动态链接。
* [JEP 277](http://openjdk.java.net/jeps/277): 改善 Deprecation。
* [JEP 278](http://openjdk.java.net/jeps/278): 为 G1 中的巨大对象增加测试。
* [JEP 279](http://openjdk.java.net/jeps/279): 改进测试故障排除。
* [JEP 280](http://openjdk.java.net/jeps/280): 指示字符串串联。
* [JEP 281](http://openjdk.java.net/jeps/281): HotSpot C++ 单元测试框架。
* [JEP 282](http://openjdk.java.net/jeps/282): Java连接器 jlink。
* [JEP 283](http://openjdk.java.net/jeps/283): 在 Linux 上支持 GTK 3。
* [JEP 284](http://openjdk.java.net/jeps/284): 新的 HotSpot 构建系统。
* [JEP 285](http://openjdk.java.net/jeps/285): 自旋等待提示。
* [JEP 287](http://openjdk.java.net/jeps/287): 实现 SHA-3 Hash 算法。
* [JEP 288](http://openjdk.java.net/jeps/288): 禁止 SHA-1 验证。
* [JEP 289](http://openjdk.java.net/jeps/289): 废弃 Applet API。
* [JEP 290](http://openjdk.java.net/jeps/290): 过滤输入的序列化数据。
* [JEP 291](http://openjdk.java.net/jeps/291): 废弃 Concurrent Mark Sweep (CMS) 垃圾收集器。
* [JEP 292](http://openjdk.java.net/jeps/292): 在 Nashorn 中支持 ECMAScript 6 特征。
* [JEP 294](http://openjdk.java.net/jeps/294): Linux/s390x 端口。
* [JEP 295](http://openjdk.java.net/jeps/295): 提前编译。
* [JEP 297](http://openjdk.java.net/jeps/297): 统一 arm32/arm64 端口。
* [JEP 298](http://openjdk.java.net/jeps/298): 移除过时的例子。
* [JEP 299](http://openjdk.java.net/jeps/299): 重新组织文档。 

# JDK 8
[JDK 8](http://openjdk.java.net/projects/jdk8/) 于2014年3月14号发布。从 Java 8 开始开发代号已经弃用了。新特性有:
* Lambda 表达式
* Pipelines 和 Streams
* Date 和 Time API
* Default 方法
* Type 注解
* Nashhorn JavaScript 引擎
* 并发计数器
* Parallel 操作
* 移除 PermGen Error
* TLS SNI

第三个有里程碑意义的 Java 版本。其中最引人注目的便是 Lambda 表达式了，从此 Java 语言原生提供了函数式编程能力。Java 8 更加适应海量云计算的需要。

具体的特性包括：
* [JEP 117](http://openjdk.java.net/jeps/117): 移除注解处理工具（Annotation-Processing Tool，apt）。
* [JEP 124](http://openjdk.java.net/jeps/124): 增强证书撤销检查 API。
* [JEP 130](http://openjdk.java.net/jeps/130): 实现 SHA-224 消息摘要算法。
* [JEP 131](http://openjdk.java.net/jeps/131): 在 64-bit Windows 中支持 PKCS#11。
* [JEP 112](http://openjdk.java.net/jeps/112): Charset 实现改善。
* [JEP 129](http://openjdk.java.net/jeps/129): 实现 NSA Suite B 加密算法。
* [JEP 105](http://openjdk.java.net/jeps/105): DocTree API。
* [JEP 106](http://openjdk.java.net/jeps/106): 扩展 `javax.tools` API 来支持 javadoc 的访问。
* [JEP 113](http://openjdk.java.net/jeps/113): 在 JDK 的 Kerberos 5 中添加 MS-SFU 扩展。
* [JEP 114](http://openjdk.java.net/jeps/114): TLS Server Name Indication (SNI) 扩展。
* [JEP 121](http://openjdk.java.net/jeps/121): 提供更强的 Password-Based-Encryption (PBE) 算法实现。
* [JEP 122](http://openjdk.java.net/jeps/122): 移除永久带（Permanent Generation）。
* [JEP 127](http://openjdk.java.net/jeps/127): 改善 Locale Data Packaging，并且采用 Unicode CLDR Data。
* [JEP 128](http://openjdk.java.net/jeps/128): Unicode BCP 47 本地匹配。
* [JEP 133](http://openjdk.java.net/jeps/133): 支持 Unicode 6.2。
* [JEP 136](http://openjdk.java.net/jeps/136): 增强错误验证。
* [JEP 153](http://openjdk.java.net/jeps/153): 启动 JavaFX 应用。
* [JEP 177](http://openjdk.java.net/jeps/177): 优化 `java.text.DecimalFormat.format`。
* [JEP 103](http://openjdk.java.net/jeps/103): 并行数组排序。
* [JEP 135](http://openjdk.java.net/jeps/135): Base64 编码和解码。
* [JEP 138](http://openjdk.java.net/jeps/138): 基于 Autoconf 的自动构建系统。
* [JEP 139](http://openjdk.java.net/jeps/139): 增强 javac 来提高构建速度。
* [JEP 142](http://openjdk.java.net/jeps/142): 减少对于特定域的高速缓存的争夺。
* [JEP 147](http://openjdk.java.net/jeps/147): 减少类元数据占用。
* [JEP 148](http://openjdk.java.net/jeps/148): 支持小虚拟机（不超过3M）的创建。
* [JEP 149](http://openjdk.java.net/jeps/149): 减少核心库的内存使用。
* [JEP 150](http://openjdk.java.net/jeps/150): 新的 Date 和 Time API。
* [JEP 160](http://openjdk.java.net/jeps/160): lambda 函数表达式。
* [JEP 164](http://openjdk.java.net/jeps/164): 利用 CPU 指令进行 AES 加密。
* [JEP 166](http://openjdk.java.net/jeps/166): 针对JKS、JCEKS、PKCS12秘钥存储的修改。
* [JEP 170](http://openjdk.java.net/jeps/170): JDBC 4.2。
* [JEP 172](http://openjdk.java.net/jeps/172): DocLint。
* [JEP 173](http://openjdk.java.net/jeps/173): 放弃一些很少使用的 GC 组合。
* [JEP 101](http://openjdk.java.net/jeps/101): 泛华目标类型接口。
* [JEP 104](http://openjdk.java.net/jeps/104): 在 Java 类型上加注解。
* [JEP 107](http://openjdk.java.net/jeps/107): 增加集合的批量数据操作。
* [JEP 109](http://openjdk.java.net/jeps/109): 在核心库中增加 Lambda 表达式。
* [JEP 115](http://openjdk.java.net/jeps/115): 认证加密的密码套件。
* [JEP 118](http://openjdk.java.net/jeps/118): 在运行时访问参数名称。
* [JEP 119](http://openjdk.java.net/jeps/119): 通过反射实现  `javax.lang.model.*` API。
* [JEP 120](http://openjdk.java.net/jeps/120): 重复注解。
* [JEP 123](http://openjdk.java.net/jeps/123): 可配置的安全随机数生成。
* [JEP 126](http://openjdk.java.net/jeps/126): lambda 表达式和虚拟扩展方法。
* [JEP 140](http://openjdk.java.net/jeps/140): 限制的 doPrivileged。
* [JEP 155](http://openjdk.java.net/jeps/155): 并发库更新。
* [JEP 161](http://openjdk.java.net/jeps/161): 紧凑版本。
* [JEP 162](http://openjdk.java.net/jeps/162): 为模块化做准备。
* [JEP 171](http://openjdk.java.net/jeps/171): 在 ` sun.misc.Unsafe` 中增加三个内存排序相关的指令。
* [JEP 174](http://openjdk.java.net/jeps/174): Nashorn JavaScript 引擎。
* [JEP 176](http://openjdk.java.net/jeps/176): 提供调用者敏感的检测机制。
* [JEP 178](http://openjdk.java.net/jeps/178): 静态链接的 jni 库。
* [JEP 179](http://openjdk.java.net/jeps/179): JDK API 的文档的支持和稳定。
* [JEP 180](http://openjdk.java.net/jeps/180): 对于频繁冲突的 HashMap 使用平衡树。
* [JEP 184](http://openjdk.java.net/jeps/184): HTTP URL的权限。
* [JEP 185](http://openjdk.java.net/jeps/): 限制外部 XML 资源的获取。

# JDK 7
开发代号是 Dolphin（海豚），于2011年7月28日发行。新特性有：
* `switch` 语句块中允许以字符串作为分支条件；
* 在创建泛型对象时应用类型推断；
* 在一个语句块中捕获多种异常；
* 支持动态语言；
* 支持 `try-with-resources`；
* 引入 Java NIO.2 开发包；
* 数值类型可以用2进制字符串表示，并且可以在字符串表示中添加下划线；
* 钻石型语法；
* `null` 值的自动处理。

这个版本中的主要的特性是 NIO2 和 Fork/Join 并发包，Java 虚拟机的稳定性真正做到的工业级，成为一个计算平台而服务于全世界。

# JDK 6
开发代号为 Mustang（野马），于2006年12月11日发行。新特性有：
* 支持脚本语言；
* 引入 JDBC 4.0 API；
* 引入 Java Compiler API；
* 可插拔注解；
* 增加对 Native PKI(Public Key Infrastructure)、Java GSS(Generic Security Service)、Kerberos 和 LDAP(Lightweight Directory Access Protocol) 的支持；
* 继承 Web Services；
* 做了很多优化。

这个语言语法改进不多，但在虚拟机内部做了大量的改进，成为一个相当成熟稳定的版本，时至今日国内的很多公司依然以 Java6 作为主要 Java 开发版本来使用。

同年 Sun 公司做出一个伟大的决定，将 Java 开源。OpenJDK 从 Sun JDK 1.7 版本分支出去，成为今天 OpenJDK 的基础。

# JDK 5
开发代号为Tiger（老虎），于2004年9月30日发行。新特性包有:
* 引入泛型；
* 增强循环，可以使用迭代方式；
* 自动装箱与自动拆箱；
* 类型安全的枚举；
* 可变参数；
* 静态引入；
* 元数据（注解）；
* 引入 Instrumentation。

Sun 不再采用 J2SE, J2EE 这种命名方式，而使用 Java SE 5, Java EE 5 这样的名称。

Java 5 是第二个里程碑式的版本。Java 语言语法发生很大的变化，如注解 (Annotation)，装箱 (Autoboxing)，泛型 (Generic)，枚举 (Enum)，foreach 等被加入，提供了 java.util.concurrent 并发包。

Java 5 对于 Java 语言的推动是巨大的，特别是注解的加入，使得语言定义灵活了很多，程序员可以写出更加符合领域定义的描述性程序。

# JDK 1.4
开发代号为 Merlin（隼），于2004年2月06日发行（首次在JCP下发行）。新特性有:
* XML 处理；
* Java 打印服务；
* 引入 Logging API；
* 引入 Java Web Start；
* 引入 JDBC 3.0 API；
* 引入断言；
* 引入 Preferences API；
* 引入链式异常处理；
* 支持 IPv6；
* 支持正则表达式；
* 引入 Image I/O slot machine API。

Java 语言真正走向成熟，提供了非常完备的语言特性，如 NIO，正则表达式，XML 处理器等。

同年微软的.NET 框架发布，两者开始了为期十几年的暗自竞争。从语言特性上来说，.NET 后发先至，一直处于优势。但 Java 依赖良好的开发者生态，绝大多数大型软件公司的使用者众多和不断贡献，以及对 Linux 操作系统良好的支持，渐渐的在服务器端获得优势地位。

# JDK 1.3
开发代号为 Kestrel（红隼），于2000年5月08日发行。新特性有：
* 引入Java Sound API；
* jar 文件索引；
* 对 Java 的各个方面都做了大量优化和增强。

J2EE 中的 Servlet 规范获得了极大的成功，伴随着互联网的兴起，和浏览器直接通过 HTTP 协议交互的 Servlet，和众多的 MVC 框架，成为 Web1.0 的网红。

# JDK 1.2
开发代号为 Playground（操场），于1998年12月8日发行。新特性有：
* 引入集合（Collection）框架；
* 对字符串常量做内存映射；
* 引入 JIT（Just In Time） 编译器；
* 引入对打包的 Java 文件进行数字签名；
* 引入控制授权访问系统资源的策略工具；
* 引入 JFC（Java Foundation Classes），包括 Swing 1.0、拖放和 Java 2D 类库；
* 引入 Java 插件；
* 在 JDBC 中引入可滚动结果集、BLOB、CLOB、批量更新和用户自定义类型；
* 在 Applet 中添加声音支持。

Java 第一个里程碑式的版本。JIT（Just in time）编译器技术，使得语言的可迁移性和执行效率达到最优的平衡，同时 Collections 集合类设计优良，在企业应用开发中迅速得到了广泛使用。

Sun 公司把 Java 技术体系分成三个方向，分别是 J2SE（面向桌面和通用应用开发），J2EE（面向企业级应用开发），J2ME（面向移动终端开发）。这个分类影响非常久远，体现出主流语言设计者的思想：针对于不同的应用领域，在形态，API 集合等进行划分。

# JDK 1.1
于 1997年2月19日发行，新特性有：
*  引入JDBC（Java Database Connectivity）；
*  支持内部类；
*  引入Java Bean；
*  引入RMI（Remote Method Invocation）；
*  引入反射（仅用于内省）。

Java 语言的基本形态基本确定了，比如反射 (reflection), JavaBean, 接口和类的关系等等，一直到今天都保持一致。然而，Java 最初的一些目标，如在浏览器中执行 Applet，以及跨平台的图形界面 Awt 很快遭遇到负面的评价。

# JDK 1.0
开发代号为Oak（橡树），于1996年1月23发行。特点有：
* 提供了一个解释执行的 Java 虚拟机；
* Applet 能在 Mozilla 浏览器中运行。

Java 的 Applet 能在 Mozilla 浏览器中运行，被看作是未来的互联网语言。

# 起源
Java 语言源于 1991 年 Sun 公司 James Gosling 领导的的 Ork 项目，1995 年 Sun 公司正式起名为 Java，并提出“Write once, Run anywhere"的口号。
