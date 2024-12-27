
# 一、简介
	当前版本V2.3（本次更新主要增加了一些红队功能）

这款工具是一款功能强大的网络安全综合工具，旨在为安全从业者、红蓝对抗人员和网络安全爱好者提供全面的网络安全解决方案。它集成了多种实用功能，包括解密、分析、扫描、溯源等，为用户提供了便捷的操作界面和丰富的功能选择。

- GitHub链接：[https://github.com/HotBoy-java/PotatoTool/releases/tag/Release](https://github.com/HotBoy-java/PotatoTool/releases/tag/Release)
- 启动命令后+debug，可打印解密报错，用于提交bug信息（例：java -jar xxx.jar debug）
- **启动密码：potato520**
# 二、优势

| 特性 | 说明 |
|:---:|:---:|
| 强大全面 | 每个功能相较于同类型工具更强大，功能支持更全面 | 
| 综合性能 | 一体化设计，用户无需切换工具或界面即可完成各项操作 | 
| 用户友好 | 界面简单友好，操作易上手 | 
| 反馈支持 | 重视用户反馈，提供及时支持和帮助 | 

# 三、使用场景

1. 红蓝对抗
2. 流量监测
3. 流量研判
4. 流量审计
5. ~~CTF竞赛~~  （下个版本）

# 四、运行环境

| 环境 | 说明 |
|:---:|:---:|
| Java版本 | 8 / 11+ (【荐】性能更高) | 
| 兼容平台 | 支持 Windows、Linux 和 Mac 操作系统 | 

# 五、价格与许可

**免费使用**：目前提供的是一个社区版本，完全免费供用户使用。这个版本包含了所有蓝队功能，并且没有任何时间限制，尽情享受工具带来的便利和效益。

**内部版**：这款工具在设计时就注重可扩展性与定制化，旨在贴合用户需求。目前有一个内部版本，具备很多强大功能，但因团队资源问题未充分测试和修补，尚未在公开版推出，后续更新会逐步发布这些功能。

**未来开源计划**：处于规划和筹备阶段，有许多细节需要进一步梳理和完善，比如代码的优化、文档的补充以及确保开源后的维护和支持体系能够稳定运行等，我会在确保用户利益和安全的前提下，谨慎地考虑开源的时机和方式。

# 六、快速入门

## 1. 功能介绍
### 1.1 一键解密，洞悉攻击行为

| 方案类型 | 支持情况 |
|:---:|:---:|
| webshell交互流量 | 支持 | 
| 网络流量包 | 支持 | 
| 多种加密方式混用 | 支持 | 
| 强混淆数据 | 支持 | 
| 组件密文数据 | 支持 | 
| 中间件等配置 | 支持 | 
| 输入格式多样化 | 支持 | 
| 多种Key爆破方式 | 支持（**解密不出来记得尝试更换方式及字典**） | 
| AI分析 | 支持 | 
| ... | ... |

- 支持所有常见webshell交互流量解密

| Webshell管理工具 | 支持情况 |
|:---:|:---:|
| 冰蝎 | 支持 | 
| 蚁剑 | 支持 | 
| 哥斯拉 | 支持 | 
| China Chopper | 支持 | 
| Cknife | 支持 | 
| ... | ... |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/51842bb2ced94d3cb1bc5555cc5653d9.png)

- 支持网络流量包解密

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4a94c303ccc64006ad700ba3d39e5062.png)

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/cbd00bbe27ff47f59367f4ca30f148f4.png)

- 支持自动检测多种加密方式混用解密

| 支持的解密方式 | 说明 | 支持情况 |
|:---:|:---:|:---:|
| AES | 高级加密标准 | 支持 |
| DES | 数据加密标准 | 支持 |
| RSA | RSA公钥加密算法 | 支持 |
| Blowfish | 对称密钥分组密码算法 | 支持 |
| XOR | 异或加密算法 | 支持 |
| SHA1 | 安全散列算法 | 支持 |
| MD5 | 消息摘要算法 | 支持 |
| MD5_16 | MD5的16位哈希 | 支持 |
| Base64 | 常用于编码二进制数据的方法 | 支持 |
| Unicode | 字符编码标准 | 支持 |
| Hex | 十六进制编码方式 | 支持 |
| URL | 统一资源定位符编码方式 | 支持 |
| Html | HTML实体编码方式 | 支持 |
| Rot13 | ROT13替换加密算法 | 支持 |
| Chr | ASCII字符编码 | 支持 |
| strRev | 字符串反转 | 支持 |
| Byte | 字节处理 | 支持 |
| Bcel | Java字节码编辑器 | 支持 |
| Gzip | 数据压缩算法 | 支持 |
| 反序列化 | 将数据从序列化的格式还原回原始格式 | 支持 |
| ... | ... | ... |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e490395b886541d6ab93ca05f5e4edca.png)

- 支持强混淆解密（Unicode多u混淆、log4j强混淆等混淆方式）

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/6ee817cedcfb42eeb0e94a6b4f938458.png)

- 支持常见组件密文数据解密

| 支持的组件 | 支持情况 |
|:---:|:---:|
| Shiro | 支持 |
| Log4j | 支持 |
| Cas | 支持 |
| JWT | 支持 |
| ... | ... |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2c2a950dfdd34cee9663da6ad6e9c79f.png)

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/67653891ffdf4083807d7d7b008b2492.png)

- 支持常见中间件等配置解密

| 支持类型 | 支持情况 |
|:---:|:---:|
| WebLogicDB | 支持 |
| JbossDB | 支持 |
| SpringDB | 支持 |
| DruidDB | 支持 |
| FinalshellDB | 支持 |
| Navicat | 支持 |
| 用友DB | 支持 |
| 致远DB | 支持 |
| 帆软DB | 支持 |
| 蓝凌DB | 支持 |
| 强智DB | 支持 |
| RealorDB | 支持 |
| HrmsDB | 支持 |
| H3CDB | 支持 |
| H3C_imcDB | 支持 |
| IvmsDB | 支持 |
| ... | ... |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/45cc6fc82c094ec2b2be8a6877a4a250.png)

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d4d07775b42e42c68363251e8135f973.png)

- 支持多种用户输入格式

| 支持类型 | 说明 |
|:---:|:---:|
| 纯密文 | 直接输入密文内容 |
| Json请求体 | 例：{"username":"密文","passwd":"密文"} |
| Form Data请求体 | 例：username=密文&passwd=密文 |
| 请求完整包 | 包含请求头部及body内容 |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/743375afd99a441484c69430c12cd233.png)

- 支持多种Key爆破方式

| 支持类型 | 说明 |
|:---:|:---:|
| 默认Key快速解密 | 快速解密 |
| 指定Key快速解密 | 用户输入Key值进行解密 |
| 使用内置50万Key字典解密 | 只适用于webshell，字典较大，速度慢 |
| 指定Key字典解密 | 用户加载本地Key字典进行解密 |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4a53e4eec5d74d228709432e01c5396d.png)

- AI分析恶意脚本

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/e3f5d99e23d0d4767801f30bb88de3e8.png)

	结果若是不满意，可点击刷新重新获取AI分析结果

### 1.2 专项加解密

- 指定专项解密，由【一键解密】单独提出来的部分加解密方法

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/5d1a1e054f2530466ee10703fd023b40.png)

### 1.3 IP筛选

- 支持多种展示形式

| 展示形式 | 支持状态 |
|:---:|:---:|
| IP提取 | 支持 |
| IP提取+归属地查询 | 支持 |
| 原文高亮IP | 支持 |
| 原文高亮IP+注明归属地 | 支持 |

- 支持自定义筛选

| 支持类型 | 支持状态 |
|:---:|:---:|
| 自定义筛选 | 支持 |
| 国内外IP分类 | 支持 |
| 内外网IP分类 | 支持 |
| 地区区域分类 | 支持 |

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/90c29f7e0476207b59e0fca4823401d7.png)

### 1.4 AI分析

- 默认采用自带的AI模型

		致力于提供优质的人工智能体验。然而，由于资金有限以及软件免费的性质，默认的AI模型可能存在一些性能上的局限性（为保留算力，暂留5轮会话记忆）。
		后续可能因资金或用户恶意行为导致暂停自带AI功能。

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/9865aa816d65767d87f6c0e970b3eca5.png)

- 可手动配置ChatGPT

		右上角设置 -> 配置GPT_Model、GPT_API_Key -> 保存

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e5e404327ac14acbbe63ed14e3467103.png)

### 1.5 反编译

- 支持的反编译器

| 支持类型 | 支持状态 |
|:---:|:---:|
| idea | 支持 |
| procyon | 支持 |

		设置中可配置默认反编译器

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/18f0817568935b2e45b02847e2aaef87.png)

- 版本计划

		支持批量反编译

### 1.6 区块链溯源
- 支持钱包地址查询

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4d802a6560624d0f8451dbae8fcc6eab.png)


- 支持交易hash查询

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/d21398b6b28278df43e3f963832f4215.png)

- 支持区块ID查询

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d7354cad1d5b41c88941f9468c41ed7e.png)


- 支持名词解释查询

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/70ae56692a88ccf6cf7bb47d88d4b3bd.png)
### 1.7 归属地查询

| 特性 | 描述 |
|:---:|:---:|
| 支持类型 | 银行卡归属地免费批量查询、手机号归属地免费批量查询。 |
| 支持广泛 | 涵盖超过2000家银行，可精准查询银行卡具体归属地或支行，以及手机号的运营商和省市信息。 |
| 数据筛选 | 提供强大的数据筛选功能，包括数据去重和元素筛选，帮助用户快速处理和分析大量查询结果。 |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/74cfeee4b746410a9b4fbff0b7e27ed0.png)

### 1.8 文件元信息提取

- 支持多种文件元信息提取，若存在GPS信息，则进行经纬度逆编码，查询具体定位。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/7d6d6337324e47958a3dc4be51308c5e.png)

### 1.9 扩展模块

- 综合性高，提供全面的资源指南，点击即可访问

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/2224cafe73b50f525f918a00e84e15ab.png)

- 具有可自定义性，根据个人需求，添加**快捷指令** 或 网站导航

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/d2239add167e5dd80a9a21ff16834866.png)

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/2bfd6bb1093dfd6f30310be2e63cc657.png)

	如果需要需要大批量修改\删除，可直接在
	【Windows】%USERPROFILE%\.PotatoTool\config.json
	【Linux\Mac】$HOME/.PotatoTool/config.json
	文件中按格式修改
### 1.10 信息收集

| 特性 | 描述 |
|:---:|:---:|
| 支持测绘平台 | Fofa、Hunter、Quake、ZoomEye、Shodan |
| 数据聚合化 | 支持同时使用多方平台检索数据，并进行聚合整理 |
| 智能扩散搜索 | 开启后，将自动对查询的信息进行智能扩散搜索，包括对公司名称进行检索，并拓展至图标、域名、证书、C段等关键信息的深度搜索 |
| 敏感信息检索 | 针对已完成全量探测的资产进行敏感信息探测，并通过搜索引擎及仓库检索信息泄露 |
| 清洗与标准化 | 提供强大的数据清洗功能，确保数据整洁有序 |
| 重复数据过滤 | 通过改进的算法，快速准确地过滤重复数据，包括相似数据的智能识别 |
| 智能脏数据过滤 | 利用先进的机器学习算法，实现智能化的脏数据过滤，确保数据质量。有效解决模糊检索影子资产时，杂数据影响 |

| 支持类型 | 支持状态 |
|:---:|:---:|
| 域名 | 支持 |
| IP | 支持 |
| 公司名称（中国） | 支持 |

- 流程图（愿网安界越来越好）

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/589e28029c63424ca2680bb2777b8edb.png)

**本流程由于 API 访问频率限制，免费版和个人会员版API_Key的检索能力可能受到影响，导致部分资产或流程无法完整执行。建议升级为企业版API 配额，从而实现全面的检索覆盖。**

- 智能检索

使用本功能时注意：

	1、【启动jar前（本工具）】，本地不要开系统代理（启动后关闭也不行）
	2、【本工具设置】中打开代理功能

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/5b1e05a4cdf444b3a844dffede8ec5cf.png)

- 公司或个人详情（含企业及符合权重的子公司的域名、网站、工商、软著、备案、微信公众号、App、权重比等信息）

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/dfe4a724d55243bcaf713e8e546ee451.png)

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/1fbe478b36d74a98ad8370a711f80430.png)

- 具体资产汇总

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/fb5dd9cca0214f77882a24588590bc52.png)

- 敏感信息汇总

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/5a27473a3333444a944f7433c51811ee.png)

- 信息泄露汇总

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4a8aefc469f34a0087fef99fa206472a.png)

### 1.11 漏洞扫描

- 测试版未公开，代码兼容性Bug修复中

| 特性 | 描述 |
|:---:|:---:|
| 内置POC脚本 | 工具内置了大量的POC脚本，覆盖了多种漏洞类型和攻击场景 |
| 高度语言兼容性 | 支持python、json(内测中)、yarm的POC |
| 高度代码兼容性 | 支持用户提供不规范的POC(暂支持python)，智能调用不规范的POC并获取不规范的输出，智能判断是否存在对应漏洞 |

### 1.12 免杀
- 免杀webShell

	公开版，具有时效性，后续迭代更新（v2.3暂未更新该功能），满足部分人需求
	测试版，暂未公开，高频率更新，维护资源有限

| 特性 | 描述 |
|:---:|:---:|
| 涉及工具 | Godzilla、Behinder、AntSword |
| 支持语言 | JSP、JSPX、PHP、ASP、ASPX |
| 支持混淆 | Base64、AES、RAW、XOR、Unicode、CSHARP、Reflect |
| 自定义型 | 自定义webShell密钥，key默认potato，(pass不变) |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/1ee72ccdc32f49febf0d149c3d0e4fe9.png)

- 伪造签名

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c56d5fb1ddc34704bb42b849701059a9.png)

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2b01cd15c0f84113b043a372d65a3f9a.png)

- 钓鱼二维码生成

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/28f9639f9bf34e3dba1e14559221a37e.png)

- 加壳（Potato壳）[暂未开放]

| 加密方案 | 支持状态 |
|:---:|:---:|
| 导入表保护 | 支持 |
| 内存校验 | 支持 |
| 压缩 | 支持 |
| 资源节加密 | 支持 |
| 调试器检测 | 支持 |
| 虚拟机检测 | 支持 |
| 自定义加密 | 支持(Bug) |

| 函数保护方案 | 支持状态 |
|:---:|:---:|
| 排除关键函数 | 支持(Bug) |
| 代码混淆 | 支持 |
| 代码虚拟化 | 支持 |
| 代码加密 | 支持 |
### 1.13 自定义内存码

| 特性 | 描述 |
|:---:|:---:|
| 支持广泛 | 支持包括Tomcat、Resin、Jetty、WebLogic、WebSphere、Undertow、GlassFish、SpringMVC以及SpringWebFlux等主流中间件和框架 |
| 支持类型 | Filter/Listener/Interceptor/HandlerMethod |
| 支持工具 | Godzilla、Behinder、AntSword |
| 支持高度自定义 | 支持自定义密钥、请求头、类名、路由路径、输出格式、封装类型 |

	特此声明：该功能是二开jMG，这部分代码不做混淆

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/ca4bed2c0b044409b910da2fa070c27f.png)

### 1.14 命令生成

| 特性 | 描述 |
|:---:|:---:|
| 支持类型 | 支持反向shell、正向shell、MSFVenom、HoaxShell、内网代理、文件下载、痕迹清理命令生成，满足渗透测试和攻击需求，提供一站式解决方案 |
| 自定义化 | 可根据特定环境输入IP和端口，系统根据参数生成多种定制化方案，确保适用性和灵活性 |
| 防检测化 | 支持添加编码防止检测，在一定程度上提高生成Payload的免杀能力，确保攻击效果 |
| 常用命令检索 | 支持对常用的内网横向攻击系统命令进行模糊检索，方便用户快速获取所需信息 |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/a42c84a2eaec4cc88f0fa22e1c092001.png)

### 1.15 命令查询

| 特性 | 描述 |
|:---:|:---:|
| 内部数据支持 | 集成系统指令、安全测试、横向移动、权限管理及渗透工具类命令 |
| 智能化解答 | 基于 AI 引擎，对未收录命令提供智能解答和使用指导（问题中尽可能不要出现空格） |
| 语法兼容 | 支持精确匹配(双引号)、OR 检索(空格)、首尾匹配(^/$)、大小写不敏感 |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/a14d3aa2b4db465292694e51285aa966.png)

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b6987d5435ff4d7aae89748ce3146e44.png)

**内部库中检索无结果才会触发智能化解答哦**

### 1.16 KB提权查询

| 特性 | 描述 |
|:---:|:---:|
| 查询提权信息 | 检查已安装的KB编号，展示存在的提权漏洞的详细信息，包括发布日期、CVE编号、KB编号、标题、影响产品、影响组件、严重性、漏洞影响、替代KB编号、漏洞利用方法 |
| 平替KB检测 | 通过对比是否已存在可替换的KB编号，剔除不存在的提权漏洞信息，减少误报，提高信息准确性 |
| 自定义筛选 | 可根据特定情况，自定义筛选/过滤条件，如影响产品、影响组件、严重性、是否存在漏洞利用等标准，减少误报，提高信息准确性 |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/7e0a026da7944a9495c0bd635c43e7d2.png)
	**若大量存在漏洞，尽可能不要选用检测平替KB编号（会挨个编号检测是否存在平替），会特别耗时。**

- 支持在线更新KB本地库

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f199100114bd42bf84fb8e3c6da8879f.png)

### 1.16 进程分析

| 特性 | 描述 |
|:---:|:---:|
| 杀软进程检测 | 自动检索当前系统中已安装的杀软，并列出其对应的进程信息 |
| 其他进程检测 | 分析输入的进程信息，检索可能存在提权或深度利用的进程，并提供相关信息 |
| 系统兼容性 | 支持Windows\Linux |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/0e44b1ebf2be472b83583b2028a4e3af.png)

-	后续会在设置中支持在线更新进程列表库，收录更多全面信息

### 1.17 信息生成

| 特性 | 描述 |
|:---:|:---:|
| 支持类型 | 个人信息、通讯信息、单位组织信息、银行卡信息 |

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/477c8e8740fb4d9399125f5d715a3257.png)

## 2. 使用技巧

### 2.1 窗口菜单

- 为所有窗口文本添加右键菜单，以便用户可以方便地进行全选、复制等操作。

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/1ef6943640a0a0d0dfa41b1f6fc52038.png)

### 2.2 个性化设置

- 用户可自定义配置代理(支持http\socks)、反编译器和AI模型、在线更新本地配置库

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/396009733c778c780999f9074ac531cb.png)
# 七、常见问题：


	Q:Mac系统arm架构，无法运行
	A:下载有javafx组件的jdk，比如zulu版本的jdk：[https://www.azul.com/downloads/?package=jdk-fx#zulu](https://www.azul.com/downloads/?package=jdk-fx#zulu)
	
	Q:运行后闪退，cmd窗口报错：Java 堆内存溢出（OutOfMemoryError）
 	A:增加 Java 虚拟机的堆内存大小，运行 jar 时添加 JVM 参数：java -Xmx2048m -jar PotatoTool-1.3-jdk8.jar  ，若报错：Error occurred during initialization of VM Could not reserve enough space for 2097152KB object heap，表明系统无法为 Java 虚拟机分配足够的内存空间，需要降低分配的内存大小，比如将2GB内存改为1GB：java -Xmx1024m -jar PotatoTool-1.3-jdk8.jar


  	Q:一键解密一直失败
   	A:可能该密文采用了个性化的Key进行加密，我们需要爆破Key，所以需要更换解密方式，比如选择内置50w字典（专门用于webshell的md5前16位）爆破，非webshell的爆破key，建议自行上传字典。若还是失败，可以和作者沟通讨论一下，完善工具


  	Q:UI界面显示不全
   	A:因界面采用DPI自适应，且未测试不常见的分辨率，所以导致部分分辨率显示异常，建议更换分辨率尝试。


	Q:内测版能公布么
 	A:内部版暂不对外开放，UI上有很多bug，功能上也没有进行全面测试。但是后面会陆续开放，不会存在收费问题。V1版本号开头为蓝队版本、V2版本开头为红蓝队全功能版本、版本号结尾单数为发布版、版本号结尾双数为内测版


	Q:无法输入中文
 	A:Arch Linux中可能存在JavaFX在Linux下的文本框不能输入中文，Java启动时加入-Djdk.gtk.version=2   如：java -Djdk.gtk.version=2 -jar xxxx.jar
  

	Q:自带的AI,交互问答时，在询问关于POC编写等敏感信息时拒绝回答
 	A:模型暂未添加sa，后续会对内置模型进行针对性sa训练，临时解决办法是根据网上bypass方案进行询问（注意，因资源有限，且使用人较多，故服务端未开启上下文对话模式）【因资源问题，优化周期比较久】

# 八、建议/bug提交：

[https://github.com/HotBoy-java/PotatoTool/issues](https://github.com/HotBoy-java/PotatoTool/issues)

# 九、获取方式

- GitHub链接：[https://github.com/HotBoy-java/PotatoTool/releases/tag/Release](https://github.com/HotBoy-java/PotatoTool/releases/tag/Release)
- 推荐使用java11+，性能更高
- 启动命令后+debug，可打印解密报错，用于提交bug信息（例：java -jar xxx.jar debug）
- **启动密码：potato520**

## 帮宝子点个star吧，Stargazers over time
[![Stargazers over time](https://starchart.cc/HotBoy-java/PotatoTool.svg?variant=adaptive)](https://starchart.cc/HotBoy-java/PotatoTool)

