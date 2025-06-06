# <font color=red>**Windows11 Penetration Suite Toolkit within Kali Linux v6.0**</font>
![image](https://img.shields.io/badge/Author-Makoto56-blueviolet.svg) ![image](https://img.shields.io/badge/Platform-Windows-red.svg) ![image](https://img.shields.io/badge/WSL-Kali-9cf.svg) ![image](https://img.shields.io/badge/Property-%E6%AD%A6%E5%99%A8%E5%BA%93-brightgreen.svg)

## <font color=blue>**✨ 更新说明:**</font>

1. **考虑到微软即将对 Windows 10 结束技术支持, 故使用 Windows 11 母盘制作;**
2. **所有运行库、系统组件、安装软件、脚本类工具均升级至最新版本, 并备注了对应的网站及版本号;**
3. **去除部分长期未更新、使用效果不佳的工具, 补充了部分实用工具;**
4. **优化扫描器、数据库等部分工具自启动后台服务占用系统资源过大的问题;**
5. **重构工具的快捷方式，运行时显示详细使用参数及方法，并尽量为每一款工具配备相对好看的图标;**
6. **Python 类工具的说明:**
  - **`由于一些比较老的工具不兼容 python3.13 新版本的 pip 库, 且 Windows 共存不同版本的 python3 容易产生环境变量冲突问题, 所以在 WSL Kali 中同时安装了 python2、python3.8、python3.13 三个版本。`**
  - **`为降低不同工具间依赖库的冲突问题, 本镜像所有 python3 工具的 pip 依赖库均以虚拟环境形式安装 (python3 -m venv) 在项目根目录下 (Windows 为 “win” 文件夹, WSL Kali 为“kali” 文件夹)。使用前需要先激活对应的虚拟环境, 否则会报错缺少运行库。`**
  - **`本镜像所有 python 工具均配备了 start.bat 快速启动脚本, 会根据工具需求调用不同版本的 python 并自动激活对应的虚拟环境, 方便一键使用。如果您需要手动运行, 请确保先激活对应的虚拟环境。`**

## <font color=blue>**📝 系统简介:**</font>

1. **基于 Windows11 Workstation 24H2 x64 原版镜像制作<font color=red>(理论不支持 ARM 设备)</font>**;
2. **完整安装 WSL2 Kali Linux 2025.1;**
  - **注: 物理主机须支持 CPU 虚拟化功能, 否则 WSL Kali 可能无法使用。</font>**
  - <font color=green>**`开启 VMware - 虚拟机设置 - 处理器 - 虚拟化引擎:`**</font>
  - <font color=green>**`虚拟化 Intel VT-x/EPT 或 AMD-V/RVI`**</font>
  - <font color=green>**`虚拟化 CPU 性能计数器`**</font>
  - <font color=green>**`虚拟化 IOMMU(IO 内存管理单元)`**</font>
3. **精简系统自带软件, 美化字体及部分图标, 适度优化;**
  - **`推荐运行环境: `**
  - **`VMware: 17.x(建议视情分配图形内存)`**
  - **`运行内存: 8 GB`**
  - **`固态硬盘: 300 GB`**

## <font color=blue>**📜 制作声明:**</font>

1. **本集成环境根据个人工作和学习的侧重点制作, 不可能做到满足所有人的需求；**
2. **本项目制作的初衷是帮助渗透新手快速搭建工作环境, 工欲善其事, 必先利其器；**
3. **本项目不接受任何形式的商业赞助；**
4. **如果您有好的意见或者建议, 请联系邮箱 `burpsuite@qq.com`。**

## <font color=blue>**⚠️ 免责声明:**</font>

1. **本镜像仅面向合法授权的企业安全建设行为, 如您需要测试本镜像, 请自行搭建环境；**
2. **在使用本镜像时, 您应确保相关行为符合当地的法律法规, 且已经取得了足够的授权；**
3. **如果您在使用本镜像中产生任何非法行为, 需自行承担相应后果, 作者不承担任何法律连带责任；**
4. **本镜像所使用的工具资源均来自于互联网整理, 如果侵犯了您的知识产权, 作者将第一时间删除。**

## <font color=blue>**🖥️ 软件及工具介绍:**</font>

### <font color=orange>**[+] AI工具 (C:\Penetration\AiTools) :**</font>

1. **[CherryStudio](https://www.cherry-ai.com/): AI 资源聚合工具 v1.3.12**
2. **[Cursor](https://www.cursor.com/cn): AI 代码编辑器 v0.50.5**
3. **[腾讯 IMA 知识库](https://ima.qq.com/): v1.72**
4. **[Ai PPT](https://www.aippt.cn/)**
5. **[ChatGPT](https://chat.openai.com/)**
6. **[DeepSeek](https://chat.deepseek.com/)**
7. **[Genspark](https://www.genspark.ai/)**
8. **[Google Gemini](https://gemini.google.com/app?hl=zh)**
9. **[Kimi](https://www.kimi.com/)**
10. **[PentestGPT](https://pentestgpt.ai/)**
11. **[Venice](https://venice.ai/)**
12. **[即梦 AI](https://jimeng.jianying.com/)**

### <font color=orange>**[+] 安卓工具 (C:\Penetration\AndroidTools):**</font>

1. **[AdbDriver](https://adb.clockworkmod.com): ADB 驱动 v1.0.31**
2. **AndroidHelper: APK 逆向工具 v2.2**
3. **AndroidKiller: APK 综合工具 v1.3.1.0**
4. **[Apk2url](https://github.com/n0mi1k/apk2url): APK 信息提取工具 v1.2**
5. **[APKDeepLens](https://github.com/d78ui98/APKDeepLens): APK 扫描工具 v1.0**
6. **[Apkinfo](https://github.com/bihe0832/Android-GetAPKInfo): APK 分析工具 v2.0.2**
7. **[Apkleaks](https://github.com/dwisiswant0/apkleaks): APK 扫描工具 v2.6.3**
8. **[ApkScan-PKID](https://github.com/Bin4xin/Awesome-APKScan-PKID): APK 查壳工具 v1.0**
9. **[Apktool](https://github.com/iBotPeaches/Apktool): APK 反编译工具 v2.11.1**
10. **[ApkToolPlus](https://github.com/linchaolong/ApkToolPlus): APK 反编译分析工具**
11. **[AppMessenger](https://github.com/sulab999/AppMessenger): APK 分析工具 v4.6.3**
12. **[BlueStacks](https://www.bluestacks.com): 蓝叠模拟器(国际版) v5**
  - <font color=green>**`已安装`**</font>
  - **`Debug Proxy`**
  - **`Dev Tools`**
  - **`Http Canary`**
  - **`MT Manager`**
  - **`Net Capture`**
  - **`Packet Capture`**
  - **`Terminal Emulator`**
13. **[BytecodeViewer](https://github.com/Konloch/bytecode-viewer): 字节码查看工具 v2.13.1**
14. **[Dextools](https://github.com/pxb1988/dex2jar): Dex 打包工具 v2.4**
15. **[Jadx-GUI](https://github.com/skylot/jadx): 反编译工具 v1.5.1**
16. **[JavaDecompiler](https://github.com/java-decompiler/jd-gui): 字节码查看工具 v1.6.6**
17. **[SuperJadx](https://github.com/pkilller/super-jadx): 反编译工具 v10.0**
18. **[Yaazhini](https://www.vegabird.com/yaazhini/): APK 漏洞扫描工具 v2.0.2**

### <font color=orange>**[+] 免杀工具 (C:\Penetration\AntivirusTools):**</font>

1. **[AVevasion](https://github.com/1y0n/av_evasion_tool): v20231208**
2. **[AvEvasionCraftOnline](https://github.com/yutianqaq/AVEvasionCraftOnline): v1.2**
3. **[Aycvxz](https://gitee.com/lsgsd/aycvxz-pubilc): 分离免杀工具 v1.4.2**
4. **[BypassAV](https://github.com/yinsel/BypassAV): v1.6**
5. **[Charlotte](https://github.com/9emin1/charlotte): v1.1**
6. **[Invoke-Obfuscation](https://github.com/danielbohannon/Invoke-Obfuscation): v1.0**
7. **[Invoke-Obfuscation-Bypass](https://github.com/komomon/Invoke-Obfuscation-Bypass): v1.0**
8. **[LoaderFly](https://github.com/wangfly-me/LoaderFly): v2.0**
9. **[MaLoader](https://github.com/lv183037/MaLoader): 基于 Tauri + Rust 免杀马生成工具 v1.1**
10. **[RingQ](https://github.com/T4y1oR/RingQ): 后渗透免杀工具**
11. **[Sandboxie](https://www.ghxi.com/sandboxie.html): 沙盒工具 v5.70.12**
12. **[SGN](https://github.com/EgeBalci/sgn): 编码工具 v2.0.1**
13. **[S-inject](https://github.com/Joe1sn/S-inject/): 注入免杀工具 v2.2**
14. **[VMProtect](http://www.dayanzai.me/vmprotect.html): v3.8.4(注册版)**
15. **[VProtect](https://ghxi.com/vprotect.html): 加壳工具 v2.1.0**

### <font color=orange>**[+] 审计工具 (C:\Penetration\AuditTools):**</font>

1. **Fortify: v24.4.0(注册版)**
2. **[PHPAuthScanner](https://github.com/caigo8/PHPAuthScanner): PHP 鉴权代码扫描器 v1.1**
3. **[Seay](https://github.com/f1tz/cnseay): Seay 源代码审计系统 v2.1**
4. **SeayDzend**

### <font color=orange>**[+] 连接工具 (C:\Penetration\ConnectTools):**</font>

1. **[1Remote](https://github.com/1Remote/1Remote) v1.2.0**
2. **[Anydesk](https://www.ghxi.com/anydesk.html) v9.5.4**
3. **[AweSun](https://sunlogin.oray.com/): 向日葵 v15.8.4**
4. **[Filezilla](https://www.ghxi.com/filezilla.html) v3.69.0**
5. **[Finalshell](https://www.hostbuf.com/) v4.5.12**
6. **[PuTTY](https://www.putty.org/) v0.83**
7. **[Teamviewer](https://www.teamviewer.com/) v15.66.5**
8. **[ToDesk](https://www.todesk.com/) v4.7.7.2**
9. **[WinSCP](https://www.ghxi.com/winscp.html) v6.5.1**
10. **[Xftp](https://www.netsarang.com/en/free-for-home-school/) v8.0(教育版)**
11. **[Xshell](https://www.netsarang.com/en/free-for-home-school/) v8.0(教育版)**

### <font color=orange>**[+] 破解工具 (C:\Penetration\CrackTools):**</font>

1. **Advanced Archive Password Recovery: 压缩包密码破解工具**
2. **Advanced Office Password Recovery: Office 密码破解工具**
3. **Advanced PDF Password Recovery: PDF 密码破解工具**
4. **DecryptPassword**
  - <font color=green>**文件夹下集成下列工具**</font>
  - **[`FinalShellPassMassDecode`](https://github.com/EstamelGG/FinalShellPassMassDecode) v1.0**
  - **[`Firefox_decrypt`](https://github.com/unode/firefox_decrypt) v1.1.1**
  - **[`Hack-browser-data-windows`](https://github.com/moonD4rk/HackBrowserData) v0.4.6**
  - **[`PassGet`](https://github.com/adeljck/PassGet)**
  - **[`SharpDecryptPwd`](https://github.com/RowTeam/SharpDecryptPwd) v2.3.0**
  - **[`TeamView_get_Password`](https://github.com/wafinfo/TeamViewer) v1.0**
  - **[`Teamviewer-dumper`](https://github.com/attackercan/teamviewer-dumper) v1.0**
  - **[`VcenterExsi_PwdDecrypt`](https://github.com/jas502n/VcenterExsi_PwdDecrypt) v1.0**
5. **[DecryptTools](https://github.com/wafinfo/DecryptTools): 加解密综合利用工具 v3.1**
6. **[e0e1-config](https://github.com/eeeeeeeeee-code/e0e1-config): 密码抓取解密工具 v1.30**
7. **[Hashcat](https://hashcat.net/hashcat/): 密码破解工具 v6.2.6**
8. **[Hydra](https://github.com/vanhauser-thc/thc-hydra): 密码破解工具 v9.1**
9. **[John](https://www.openwall.com/john/): 密码破解工具 v1.9.0**
10. **[Johnny](https://openwall.info/wiki/john/johnny): John 图形化版本 v2.2**
11. **[Kraken](https://github.com/jasonxtn/Kraken): 密码暴力破解工具**
12. **MD5Crack: MD5碰撞工具 v1.0**
13. **[Web Browser Pass View](https://www.nirsoft.net/utils/web_browser_password.html): 浏览器密码抓取工具**
14. **[SNETCracker](https://github.com/shack2/SNETCracker): 超级弱口令检测工具 v1.0**
15. **WebshellCrack: K8 一句话木马密码破解工具**
16. **[Week-Passwd](https://github.com/BBD-YZZ/week-passwd): 弱口令检测工具 V2.0**

### <font color=orange>**[+] 夺旗工具 (C:\Penetration\CTFTools):**</font>

1. **ASCII: ASCII 码转换工具**
2. **Audacity: 音频工具**
3. **BehinderDecode: 冰蝎流量解码工具**
4. **[BerylEnigma](https://github.com/ffffffff0x/BerylEnigma): 密码学工具 v1.15.0**
5. **[Binwalk](https://github.com/ReFirmLabs/binwalk): 文件分析工具 v3.1.0**
6. **[Blind_Watermark](https://github.com/guofei9987/blind_watermark): 盲水印工具 v0.2.1**
7. **[CaptfEncoder](https://github.com/guyoung/CaptfEncoder): 密码学工具 V2**
8. **[Ciphey](https://github.com/Ciphey/Ciphey): 全自动解密工具 V5.14.0**
9. **Converter: 编码转换工具**
10. **CRCCalculator: CRC 计算工具**
11. **[CTFCrack](https://github.com/0Chencc/CTFCrackTools): CTF 工具框架 v2.1**
12. **[CTFCrackTools](https://github.com/0Chencc/CTFCrackTools): CTF 工具框架 v4.0.7**
13. **CTFEditor: 随波逐流 CTF 工具**
14. **[CTFTools](https://github.com/qianxiao996/CTF-Tools/): 密码学工具 v1.3.7**
15. **[CyberChef](https://github.com/gchq/CyberChef): 密码学工具 v10.19.4**
16. **DesTool: DES 加解密工具**
17. **FindFlag: Flag 查找工具**
18. **[Foremost](https://github.com/korczis/foremost): 分离工具**
19. **GifTools: GIF 图片工具**
20. **[GNUplot](http://www.gnuplot.info/): 数学绘图工具 v6.0.2**
21. **JPHS: 图片隐写工具**
22. **[LSB-Steganography](https://github.com/RobinDavid/LSB-Steganography): 图片隐写工具**
23. **MossTool: 摩斯密码转换工具**
24. **[MP3Steno](https://github.com/MIUIEI/MP3Steno): 音频隐写工具**
25. **[Outguess](https://github.com/crorvick/outguess): 隐写工具**
26. **PcapTool: 流量分析工具**
27. **[PixelJihad](https://github.com/oakes/PixelJihad): 图片隐写工具**
28. **PixRecovery: 图片修复工具**
29. **PNGCalculator: PNG 图片计算工具**
30. **PNGCheck: PNG 图片计算工具**
31. **PNGDebugger: PNG 图片计算工具**
32. **PYGTools: 飘云阁密码学工具**
33. **QRCode: 二维码批量扫描工具**
34. **QRResearch: 二维码解析工具**
35. **Regular: 正则工具**
36. **RSATool: RSA 计算工具**
37. **SM4: SM4 加解密工具**
38. **[Stegdetect](https://github.com/abeluck/stegdetect): 隐写工具**
39. **[Steghide](https://github.com/StefanoDeVuono/steghide): 隐写工具**
40. **[Stegsolve](https://github.com/Giotino/stegsolve): 隐写工具**
41. **TaowaTool: CTF 工具框架**
42. **[TweakPNG](https://github.com/jsummers/tweakpng): PNG 调整工具**
43. **Ulead GIF Animator: GIF 图片工具**
44. **[wbStego](http://www.bailer.at/wbstego/pr_4ixopen.htm): 图片隐写工具**
45. **WinDecrypto: 密码学工具**
46. **[WinHex](https://www.x-ways.net/winhex/): 十六进制编辑工具**
47. **Xiaokui: 小葵编码工具**
48. **ZZYQR: 二维码解析工具**

### <font color=orange>**[+] 数据库工具 (C:\Penetration\DatabaseTools):**</font>

1. **[Another Redis Desktop Manager](https://github.com/qishibo/AnotherRedisDesktopManager): Redis 客户端 v1.7.1**
2. **[DatabaseTools](https://github.com/Hel10-Web/Databasetools): 数据库综合利用工具 v1.2**
3. **[HeidiSQL](https://www.ghxi.com/heidisql.html): 数据库管理工具 v12.10**
4. **[MariaDB](https://mariadb.org/): Mysql 数据库 v11.7**
  - <font color=green>**`username: root`**</font>
  - <font color=green>**`password: sqladmin`**</font>
  - <font color=green>**`如需使用, 请先运行“开启服务”快捷方式。`**</font>
5. **[Multiple Database Utilization Tools](https://github.com/SafeGroceryStore/MDUT): 数据库综合利用工具 v2.1.1**
6. **[Multiple Database Utilization Tools - Extend](https://github.com/DeEpinGh0st/MDUT-Extend-Release): MDUT 增强版 v1.2.0**
7. **[Navicat](https://www.ghxi.com/navicat17.html): 数据库管理工具(注册版) v17.1.12**
8. **[Neo4j](https://neo4j.com/) v1.6.2**
  - <font color=green>**`username: root`**</font>
  - <font color=green>**`password: sqladmin`**</font>
9. **[Oracle 23ai Free](https://www.oracle.com/cn/database/free/get-started/)**
  - <font color=green>**`username: sys`**</font>
  - <font color=green>**`password: sqladmin`**</font>
  - <font color=green>**`如需使用, 请先运行“开启服务”快捷方式。`**</font>
10. **[OracleShell](https://github.com/jas502n/oracleShell): Oracle 数据库利用工具 v1.0**
11. **[OSS-Browser](https://github.com/aliyun/oss-browser): 数据库管理工具 v1.18.0**
12. **PostgreUtil: Postgresql 数据库利用工具 v1.0**
13. **Redis: Redis 客户端(Kali)**
14. **[SharpsqlTools](https://github.com/uknowsec/SharpSQLTools): sqlServer 利用工具 v41**
15. **[sqLite](https://www.sqlite.org/): sqLite 客户端 v3.13.1**
16. **[sqlKnife](https://github.com/0x727/SqlKnife_0x727): sqlServer 利用工具 v1.2**
17. **[Sqlmap](https://github.com/sqlmapproject/sqlmap): 数据库利用工具 v1.9**
18. **[Sqlmap Studio](https://github.com/xinyikan/sqlmap-studio): 配置 SQLMap 命令**
19. **[SqlmapXPlus](https://github.com/co01cat/SqlmapXPlus): Sqlmap 二开版 v1.6**
20. **[sqlServer 2022](https://www.microsoft.com/zh-cn/evalcenter/download-sql-server-2019): 专业版**
  - <font color=green>**`username: sa`**</font>
  - <font color=green>**`password: sqladmin`**</font>
  - <font color=green>**`如需使用, 请先运行“开启服务”快捷方式。`**</font>
21. **[sqlServer Management Studio 21](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16#download-ssms): sqlServer 管理工具**
22. **[sqlTools](https://github.com/uknowsec/SharpSQLTools): sqlServer 利用工具 v2.0**
23. **[ssqlinjection](https://github.com/shack2/SuperSQLInjectionV1): 超级注入工具 v1.0**
24. **[Sylas](https://github.com/Ryze-T/Sylas): 数据库利用工具**
25. **[TinyRDM](https://github.com/tiny-craft/tiny-rdm/releases/tag/v1.1.10): Redis 客户端 v1.2.3**
26. **[Toad for Oracle](https://www.quest.com/products/toad-for-oracle/): Oracle 客户端 v16.2.98**

### <font color=orange>**[+] 字典工具 (C:\Penetration\DictionaryTools):**</font>

1. **[UserNameDictTools](https://github.com/abc123info/UserNameDictTools): v0.36**
2. **[Social Engineering Dictionary Generator](https://github.com/zgjx6/SocialEngineeringDictionaryGenerator): 社工字典生成工具 v1.2.0**
3. **木头字典生成工具**
4. **品轩字典生成工具**
5. **[Pentestdicts](https://github.com/evilc0deooo/PentesterSpecialDict)**

### <font color=orange>**[+] 磁盘工具 (C:\Penetration\DiskTools):**</font>

1. **[傲梅分区助手](https://www.ghxi.com/aomeipartitionassistant.html) v10.8.1**
2. **[傲梅系统备份](https://www.ghxi.com/aomeibackupper.html) v7.5.0**
3. **[Disk Drill](https://www.cleverfiles.com/): 数据恢复工具(注册版) v5.7.917.0**
4. **DiskGenius: v5.6.1.1580(注册版)**
5. **[SSDFresh](https://www.abelssoft.de/en/windows/system-utilities/ssd-fresh): 磁盘整理工具 v2025.14.0**

### <font color=orange>**[+] 编辑工具 (C:\Penetration\EditTools):**</font>

1. **[010Editor](https://www.ghxi.com/010editor.html): 十六进制编辑工具(注册版) v13.0.1**
2. **[AnyTXT](https://www.ghxi.com/anytxtsearcher.html): 文本搜索工具 v13.2034**
3. **BeyondCompare: 文件对比工具 v5.0.7**
4. **[JsonViewer](https://dadroit.com/download/): Json 查看编辑工具 v3.1**
5. **[Microsoft VS Code](https://code.visualstudio.com/download) v1.100.2**
6. **[myBase](https://www.ghxi.com/mybase.html): 个人数据库编辑工具(注册版) v7.3**
7. **[Notepad++](https://notepad-plus-plus.org/downloads/): 编辑工具 v8.4.4**
8. **PSTConverter: Outlook PST 邮件转换工具**
9. **[SharpSword](https://github.com/OG-Sadpanda/SharpSword): Word 命令行查看工具**
10. **[Sublime Text](https://www.ghxi.com/sublimetext4.html): 编辑工具(注册版) v4.4192**
11. **[ToolsFx](https://github.com/Leon406/ToolsFx): 密码学工具 v1.18.0**
12. **[Typora](https://www.ghxi.com/typora.html): MarkDown 编辑工具(注册版) v1.9.5**
13. **[UltraEdit](https://www.ghxi.com/ultraedit.html): 编辑工具 v2024.3**
14. **[WinHex](https://www.ghxi.com/winhex.html): 16进制编辑工具(注册版) v21.4**
15. **XMind: 思维导图工具(注册版) v25.04**

### <font color=orange>**[+] 漏洞工具 (C:\Penetration\ExploitTools):**</font>

1. **漏洞利用工具**
  - **[Aakian-FaCai](https://github.com/zangcc/Aakian-FaCai): VUE 漏洞扫描工具 v1.0.0**
  - **[AliyunAKTools](https://github.com/mrknow001/aliyun-accesskey-Tools): 阿里云利用工具 v1.3**
  - **AptTools: 综合漏洞利用工具**
  - **[AuxTools](https://github.com/doimet/AuxTools): 漏洞综合利用工具 v5.5.3**
  - **[EquationToolsGUI](https://github.com/abc123info/EquationToolsGUI): 方程式工具包图形界面版 v0.3**
  - **[ExpDemo](https://github.com/yhy0/ExpDemo-JavaFX): 综合漏洞利用工具 v1.9**
  - **[Exp-Tools](https://github.com/cseroad/Exp-Tools): 综合漏洞利用工具 v1.3.1**
  - **[HeapdumpTool](https://github.com/wyzxxz/heapdump_tool): 敏感信息提取工具**
  - **[HVVExploitApply](https://github.com/ExpLangcn/HVVExploitApply): 综合漏洞利用工具 v1.5**
  - **[Hyacinth](https://github.com/pureqh/Hyacinth): 综合漏洞利用工具 v2.0**
  - **[IWannaGetAll](https://github.com/R4gd0ll/I-Wanna-Get-All): OA 漏洞利用工具 v1.4.0**
  - **[JavaChains](https://github.com/vulhub/java-chains): Java Payload 综合生成与利用平台 v1.4.1**
  - **[JDumpSpider](https://github.com/whwlsfb/JDumpSpider): 敏感信息提取工具 v20250409T071858**
  - **[JNDI-Exploit](https://github.com/welk1n/JNDI-Injection-Exploit): JNDI 注入测试工具 v1.4**
  - **[JNDI-Injection-Exploit](https://github.com/welk1n/JNDI-Injection-Exploit): JNDI 注入测试工具 v1.0**
  - **[JNDI-Injection-Exploit-Plus](https://github.com/cckuailong/JNDI-Injection-Exploit-Plus): JNDI 注入测试工具 v2.5**
  - **[Linux Exploit Suggester](https://github.com/The-Z-Labs/linux-exploit-suggester/): Linux 提权工具 v1.1**
  - **[LiqunKit](https://github.com/Liqunkit/LiqunKit_): 综合漏洞利用工具 v1.6.2**
  - **[List Cloud](https://github.com/wgpsec/lc): 云攻击资产梳理工具 v1.1.0**
  - **[Moriarty](https://github.com/BC-SECURITY/Moriarty): Windows 提权工具 v1.2**
  - **[MYExploit](https://github.com/achuna33/MYExploit): 综合漏洞利用工具 v2.0.5**
  - **[Nuclei](https://github.com/projectdiscovery/nuclei): 漏洞扫描利用工具 v3.4.4**
  - **[Poc2jar](https://github.com/f0ng/poc2jar): 综合漏洞利用工具 v0.6.8**
  - **[PotatoTool](https://github.com/HotBoy-java/PotatoTool): 综合利用工具 v2.5**
  - **[R-Knife](https://github.com/qianxiao996/R-Knife): 综合漏洞利用工具 v1.2**
  - **SearchSploit: (Kali)**
  - **[SuperXray](https://github.com/4ra1n/super-xray): Xray 图形化版本**
  - **TheLostWorld: OA 漏洞利用工具 v1.1**
  - **[Unauthorized](https://github.com/xk11z/unauthorized): 未授权漏洞检测工具**
  - **[Windows Exploit Suggester - NG](https://github.com/bitsadmin/wesng): Windows 提权工具**
  - **Wiki: 零组文档库 & 漏洞文档库**
  - **[Xray](https://github.com/chaitin/xray): 漏洞扫描利用工具 v2.0**
  - **[Ysoserial](https://github.com/frohoff/ysoserial): Java 反序列化利用工具 v0.0.6**
2. **EXP & POC : `C:\Penetration\ExploitTools\Vulnerability`**
  - <font color=green>**`漏洞库综合了下列项目, 更多漏洞 EXP & POC 请善用 Everything 搜索:`**</font>
  - **[`CMS-Hunter`](https://github.com/SecWiki/CMS-Hunter)**
  - **[`expHub`](https://github.com/zhzyker/exphub)**
  - **[`Middleware-Vulnerability-Detection`](https://github.com/mai-lang-chai/middleware-vulnerability-detection)**
  - **[`System-Vulnerability`](https://github.com/mai-lang-chai/system-vulnerability)**
  - **[`Vulnerability`](https://github.com/edgesecurityteam/vulnerability)**

### <font color=orange>**[+] 取证工具 (C:\Penetration\ForensicsTools):**</font>

1. **[AlternateStreamView](https://www.nirsoft.net/utils/alternate_data_streams.html): NTFS 数据流工具 v1.58**
2. **[AutoSpy](https://www.autopsy.com/): v4.22.1**
3. **[EvtxECmd](https://ericzimmerman.github.io/#!index.md): Windows 日志分析工具 v1.5.2.0**
4. **[FireKylin](https://github.com/MountCloud/FireKylin): 系统痕迹采集工具 v1.4.0**
5. **[GetInfo](https://github.com/ra66itmachine/GetInfo): 应急响应信息采集 v1.2.1**
6. **Get Win info**
7. **[Gather](https://github.com/wwl012345/gather): Linux服务器信息收集脚本 v1.0**
8. **[GhostWolf](https://github.com/SickleSec/GhostWolf): 内存敏感信息提取工具 v1.1**
9. **[Hawkeye](https://github.com/mir1ce/Hawkeye): 应急响应工具 v3.0**
10. **[Hema](https://www.shellpub.com/): 河马 Webshell 查杀 v1.8.2**
11. **[KunWu](https://github.com/kunwu2023/kunwu): 昆吾 Webshell 查杀 v0.1.0**
12. **[Log Parser](https://www.microsoft.com/en-us/download/details.aspx?id=24659): Windows 日志工具 v2.2**
13. **[Log Parser Lizard](https://lizard-labs.com/log_parser_lizard.aspx): LogParser 图形化工具 v8.7**
14. **[Log Parser Studio](https://techcommunity.microsoft.com/t5/exchange-team-blog/introducing-log-parser-studio/ba-p/601131): LogParser 图形化工具 v3.0**
15. **[LovelyMem](https://github.com/Tokeii0/LovelyMem/): 综合取证工具 v0.95**
16. **[Magnet AXIOM](https://breachforums.cx/Thread-Magnet-Axiom-7-8-crack): 综合取证工具 v8.4**
17. **[MemProcFS](https://github.com/ufrisk/MemProcFS): 内存取证工具 v5.14**
18. **[NTFSStreamsEditor](https://github.com/studycpp/NtfsStreamsEditor): NTFS 数据流工具 v2.0.2**
19. **[NTPWEdit](https://github.com/patrickgill/ntpwedit): SAM 文件编辑工具 v0.5**
20. **[oletools](https://github.com/decalage2/oletools): OLE 文件分析工具 v0.60.2**
21. **[QEMU](https://www.qemu.org/download/): 镜像分析工具 v20250422**
22. **[RegistryExplorer](https://ericzimmerman.github.io/#!index.md): Windows 注册表分析工具 v2.1.0**
23. **[Volatility2](https://github.com/volatilityfoundation/volatility): v2.6.1**
24. **[Volatility3](https://github.com/volatilityfoundation/volatility3): v2.26.0**
25. **[WindowsBaselineAssistant](https://github.com/DeEpinGh0st/WindowsBaselineAssistant): Windows 安全基线加固助手 v1.2.3**
26. **[WindowsLogsAnalysis](https://github.com/dogadmin/windodws-logs-analysis): 日志分析工具 v1.0**
27. **[WinPmem](https://github.com/Velocidex/WinPmem): Windows 内存取证工具 v4.0**
28. **[WxDump](https://github.com/cmluZw/WxDump): 微信取证工具 v1.4.1**

### <font color=orange>**[+] 内网工具 (C:\Penetration\IntranetTools):**</font>

1. **[3Gstudent](https://github.com/3gstudent): 三好学生脚本**
  - **`Homework-of-C-Language`**
  - **`Homework-of-C-Sharp`**
  - **`Homework-of-Go`**
  - **`Homework-of-Powershell`**
  - **`Homework-of-Python`**
2. **AddUser: 添加用户工具**
  - <font color=green>**`文件夹下集成下列工具`**</font>
  - **`bypass`**
  - **`bypass360`**
  - **`CreateHiddenAccount`**
  - **`hidecount`**
  - **`Suborner`**
  - **`vbs`**
3. **[ADExplore](https://learn.microsoft.com/en-us/sysinternals/downloads/adexplorer): LDAP 工具 v1.52**
4. **[ADExplorerSnapshot](https://github.com/c3c/ADExplorerSnapshot.py): LDAP 工具 v1.0**
5. **[ADinfo](https://github.com/lzzbb/Adinfo): 内网信息搜集工具 v20220916**
6. **[BloodHound](https://github.com/SpecterOps/BloodHound): 域渗透分析工具 v7.4.0**
  - <font color=green>**`username: admin`**</font>
  - <font color=green>**`password: Bloodhoundpassword@2025`**</font>
  - <font color=green>**`如需使用, 请先运行“开启服务”快捷方式。`**</font>
7. **[BloudyAD](https://github.com/CravateRouge/bloodyAD): 域渗透利用工具 v2.1.18**
8. **[CrackMapExec](https://github.com/Porchetta-Industries/CrackMapExec): 内网综合利用工具 v5.4.0**
9. **[Cube](https://github.com/JKme/cube): 内网密码爆破漏扫工具 v1.2.9**
10. **[DomainInfoFind](https://github.com/wangfly-me/DomainInfo_Find): 获取域内机器的桌面文件 v1.0**
11. **[DomainTools](https://github.com/SkewwG/domainTools): 域渗透综合利用工具 v1.0**
12. **[EarthWorm](https://github.com/rootkiter/Binary-files): 内网穿透工具 v1.2**
13. **[Evil-WinRM](https://github.com/Hackplayers/evil-winrm): WinRM 利用工具 v3.7**
14. **[FScan](https://fscan.club/): 内网扫描工具 v2.0.1**
15. **[GoExec ](https://github.com/FalconOpsLLC/goexec/): Windows 远程执行多功能工具 v0.1.2**
16. **[GoToHTTP](https://gotohttp.com/): 远控工具 v10.2**
17. **[HackerPermKeeper](https://github.com/RuoJi6/HackerPermKeeper): 权限维持工具 v7.0**
18. **[Hoaxshell](https://github.com/t3l3machus/hoaxshell): 远控工具**
19. **imPacket: 内网协议工具**
  - <font color=green>**`文件夹下集成下列工具`**</font>
  - **[`imPacket-python`](https://github.com/SecureAuthCorp/impacket): v0.13.0**
  - **[`impacket-windows`](https://github.com/maaaaz/impacket-examples-windows) v0.9.17**
  - **[`wmiexec-pro`](https://github.com/XiaoliChan/wmiexec-Pro) v0.3**
20. **[Kerbrute](https://github.com/ropnop/kerbrute): 域枚举爆破工具 v1.0.3**
21. **Ladon: 内网综合利用工具 v12.4**
22. **[LdapAdmin](http://www.ldapadmin.org/): LDAP 工具 v1.8.3**
23. **[LDAPDomainDump](https://github.com/dirkjanm/ldapdomaindump): LDAP 工具 v0.10.0**
24. **[Mimikatz](https://github.com/gentilkiwi/mimikatz): 密码抓取工具**
  - <font color=green>**`文件夹下集成下列工具`**</font>
  - **[`CallBackDump`](https://github.com/seventeenman/CallBackDump)**
  - **[`DumpHash`](https://github.com/Avienma/DumpHash)**
  - **[`GoSecretsDump`](https://github.com/C-Sto/gosecretsdump): v0.3.1**
  - **`HKLM`**
  - **[`Kekeo`](https://github.com/gentilkiwi/kekeo): v2.2.0**
  - **[`LaZagne`](https://github.com/AlessandroZ/LaZagne): v2.4.7**
  - **[`Mimipenguin`](https://github.com/huntergregal/mimipenguin): v2.0**
  - **[`MultiDump`](https://github.com/Xre0uS/MultiDump)**
  - **[`NTDSDumpEx`](https://github.com/zcgonvh/NTDSDumpEx): v0.3**
  - **[`Procdump`](https://learn.microsoft.com/en-us/sysinternals/downloads/procdump): v11.0**
  - **[`Pwdump`](https://www.openwall.com/passwords/windows-pwdump)**
  - **[`Quarkspwdump`](https://blog.quarkslab.com/quarks-pwdump.html)**
25. **[Moonwalk](https://github.com/mufeedvh/moonwalk): Linux 痕迹恢复工具**
26. **[Nacs](https://github.com/u21h2/nacs): 内网扫描工具 v0.0.4**
27. **[NetSpy](https://github.com/shmilylty/netspy): 内网网段探测工具 v0.0.5**
28. **[OpenRDP](https://github.com/lengjibo/RedTeamTools/blob/master/windows/%E5%BC%803389%E5%B7%A5%E5%85%B7/): 开启远程桌面工具**
29. **[PEASS-ng](https://github.com/carlospolop/PEASS-ng): Linux 权限提升工具 v20250601**
30. **[Platypus](https://github.com/WangYihang/Platypus) 反向 shell 工具 v1.5.0**
31. **[PSTools](https://learn.microsoft.com/en-us/sysinternals/downloads/pstools): 微软 psexec 工具 v2.5.1**
32. **[PyStinger](https://github.com/FunnyWolf/pystinger): 流量代理工具 v1.6**
33. **[Qscan](https://github.com/qi4L/qscan): 内网扫描工具 v1.8**
34. **[Railgun](https://github.com/lz520520/railgun): 内网渗透综合利用工具 v2.0.3**
35. **[RedPersist](https://github.com/mertdas/RedPersist): 权限持久化工具 v1.0**
36. **[SearchAll](https://github.com/Naturehi666/searchall): 内网信息收集工具 v3.5.11**
37. **[ScheduleRunner](https://github.com/netero1010/ScheduleRunner): 计划任务利用工具 v1.3**
38. **SharpTools:**
  - <font color=green>**`文件夹下集成下列工具`**</font>
  - **[`CSharp_EventLog`](https://github.com/TryA9ain/CSharp_EventLog): 日志分析工具 v1.1**
  - **[`ListRDPConnections`](https://github.com/Heart-Sky/ListRDPConnections): 远程桌面连接记录枚举工具 v0.0.3**
  - **[`SharpAdiDnsDump`](https://github.com/b4rtik/SharpAdidnsdump): 域 DNS 枚举工具**
  - **[`SharpEventLog`](https://github.com/uknowsec/SharpEventLog): 日志分析工具**
  - **[`SharpHide`](https://github.com/outflanknl/SharpHide): 创建隐藏注册表运行键**
  - **[`SharpHound`](https://github.com/BloodHoundAD/SharpHound): 域渗透分析工具 v2.6.6**
  - **[`SharpNetCheck`](https://github.com/uknowsec/SharpNetCheck): 出网探测工具**
  - **[`SharpRDPLog`](https://github.com/Adminisme/SharpRDPLog): 远程桌面连接记录枚举工具**
  - **[`SharpToken`](https://github.com/BeichenDream/SharpToken): 令牌窃取工具 v1.2**
39. **[Traitor](https://github.com/liamg/traitor): Linux 提权工具 v0.0.14**
40. **[WMIHacker](https://github.com/rootclay/WMIHACKER): WMI 利用工具 v0.6**
41. **[Yasso](https://github.com/sairson/Yasso): 内网渗透综合利用工具 v0.06**

### <font color=orange>**[+] 影音图像 (C:\Penetration\MediaTools):**</font>

1. **Adobe Acrobat DC 2025: PDF 编辑工具(注册版)**
2. **Adobe Photoshop 2025**
3. **[Bandicam](https://ghxi.com/bandicam.html): 屏幕录像工具(注册版) v8.1**
4. **[FormatFactory](https://ghxi.com/formatfactory-2.html): 格式工厂(注册版) v5.20**
5. **[Goldwave](https://www.goldwave.com/): 音频编辑工具 v7.0.2**
6. **[Honeyview](https://www.bandisoft.com/honeyview/): 图片查看工具 v7.17**
7. **[K-Lite Codec Pack](https://codecguide.com/download_kl.htm): 视频解码库 v1895**
8. **[PotPlayer](https://ghxi.com/potplayer.html): 播放器 v1.7**
9. **[Snipaste](https://ghxi.com/snipaste.html): 截图工具 v2.10.6**

### <font color=orange>**[+] 网络工具 (C:\Penetration\NetworkTools):**</font>

1. **[Chrome](https://ghxi.com/chrome.html): 136.0.7103.114 绿色修改版**
  - <font color=green>**`集成插件`**</font>
  - **`Adblock: 广告拦截工具`**
  - **`Adobe Acrobat: PDF 编辑`**
  - **`Charset: 修改网页编码工具`**
  - **`Chrome清理大师: 清理工具`**
  - **`CrapApi: Http 接口调试插件`**
  - **`EditThisCookie: cookie编辑工具`**
  - **`FindSomething: 敏感文件搜集工具`**
  - **`Hack-Tools: 红队综合小工具`**
  - **`Hackbar`**
  - **`Imagus: 图片预览工具`**
  - **`Infinity: 标签页工具`**
  - **`IP address and domain inf: ip & domain 探测工具`**
  - **`IP Whois & Flags Chrome & Websites Rating: whois 探测工具`**
  - **`Neater bookmarks: 书签管理工具`**
  - **`Onetab: 标签管理工具`**
  - **`OWASP Penetration Testing Kit: 浏览器渗透测试工具`**
  - **`Proxy switchyomega: 代理切换工具`**
  - **`Shodan: 端口探测工具`**
  - **`Supercopy: 超级复制`**
  - **`User-Agent Switcher: 浏览头切换工具`**
  - **`Wappalyzer: 网页技术分析工具`**
  - **`WebSocket Test Client: websocket工具`**
  - **`Whatruns: 网页技术分析工具`**
  - **`XSS辅助工具`**
  - **`Yet Another Drag and Go FIX: 链接拖拽工具`**
  - **`图片另存为JPG/PNG/WebP`**
  - **`Toolbox 常用工具`**
  - **`篡改猴`**
    - **[`github-chinese`](https://github.com/maboloshi/github-chinese)**
  - **`草料二维码`**
2. **[Free Download Manager](https://www.freedownloadmanager.org/): 下载工具 v6.25**
3. **[Telegram](https://telegram.org/): v5.14.3**
4. **[百度网盘](https://telegram.org/): v7.36.0.3(绿色版 )**

### <font color=orange>**[+] 办公工具 (C:\Penetration\OfficeTools):**</font>

1. **Office: 2024 专业增强版**
  - **`Word 2024`** 
  - **`Excel 2024`** 
  - **`Powerpoint 2024`** 
  - **`Access 2024`** 
  - **`Onenote 2024`** 
  - **`Outlook 2024`**
2. **WPS: 2023 专业增强版**

### <font color=orange>**[+] 编程工具 (C:\Penetration\ProgramTools):**</font>

1. **[Go](https://go.dev/): v1.24.3**
  - <font color=green>**`修改源为阿里云`**</font>
2. **Java:**
  - **`jdk8: 绿色版, 如有软件需要 jdk8 环境运行可直接调用/jdk1.8.0/bin/java.exe即可。`**
  - **`jdk21: 安装版, 已配置环境变量, 系统默认调用 jdk21。`**
3. **JetBrains: 2025.1(注册版)**
  - **`CLion 2025`**
  - **`DataGrip 2025`**
  - **`GoLand 2025`**
  - **`IntelliJ IDEA 2025`**
  - **`PhpStorm 2025`**
  - **`PyCharm 2025`**
  - **`Rider 2025`**
  - **`RubyMine 2025`**
  - **`RustRover 2025`**
  - **`WebStorm 2025`**
  - <font color=green>**`已禁用自动更新, 专业版激活至2026年9月, 破解补丁到期后会循环激活, 理论上无需手动操作。如遇到激活状态失效, 请按教程手动运行/JetBrains/#Crack# 目录下的破解脚本。`**</font>
4. **[Maven](https://maven.apache.org/): Windows & WSL Kali 同步安装 v3.9.9**
5. **[MinGW64](https://github.com/niXman/mingw-builds-binaries/): v15.1.0**
6. **[Nim](https://nim-lang.org/): v2.2.4**
7. **[Node.js](https://nodejs.org/): v22.16.0**
8. **[Python](https://www.python.org/):**
  - <font color=green>**`修改源为阿里云`**</font>
  - **`python2: 安装包形式安装, python2 命令启动(python2 test.py)`**
  - **`python3: Microsoft Store 直装, python 或 python3 命令启动(python test.py / python3 test.py)`**
  - **`使用 pip 命令调用 python3 pip`**
  - <font color=green>**`由于一些比较老的项目不兼容 python3.13 新版本的 pip 库, 且 Windows 共存不同版本的 python3 容易产生环境变量冲突问题, 所以在 WSL Kali 中同时安装了python2、python3.8、python3.13 三个版本。`**</font>
  - <font color=green>**`由于新版 python3 的特性, 为降低不同项目间依赖库的冲突问题, 本镜像所有 python3 工具的 pip 依赖库均以虚拟环境形式安装 (python3 -m venv) 在项目根目录下 (Windows 为 “win” 文件夹, WSL Kali 为“kali” 文件夹)。使用前需要先激活对应的虚拟环境, 否则会报错缺少运行库。`**</font>
  - <font color=green>**`本镜像所有 python 项目均配备了 start.bat 快速启动脚本, 会根据项目需求调用不同版本的 python 并自动激活对应的虚拟环境, 方便一键使用。如果您需要手动运行, 请确保先激活对应的虚拟环境。`**</font>
9. **[Rust](https://www.rust-lang.org/): v1.87.0**
  - <font color=green>**`修改软件源为中科大`**</font>
10. **[TDM-GCC](https://github.com/jmeubank/tdm-gcc/): v10.3.0**
11. **Microsoft Visual Studio 2022: 社区版**

### <font color=orange>**[+] 逆向工具 (C:\Penetration\ReverseTools):**</font>

1. **[DetectItEasy](https://ghxi.com/die.html): 查壳工具 v3.10**
2. **[dnSpy](https://github.com/dnSpy/dnSpy): .Net 逆向工具 v6.1.8**
3. **exeScope: exe 编辑工具 v6.50**
4. **[Ghidra](https://github.com/NationalSecurityAgency/ghidra): 逆向工具 v11.3.2**
5. **[GhostExplore](https://symantec-ghost-explorer.software.informer.com/): GHO 文件编辑工具 v12.0**
6. **[GreenHelper](https://ghxi.com/gscript.html): 绿化工具 v1.4**
7. **[HashTool](https://github.com/KiyanYang/HashTool): Hash 计算工具 v1.4.0**
8. **[IDAPro](https://ghxi.com/pcida.html): v9.1(注册版)**
9. **[ILSpy](https://github.com/icsharpcode/ILSpy): .Net 逆向工具 v9.1.0**
10. **[OllyDebug](https://ghxi.com/ollydug.html): 吾爱破解修复增强版 v1.10**
11. **[PeiD](https://www.aldeid.com/wiki/PEiD): 查壳工具 v0.95**
12. **SignTool: 签名工具 v1.0**
13. **[UPX](https://upx.github.io/): 加壳工具 v3.95**
14. **[x64Debug](https://ghxi.com/x64_dbg.html): 调试工具 v2025**

### <font color=orange>**[+] 扫描工具 (C:\Penetration\ScanTools):**</font>

1. **Acunetix: v25.1.250204093(注册版)**
  - <font color=green>**`username: admin@awvs.com`**</font>
  - <font color=green>**`password: Admin@awvs.com`**</font>
  - <font color=green>**`如需使用, 请先运行“开启服务”快捷方式。`**</font>
2. **AppScan: v10.8.0(注册版)**
3. **[EasySpider](https://www.easyspider.net/): 爬虫工具 v0.6.3**
4. **Nessus: v2025.04.29(注册版)**
  - <font color=green>**`username: admin`**</font>
  - <font color=green>**`password: password`**</font>
  - <font color=green>**`如需使用, 请先运行“开启服务”快捷方式。`**</font>
  - <font color=green>**`Nessusd 服务开启后会自动编译插件, 期间 CPU 占用率较高, 编译完成后恢复正常, 具体进度可在Nessus Web 后台中查看。`**</font>
5. **Invicti Netsparker: v25.5.0(注册版)**
6. **[MasScan](https://github.com/robertdavidgraham/masscan/): 端口扫描工具(Kali) v1.3.2**
7. **[Nmap](https://nmap.org/): v7.97**
8. **[ObserverWard](https://github.com/emo-crab/observer_ward): 服务指纹识别工具 v2025.5.15**
9. **RouterScan: C 段扫描工具 v2.60**
10. **ScanBox:**
  - <font color=green>**`文件夹下集成下列工具`**</font>
  - **`AVScan: 杀毒软件检测工具`**
    - **`CheckAV`**
  - **`CDNScan: CDN 扫描工具`**
    - **[`CDNCheck`](https://github.com/projectdiscovery/cdncheck): v1.1.20**
    - **[`CF-Hero`](https://github.com/musana/CF-Hero): v1.0.4**
  - **`LeakScan: 敏感文件扫描工具`**	
    - **[`BBScan`](https://github.com/lijiejie/BBScan): v3.0**
    - **[`dirMap`](https://github.com/H4ckForJob/dirmap): v1.1**
    - **[`dirPro`](https://github.com/coleak2021/dirpro): v1.0**
    - **[`dirSearch`](https://github.com/maurosoria/dirsearch): v0.4.3**
    - **[`DudeSuite`](https://github.com/x364e3ab6/DudeSuite): v1.2.0.3**
    - **[`DumpAll`](https://github.com/0xHJK/dumpall): v0.4.0**
	- **[`ForBy`](https://github.com/Scorcsoft/forBy): .DS_Store 文件泄露利用工具 v1.0.1**
    - **[`Fuzz Faster U Fool`](https://github.com/ffuf/ffuf) v2.1.0**
    - **[`GitHack`](https://github.com/lijiejie/GitHack): v1.0**
    - **[`GitHacker`](https://github.com/WangYihang/GitHacker): v1.1.3**
    - **[`Gobuster`](https://github.com/OJ/gobuster): v3.6.0**
    - **[`Golin`](https://github.com/selinuxG/Golin): v1.2.6**
    - **[`Httpx`](https://github.com/projectdiscovery/httpx) v1.7.0**
    - **`JoomScan: Kali`**
    - **[`密探`](https://github.com/kkbo8005/mitan): v1.2.3**
    - **[`SnowShadow`](https://github.com/jinsezlb/SnowShadow): v1.0**
	- **[`Spray`](https://github.com/chainreactors/spray): v1.2.1**
    - **[`svnExploit`](https://github.com/admintony/svnExploit): v1.0**
    - **[`TscanPlus 无影`](https://github.com/TideSec/TscanPlus): v2.8.2**
    - **[`URLFinder`](https://github.com/pingc0y/URLFinder): v2023.9.9**
    - **`WPScan`: Kali**
    - **[`XSStrike`](https://github.com/s0md3v/XSStrike) v3.1.6**
    - **`御剑`**
  - **`SubDomain 子域名探测工具`**
    - **[`Amass`](https://github.com/owasp-amass/amass) v4.2.0**
    - **[`百川`](https://github.com/fankun99/baicuan): v1.1**
    - **[`Censys`](https://search.censys.io/) v2.0**
    - **[`FlashSearch`](https://github.com/testzboy/FlashSearch)**
    - **[`FofaView`](https://github.com/wgpsec/fofa_viewer): v1.1.15**
    - **[`GreyNoise`](https://viz.greynoise.io/)**
    - **[`Hunter`](https://hunter.how/)**
    - **[`InfoSearchAll`](https://github.com/ExpLangcn/InfoSearchAll): v1.2**
    - **`Layer: 子域名挖掘机`**
    - **[`ODIN`](https://search.odin.io/)**
    - **[`OneforAll`](https://github.com/shmilylty/OneForAll): v0.4.5**
    - **[`Subfinder`](https://github.com/projectdiscovery/subfinder): v2.7.1**
    - **[`Sublist3r`](https://github.com/aboul3la/Sublist3r): v1.1**

### <font color=orange>**[+] 权限工具 (C:\Penetration\ShellTools):**</font>

1. **[Antsword](https://github.com/AntSwordProject/AntSword-Loader): 蚁剑(已集成插件) v4.0.3**
2. **[Behinder](https://github.com/rebeyond/Behinder): 冰蝎**
  - **`behinder 3.0 beta11`**
  - **`behinder 4.1`**
3. **[ByPassBehinder](https://github.com/Tas9er/ByPassBehinder): 冰蝎免杀 v1.0**
4. **[ByPassGodzilla](https://github.com/Tas9er/ByPassGodzilla): 哥斯拉免杀 v1.0**
5. **Cobaltstrike:**
  - **[`猫猫二开`](https://github.com/TryGOTry/CobaltStrike_Cat_4.5): v4.5**
  - **[`坤坤二开`](https://github.com/D13Xian/CobaltStrike-KunKun): v4.5**
  - <font color=green>**`集成插件 (C:\Penetration\ShellTools\CobaltStrike\Scripts)`**</font>
    - **[`ADCollection`](https://github.com/lengjibo/RedTeamTools)**
    - **[`AntiVirusCheck`](https://github.com/raspberryhusky/antiVirusCheck)**
    - **[`BypassUserAdd`](https://github.com/crisprss/BypassUserAdd)**
    - **[`CrossC2 Kit`](https://github.com/CrossC2/CrossC2Kit)**
    - **[`CS-AutoPostChain`](https://github.com/lintstar/CS-AutoPostChain)**
    - **[`EasyPersistent`](https://github.com/yanghaoi/CobaltStrike_CNA)**
    - **[`Erebus`](https://github.com/DeEpinGh0st/Erebus): v1.3.6**
    - **[`EventLogMaster`](https://github.com/QAX-A-Team/EventLogMaster)**
    - **[`LSTAR`](https://github.com/lintstar/LSTAR): v2022.01.15**
    - **[`mikasa`](https://github.com/Mikasazero)**
    - **`mr.xie: 谢公子插件`**
    - **[`OLa`](https://github.com/Sec-Fork/OLa)**
    - **[`Pillager`](https://github.com/qwqdanchun/Pillager): v2024.09.07**
    - **[`taowu`](https://github.com/pandasec888/taowu-cobalt-strike)**
6. **[GBBypass](https://github.com/czz1233/GBByPass): 冰蝎 & 哥斯拉 Webshell 免杀 v1.2**
7. **Godzilla: 哥斯拉 v4.0.1**
  - **[`原版`]((https://github.com/BeichenDream/Godzilla)): **
  - **[`ekp 二开版`](https://github.com/ekkoo-z/Z-Godzilla_ekp): **
8. **WSL Kali Linux 2025.1**
  - <font color=green>**`username: kali password: kali`**</font>
  - <font color=green>**`username: root password: root`**</font>
  - <font color=green>**`修改软件源为阿里云`**</font>
  - <font color=green>**`如需使用桌面环境, 请运行“开启 kex 服务”快捷方式, 输入 kali 密码后稍等 (不要关闭终端) 即可进入桌面环境, 进入桌面后按 F8 去除 Full screen 可使用窗口模式。`**</font>
  - <font color=green>**`桌面环境非常占用系统资源, 建议非必要不开启, 使用完成后建议将 WSL Kali 关机释放内存。`**</font>
  - <font color=green>**`kex 管理密码为 password, 日常使用时不会要求输入。`**</font>
9. **Metasploit-Framework: (Kali)**
10. **Msfvenom: MSF 木马生成工具(Kali)**
11. **[Skyscorpion](https://github.com/shack2/skyscorpion): 天蝎 v1.0**
12. **WebShell: 一句话木马(密码统一为 cmd)**
  - **[`Webshell 收集项目`](https://github.com/tennc/webshell)**
13. **[WebshellBypassedHuman](https://github.com/Macr0phag3/webshell-bypassed-human): Webshell 免杀**
14. **[WebshellGenerate](https://github.com/cseroad/Webshell_Generate): Webshell 生成工具 v1.2.4**
15. **[XG拟态](https://github.com/xiaogang000/XG_NTAI): Webshell 免杀工具 v2.5**

### <font color=orange>**[+] 社工工具 (C:\Penetration\SocialEngineeringTools):**</font>

1. **[Mip22](https://github.com/makdosx/mip22): 钓鱼工具**
2. **[SocialEngineeringToolkit](https://github.com/trustedsec/social-engineer-toolkit): 社工工具包(Kali)**
3. **[Swaks](https://github.com/jetmore/swaks): 邮件伪造工具**

### <font color=orange>**[+] 系统工具 (C:\Penetration\SystemTools):**</font>

1. **7-Zip: v24.09(单文件版)**
2. **[Bandizip](https://ghxi.com/bandizip.html): 压缩工具(注册版) v7.37**
3. **[Clink](https://chrisant996.github.io/clink/) 命令行增强工具 v1.7.19**
4. **[Dism++](https://github.com/Chuyu-Team/Dism-Multi-language): 系统调节工具 v10.1.1002.1B**
5. **[Docker Desktop](https://www.docker.com/products/docker-desktop/): v4.41.2(汉化版)**
  - <font color=green>**`修改源为清华大学 & 网易 163`**</font>
6. **[Everything](https://ghxi.com/everything.html): 搜索工具 v1.4.1**
7. **[FastCopy](https://www.ghxi.com/fastcopy.html): 复制工具 v5.9.0**
8. **[Git](https://git-scm.com/): v2.49.0**
9. **[HEU KMS Activator](https://www.ghxi.com/heukmsactivator.html): 激活工具 v62.0**
10. **IOBit:**
  - **[`AdvancedSystemcare`](https://ghxi.com/advancedsystemcareultimate.html): 优化清理工具(注册版) v18.0.3.240**
  - **[`DriverBooster`](https://ghxi.com/iobitdriverbooster.html): 驱动工具(注册版) v12.4.0.585**
  - **[`Uninstaller`](https://ghxi.com/iobituninstaller.html): 卸载工具(注册版) v14.3.1.8**
  - **[`SmartDefrag`](https://ghxi.com/iobitsmartdefrag.html): 磁盘整理工具(注册版) v10.4.0.441**
11. **[Maye Lite](https://www.ghxi.com/mayelite.html): 快捷启动工具 v12.8.0.250416**
12. **[MenuManager](https://ghxi.com/contextmenumanager.html): 右键菜单管理工具 v3.3.3.1**
13. **[NTLite](https://www.ntlite.com/): 系统调节工具 v2025.5**
14. **[OncePower](https://www.ghxi.com/oncepower.html): 批量重命名工具 v2.24.1**
15. **[Oh My Posh](https://ohmyposh.dev/): 终端美化工具 v26.0.2**
16. **[OpenSSH](https://www.openssh.com/) SSH 协议工具 v10.0**
17. **[PCMaster](https://ghxi.com/pcmaster.html): 系统调整工具**
  - <font color=green>**`已创建右键快捷菜单:`**</font>
  - **`在此处打开 Terminal 终端`**
  - **`在此处打开 Kali Linux 终端`**
  - **`在此处打开 Notepad`**
  - **`控制面板`**
  - **`计算器`**
  - **`注册表`**
18. **UltraISO: iso 编辑工具 v9.7.6**
19. **wget & wget2**

### <font color=orange>**[+] 主题工具 (C:\Penetration\ThemeTools):**</font>

1. **ICON: 第三方图标**
2. **Refresh: 存刷图标缓新工具**

### <font color=orange>**[+] 流量工具 (C:\Penetration\TrafficTools):**</font>

1. **BlueTeamTools: 流量解密工具 v2.1.6**
2. **BurpSuite: v2025.2(注册版)**
  - <font color=green>**`集成插件`:**</font>
  - **[`汉化`](https://github.com/funkyoummp/burpsuitecn)**
  - **[`BurpFastJsonScan`](https://github.com/pmiaowu/BurpFastJsonScan)**
  - **[`BurpShiroPassiveScan`](https://github.com/pmiaowu/BurpShiroPassiveScan)**
  - **[`403Bypasser`](https://github.com/sting8k/BurpSuite_403Bypasser)**
  - **[`burp-vulners-scanner`](https://github.com/vulnersCom/burp-vulners-scanner)**
  - **[`ChangeuUnicode`](https://github.com/coffeehb/tools/tree/5c7fef3ff99ac4f80dcb52c73f70181848053315/burpUnicode)**
  - **[`ChunkedCodingConverter`](https://github.com/c0ny1/chunked-coding-converter)**
  - **[`DomainHunterPro`](https://github.com/bit4woo/domain_hunter_pro)**
  - **[`FakeIP`](https://github.com/TheKingOfDuck/burpFakeIP)**
  - **[`FransLinkfinder`]()**
  - **[`Hackbar`](https://github.com/d3vilbug/HackBar)**
  - **[`Log4j2Scan`](https://github.com/whwlsfb/Log4j2Scan)**
  - **[`Sqlmap4burp`](https://github.com/c0ny1/sqlmap4burp-plus-plus)**
  - **[`TsojanScan`](https://github.com/Tsojan/TsojanScan)**
  - **[`TurboIntruder`](https://github.com/PortSwigger/turbo-intruder)**
3. **[Fiddler Debugger](https://ghxi.com/fiddler.html): 流量抓包工具(汉化版) v5.0**
4. **[Fiddler Everywhere](https://github.com/msojocs/fiddler-everywhere-enhance): 流量抓包工具(注册版) v6.5.0**
5. **Firefox: 集成插件版 v49.0 **
6. **[Frp](https://github.com/fatedier/frp): 内网穿透工具 v0.62.1**
7. **[GoProxy](https://github.com/snail007/goproxy) v15.0**
8. **[GO Simple Tunnel](https://github.com/ginuerzh/gost): 隧道工具 v2.12.0**
9. **[Laragon](https://laragon.org/download/): 集成环境 v8.1.0**
10. **[LiqunShield](https://github.com/Liqunkit/LiqunShield): Webshell 流量分析工具**
11. **Netcat
  - **[`Netcat`](https://eternallybored.org/misc/netcat/): 原版 v1.11**
  - **[`Ncat`](https://nmap.org/ncat/): Nmap 重构版 v5.59**
  - **[`Rustcat`](https://github.com/robiot/rustcat): Rust 重构版 v3.0.0**
12. **[Neo-reGeorg](https://github.com/L-codes/Neo-reGeorg): Http 隧道工具 v5.2.1**
13. **[NetSetMan](https://ghxi.com/netsetman.html): 网络参数设置工具 v5.4.0**
14. **[NETworkManager](https://github.com/BornToBeRoot/NETworkManager/): 网络管理工具 v2025.1.18.0**
15. **[NPS](https://github.com/ehang-io/nps): 内网代理工具 v0.26.10**
16. **[OpenVPN](https://openvpn.net/): VPN 工具 v3.7.2**
17. **[phpStudy](https://www.xp.cn/): 集成环境 v8.1.1.3**
18. **[Proxifier](https://www.proxifier.com/): 流量代理工具(注册版) v4.1.4**
19. **[ProxyPin](https://github.com/wanghongenpin/proxypin): 流量抓包工具 v1.1.9**
20. **[ShadowSocks](https://github.com/shadowsocks/shadowsocks-windows): 科学上网工具 v4.4.1.0**
21. **[Stowaway](https://github.com/ph4ntonn/Stowaway): 内网穿透工具 v2.2**
22. **[Suo5](https://github.com/zema1/suo5): Http 隧道工具 v1.3.1**
23. **[TorBowser](https://www.torproject.org/): 洋葱浏览器 v14.5.2**
24. **[v2rayN](https://github.com/2dust/v2rayN): 科学上网工具 v7.12.3**
25. **[WireShark](https://www.wireshark.org/): 流量抓包分析工具 v4.4.6**
26. **[Yakit](https://github.com/yaklang/yakit): v1.4.1**

## <font color=blue>**全套虚拟机镜像:**</font>

1. **`Windows 7 x64`**
2. **`Windows 8 x64`**
3. **`Windows 10 x64`**
4. **`Windows Server 2008 x64`**
5. **`Windows Server 2012 x64`**
6. **`Windows Server 2016 x64`**
7. **`Windows Server 2019 x64`**
8. **`Ubuntu 20 x64`**
  - **所有虚拟机镜像均安装: **
    - **`VMTools`**
    - **`7z`**
    - **`Microsoft Visual C++ 2008-2022 运行库`**
    - **`密钥或激活工具激活`**

  - **`可供测试软件, 环境搭建等用途。`**
  - <font color=green>**`虚拟机账号密码已备注在 VMware 描述栏处, 请注意查看。`**</font>

## <font color=blue>**下载链接:**</font>
> **小水管上传中...**

## <font color=blue>**参考截图:**</font>
