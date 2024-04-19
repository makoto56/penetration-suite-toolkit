# <font color=red>**Windows10 Penetration Suite Toolkit within Kali Linux v5.0**</font>
![image](https://img.shields.io/badge/Author-Makoto56-blueviolet.svg) ![image](https://img.shields.io/badge/Platform-Windows-red.svg) ![image](https://img.shields.io/badge/WSL-Kali-9cf.svg) ![image](https://img.shields.io/badge/Property-%E6%AD%A6%E5%99%A8%E5%BA%93-brightgreen.svg)

# <font color=blue>**2024.4.17 更新说明:**</font>

1. **安卓、CTF、逆向、AI、取证、数据库等分类补充了部分实用工具；**
2. **去除部分长期未更新、使用效果不佳及功能重复的工具；**
3. **优化扫描器、数据库等部分工具系统资源占用过大问题；**
4. **重构工具快捷方式，注明详细使用参数及方法，图标美化；**
5. **系统、组件及工具常规升级更新。**

# <font color=blue>**系统简介:**</font>

1. **基于 Windows10 Workstation 22H2 x64 原版镜像制作<font color=red>(不适用于ARM设备)</font>；**
2. **完整安装 WSL2 Kali Linux 2024.1；**
 - <font color=Red>**注: 物理主机必须支持 CPU 虚拟化功能，否则 WSL2 无法使用！**</font>
 - <font color=green>**开启 VMware - 虚拟机设置 - 处理器 - 虚拟化引擎:**</font>
 - <font color=green>**虚拟化 Intel VT-x/EPT 或 AMD-V/RVI**</font>
 - <font color=green>**虚拟化 CPU 性能计数器**</font>
 - <font color=green>**虚拟化 IOMMU(IO 内存管理单元)**</font>
3. **精简系统自带软件，美化字体及部分图标，适度优化；**
 - **推荐运行环境:**
 - **VMware: 16.x(建议视情分配图形内存)**
 - **运行内存: 8G**
 - **固态硬盘: 300G**
# <font color=blue>**制作声明:**</font>

1. **所有的安装类软件均下载自对应的官方网站；**
2. **所有的绿色类软件均下载自[果核剥壳](https://www.ghxi.com) ；**
3. **所有的脚本类工具均下载自Github；**
4. **部分授权类工具(破解版)及优秀的渗透工具来自微信公号分享；**
 - **排名不分先后，同时也推荐大家关注，一起变得更强。**
> **雾晓安全、果核剥壳、归零安全、潇湘信安、学蚁致用、谢公子学安全、利刃信安、棉花糖网络安全圈、狐狸说安全、HACK技术沉淀营、无尾熊安全、T00ls、渗透攻击红队、洛米唯熊、雷石安全实验室、酒仙桥六号部队、InBug实验室、鸿鹄实验室、黑白之道、HACK之道、GobySec、Gcow安全团队、Gamma实验室、CobaltStrike实战、网络安全与黑客技术、QZ的安全悟道、菜鸟学信安、乌雲安全、白帽子飙车路、信安之路、chaosec、鸟哥谈安全、安全小飞侠、moonsec、系统安全运维、天驿安全、零组攻防实验室、Lemonsec、橘猫学安全、Hacking黑白红、渗透安全团队、渗透xiao白帽、白帽子社区、HACK学习呀、猪猪谈安全、开普勒安全团队、吾爱破解论坛、WhITECat安全团队、寻云安全团队、Khan安全攻防实验室、Bypass、天億网络安全、关注安全技术、玄魂工作室、边界骇客、零度安全攻防实验室、WgpSec狼组安全团队、黑白天实验室、靶机狂魔、渗透云笔记、TeamsSix、hijackY、重生信息安全、TimeLine Sec、GobySec、Gcow安全团队、冰蚕实验室。**
5. **本集成环境是根据本人渗透工作和学习中的侧重点进行制作，不可能做到满足所有人的需求；**
6. **本项目制作的初衷是帮助渗透新手快速搭建工作环境，工欲善其事，必先利其器；**
7. **本项目由于后期调试原因可能会遗留部分本人的信息，请直接忽视；**
8. **本项目坚决不接受也从未曾接受任何形式的赞助；**
9. **如果您有好的意见或者建议，请联系邮箱 burpsuite@qq.com。**

# <font color=blue>**免责声明:**</font>

1. **本镜像仅面向合法授权的企业安全建设行为，如您需要测试本镜像的可用性，请自行搭建靶机环境；**
2. **在使用本镜像进行检测时，您应确保该行为符合当地的法律法规，并且已经取得了足够的授权；**
3. **如您在使用本镜像的过程中存在任何非法行为，您需自行承担相应后果，作者将不承担任何法律及连带责任；**
4. **本镜像所使用的工具资源均来自于网友投稿及互联网整理，作者仅提供分享交流平台，不为其版权负责。如果您发现本镜像中有侵犯您(或贵司)知识产权的资源，请及时反馈，作者会第一时间进行修改或删除。**

# <font color=blue>**软件及工具介绍:**</font>

## **Windows App:**
1. **WSL2 Kali Linux 2024.1**
2. **Windows Terminal**
2. **TranslucentTB**

## **渗透测试:**

 **常用的Python、C#、Java等工具均配有 start.bat 或 start.vbs 快捷启动方式**

### <font color=orange>**[+] 人工智能 (C:\Penetration\AiTools) :**</font>

1. **[阿水Ai](https://ai.ashuiai.com/home): Ai资源聚合**
2. **[ChatGPT](https://chat.openai.com/)**
3. **[HackerGPT](https://chat.hackerai.co/zh)**

### <font color=orange>**[+] 安卓工具 (C:\Penetration\AndroidTools):**</font>

1. **[AdbDriver](https://adb.clockworkmod.com): ADB 驱动**
2. **AndroidHelper: APK 逆向工具**
3. **AndroidKiller: APK 综合工具**
4. **[Apk2url](https://github.com/n0mi1k/apk2url): APK 信息提取工具**
5. **[APKDeepLens](https://github.com/d78ui98/APKDeepLens): APK 扫描工具**
6. **[Apkinfo](https://github.com/bihe0832/Android-GetAPKInfo): APK 分析工具**
7. **[Apkleaks](https://github.com/dwisiswant0/apkleaks): APK 扫描工具**
8. **ApkScan-PKID: APK 查壳工具**
9. **[Apktool](https://github.com/iBotPeaches/Apktool): APK 反编译工具**
10. **[ApkToolPlus](https://github.com/linchaolong/ApkToolPlus): APK 反编译分析工具**
11. **[AppMessenger](https://github.com/sulab999/AppMessenger): APK 分析工具**
12. **[BlueStacks](https://www.bluestacks.com): 蓝叠安卓模拟器(安卓9.0)**
 - **已安装:**
 - **Debug Proxy**
 - **Dev Tools**
 - **Http Canary**
 - **JuiceSSH**
 - **MT Manager**
 - **Net Capture**
 - **Packet Capture**
 - **Terminal Emulator**
13. **[BytecodeViewer](https://github.com/Konloch/bytecode-viewer): 字节码查看工具**
14. **[Dextools](https://github.com/pxb1988/dex2jar): Dex 打包工具**
15. **[Jadx](https://github.com/skylot/jadx): 反编译工具**
16. **[JavaDecompiler](https://github.com/java-decompiler/jd-gui): 字节码查看工具**
17. **SuperJadx: 反编译工具**
18. **[Yaazhini](https://www.vegabird.com/yaazhini/): APK 漏洞扫描工具**

### <font color=orange>**[+] 免杀工具 (C:\Penetration\AntivirusTools):**</font>

1. **[AVevasion](https://github.com/1y0n/av_evasion_tool)**
2. **[AvEvasionCraftOnline](https://github.com/yutianqaq/AVEvasionCraftOnline)**
3. **[Aycvxz](https://gitee.com/lsgsd/aycvxz-pubilc)**
4. **[Charlotte](https://github.com/9emin1/charlotte)**
5. **[Invoke-Obfuscation](https://github.com/danielbohannon/Invoke-Obfuscation)**
6. **[LoaderFly](https://github.com/wangfly-me/LoaderFly)**
7. **[Powershell-Obfuscation](https://github.com/H4de5-7/powershell-obfuscation)**
8. **[Sandboxie](https://sandboxie-plus.com/): 沙盒工具**
9. **[VMProtect](http://www.dayanzai.me/vmprotect.html): 3.8.4(注册版)**
10. **[VProtect](https://ghxi.com/vprotect.html): 加壳工具**

### <font color=orange>**[+] 审计工具 (C:\Penetration\AuditTools):**</font>

1. **Fortify: 23.2(注册版)**
2. **Seay: PHP 代码审计工具**
3. **SeayDzend: PHP 代码审计工具**

### <font color=orange>**[+] 连接工具 (C:\Penetration\ConnectTools):**</font>

1. **[1Remote](https://github.com/1Remote/1Remote)**
2. **[Anydesk](https://www.ghxi.com/anydesk.html)**
3. **[Filezilla](https://www.ghxi.com/filezilla.html)**
4. **[Finalshell](https://www.hostbuf.com/)**
5. **[PuTTY](https://www.putty.org/)**
6. **[Sunlogin](https://sunlogin.oray.com/): 向日葵**
7. **[Teamviewer](https://www.teamviewer.com/)**
8. **[ToDesk](https://www.todesk.com/)**
9. **[WinSCP](https://www.ghxi.com/winscp.html)**
10. **[Xftp](https://www.netsarang.com/en/free-for-home-school/)(教育版)**
11. **[Xshell](https://www.netsarang.com/en/free-for-home-school/)(教育版)**

### <font color=orange>**[+] 破解工具 (C:\Penetration\CrackTools):**</font>

1. **AccessCrack: MDB 密码破解工具**
2. **Advanced Archive Password Recovery: 压缩包密码破解工具**
3. **Advanced Office Password Recovery: Office 密码破解工具**
4. **Advanced PDF Password Recovery: PDF 密码破解工具**
5. **DecryptPassword**
 - **文件夹下集成下列密码破解工具:**
 - **[finalshell-decoder](https://github.com/passer-W/FinalShell-Decoder)**
 - **[finalshellPasswordDecoder](https://github.com/qurikuduo/finalshellPasswordDecoder)**
 - **[firefox_decrypt](https://github.com/unode/firefox_decrypt)**
 - **[FireFox-Thief](https://github.com/LimerBoy/FireFox-Thief)**
 - **[hack-browser-data-windows](https://github.com/moonD4rk/HackBrowserData)**
 - **[how-does-navicat-encrypt-password](https://github.com/HyperSine/how-does-navicat-encrypt-password)**
 - **[how-does-SecureCRT-encrypt-password](https://github.com/HyperSine/how-does-SecureCRT-encrypt-password)**
 - **[how-does-Xmanager-encrypt-password](https://github.com/HyperSine/how-does-Xmanager-encrypt-password)**
 - **[Safe360Browsergetpass](https://github.com/hayasec/360SafeBrowsergetpass)**
 - **[SharpDecryptPwd](https://github.com/uknowsec/SharpDecryptPwd)**
 - **[teamviewer-dumper](https://github.com/attackercan/teamviewer-dumper)**
 - **[vcenterExsi_PwdDecrypt](https://github.com/jas502n/VcenterExsi_PwdDecrypt)**
 - **[winscppasswd](https://github.com/anoopengineer/winscppasswd)**
6. **[DecryptTools](https://github.com/wafinfo/DecryptTools): 加解密综合利用工具**
7. **[Hashcat](https://hashcat.net/hashcat/): 密码破解工具**
8. **[Hydra](https://github.com/vanhauser-thc/thc-hydra): 口令爆破工具**
9. **[John](https://www.openwall.com/john/): 密码破解工具**
10. **[Johnny](https://openwall.info/wiki/john/johnny): John 图形化版本**
11. **MD5Crack: MD5碰撞工具**
12. **[SNETCracker](https://github.com/shack2/SNETCracker): 超级弱口令检测工具**
13. **WebshellCrack: 一句话木马密码破解工具**

### <font color=orange>**[+] 夺旗工具 (C:\Penetration\CTFTools):**</font>

1. **ASCII: ASCII码转换工具**
2. **Audacity: 音频工具**
3. **BehinderDecode: 冰蝎流量解码工具**
4. **[BerylEnigma](https://github.com/ffffffff0x/BerylEnigma): 密码学工具**
5. **[Binwalk](https://github.com/ReFirmLabs/binwalk): 文件分析工具**
6. **[BlindWatermark](https://github.com/linyacool/blind-watermark): 盲水印工具**
7. **[CaptfEncoder](https://github.com/guyoung/CaptfEncoder): 密码学工具**
8. **[Ciphey](https://github.com/Ciphey/Ciphey): 全自动解密工具**
9. **Converter: 编码转换工具**
10. **CRCCalculator: CRC 计算工具**
11. **[CTFCrack](https://github.com/0Chencc/CTFCrackTools): CTF 工具框架**
12. **[CTFCrackTools](https://github.com/0Chencc/CTFCrackTools): CTF 工具框架**
13. **CTFEditor: 编码转换工具**
14. **[CTFTools](https://github.com/qianxiao996/CTF-Tools/): 密码学工具**
15. **[CyberChef](https://github.com/gchq/CyberChef): 编码转换工具**
16. **DesTool: DES 加解密工具**
17. **[F5-Steganography](https://github.com/matthewgao/F5-steganography): 隐写工具**
18. **FindFlag: Flag 查找工具**
19. **[Foremost](https://github.com/korczis/foremost): 分离工具**
20. **GifTools: GIF 图片工具**
21. **[GNUplot](http://www.gnuplot.info/): 数学绘图工具**
22. **JPHS: 图片隐写工具**
23. **[LSB-Steganography](https://github.com/RobinDavid/LSB-Steganography): 图片隐写工具**
24. **MossTool: 摩斯密码转换工具**
25. **[MP3Steno](https://github.com/MIUIEI/MP3Steno): 音频隐写工具**
26. **[Outguess](https://github.com/crorvick/outguess): 隐写工具**
27. **PcapTool: 流量分析工具**
28. **[PixelJihad](https://github.com/oakes/PixelJihad): 图片隐写工具**
29. **PixRecovery: 图片修复工具**
30. **PNGCalculator: PNG 图片计算工具**
31. **PNGCheck: PNG 图片计算工具**
32. **PNGDebugger: PNG 图片计算工具**
33. **PYGTools: 飘云阁密码学工具**
34. **QRCode: 二维码批量扫描工具**
35. **QRResearch: 二维码解析工具**
36. **Regular: 正则工具**
37. **RSATool: RSA 计算工具**
38. **SM4: SM4 加解密工具**
39. **[Stegdetect](https://github.com/abeluck/stegdetect): 隐写工具**
40. **[Steghide](https://github.com/StefanoDeVuono/steghide): 隐写工具**
41. **[Stegsolve](https://github.com/Giotino/stegsolve): 隐写工具**
42. **TaowaTool: CTF 工具框架**
43. **[ToolsFx](https://github.com/Leon406/ToolsFx): 密码学工具**
44. **[TweakPNG](https://github.com/jsummers/tweakpng): PNG 调整工具**
45. **Ulead GIF Animator: GIF 图片工具**
46. **[wbStego](http://www.bailer.at/wbstego/pr_4ixopen.htm): 图片隐写工具**
47. **WinDecrypto: 密码学工具**
48. **[WinHex](https://www.x-ways.net/winhex/): 十六进制编辑工具**
49. **Xiaokui: 小葵编码工具**
50. **ZZYQR: 二维码解析工具**

### <font color=orange>**[+] 数据库工具 (C:\Penetration\DatabaseTools):**</font>

1. **Access Database Browser: MDB数据库查看工具**
2. **[Another Redis Desktop Manager](https://github.com/qishibo/AnotherRedisDesktopManager): Redis 客户端**
3. **[DatabaseTools](https://github.com/Hel10-Web/Databasetools): 数据库综合利用工具**
4. **[HeidiSQL](https://www.ghxi.com/heidisql.html): 数据库管理工具**
5. **[MariaDB](https://mariadb.org/): Mysql 数据库**
 - <font color=green>**username: root**</font>
 - <font color=green>**password: sqladmin**</font>
 - <font color=green>**如需使用请先运行开启服务快捷方式**</font>
6. **[MultipleDatabaseUtilizationTools](https://github.com/SafeGroceryStore/MDUT): 数据库综合利用工具**
7. **[Navicat](https://github.com/LiJunYi2/navicat-keygen-16V): 数据库管理工具(注册版)**
8. **[Neo4j](https://neo4j.com/)**
 - <font color=green>**username: root**</font>
 - <font color=green>**password: sqladmin**</font>
9. **[Oracle 19c](https://www.oracle.com/cn/database/technologies/oracle19c-windows-downloads.html)**
 - <font color=green>**username: system**</font>
 - <font color=green>**password: sqladmin**</font>
 - <font color=green>**如需使用请先运行开启服务快捷方式**</font>
10. **[OracleShell](https://github.com/jas502n/oracleShell): Oracle 数据库利用工具**
11. **[OSSBrowser](https://github.com/aliyun/oss-browser): 数据库管理工具**
12. **PostgreUtil: Postgresql 数据库利用工具**
13. **Redis: Redis 客户端(Kali)**
14. **[SharpsqlTools](https://github.com/uknowsec/SharpSQLTools): sqlServer 利用工具**
15. **[sqLite](https://www.sqlite.org/): sqLite 客户端**
16. **[sqlKnife](https://github.com/0x727/SqlKnife_0x727): sqlServer 利用工具**
17. **[Sqlmap](https://github.com/sqlmapproject/sqlmap): 数据库利用工具**
18. **[SqlmapXPlus](https://github.com/co01cat/SqlmapXPlus): Sqlmap 二开版**
19. **[sqlServer 2019](https://www.microsoft.com/zh-cn/evalcenter/download-sql-server-2019): sqlServer 2019 专业版**
 - <font color=green>**username: sa**</font>
 - <font color=green>**password: sqladmin**</font>
 - <font color=green>**如需使用请先运行开启服务快捷方式**</font>
20. **[sqlServer Management Studio 18](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16#download-ssms): sqlServer 管理工具**
21. **[sqlTools](https://github.com/uknowsec/SharpSQLTools): sqlServer 利用工具**
22. **[ssqlinjection](https://github.com/shack2/SuperSQLInjectionV1): 超级注入工具**
23. **[Sylas](https://github.com/Ryze-T/Sylas): 数据库利用工具**
24. **[TinyRDM](https://github.com/tiny-craft/tiny-rdm/releases/tag/v1.1.10): Redis 客户端**
25. **[ToadOracle](https://www.quest.com/products/toad-for-oracle/): Oracle 客户端**

### <font color=orange>**[+] 字典工具 (C:\Penetration\DictionaryTools):**</font>

1. **DictMaker: 字典生成工具**
 - **[DictTools](https://github.com/abc123info/UserNameDictTools)**
 - **[PwdBUD](https://github.com/ort4u/PwdBUD)**
 - **[Social Engineering Dictionary Generator](https://github.com/zgjx6/SocialEngineeringDictionaryGenerator): 社工密码生成工具**
 - **黑刀字典生成工具**
 - **火花字典生成工具**
 - **木头字典生成工具**
 - **品轩字典生成工具**
 - **易优字典生成工具**
2. **[Pentestdicts](https://github.com/ppbibo/pentesterspecialdict)**

### <font color=orange>**[+] 磁盘工具 (C:\Penetration\DiskTools):**</font>

1. **[DiskDrill](https://www.cleverfiles.com/): 数据恢复工具(注册版)**
2. **DiskGenius(注册版)**
3. **[SSDFresh](https://www.abelssoft.de/en/windows/system-utilities/ssd-fresh): 磁盘整理工具**

### <font color=orange>**[+] 编辑工具 (C:\Penetration\EditTools):**</font>

1. **[010Editor](https://www.ghxi.com/010editor.html): 十六进制编辑工具(注册版)**
2. **[AnyTXT](https://www.ghxi.com/anytxtsearcher.html): 文本搜索工具**
3. **BeyondCompare: 文件对比工具**
4. **[eSearch](https://www.ghxi.com/esearch.html): 截屏、录屏、OCR、搜索、翻译、贴图、搜图(已集成离线OCR库)**
5. **[FFRename](https://www.ghxi.com/ffrename.html): 菲菲更名宝贝(注册版)**
6. **FindStr: 文本搜索工具**
7. **[JsonViewer](https://dadroit.com/download/): Json查看编辑工具**
8. **[myBase](https://www.ghxi.com/mybase.html): 个人数据库编辑工具(注册版)**
9. **[Notepad++](https://notepad-plus-plus.org/downloads/): 编辑工具**
10. **PSTConverter: Outlook PST 邮件转换工具**
11. **[SharpSword](https://github.com/OG-Sadpanda/SharpSword): Word 命令行查看工具**
12. **[Sublime](https://www.ghxi.com/sublimetext4.html): 编辑工具(注册版)**
13. **[Typora](https://www.ghxi.com/typora.html): MarkDown 编辑工具(注册版)**
14. **[UltraEdit](https://www.ghxi.com/ultraedit.html): 编辑工具**
15. **[VisualStudio Code](https://code.visualstudio.com/download)**
16. **XMind: 思维导图工具**

### <font color=orange>**[+] 漏洞工具 (C:\Penetration\ExploitTools):**</font>

1. **Airflow**
2. **Apache**
3. **Apereo-CAS**
4. **AppWeb**
5. **Aria2**
6. **Bash**
7. **Cacti**
8. **Cas**
9. **Celery**
10. **CGI**
11. **Chrome**
12. **Citrix**
13. **CMSHunter**
14. **ColdFusion**
15. **Confluence**
16. **D-Link**
17. **Database**
18. **DNS**
19. **Docker**
20. **Elasticsearch**
21. **Electron**
22. **elFinder**
23. **Exiftool**
24. **F5-BIG-IP**
25. **FastAdmin**
26. **Fastjson**
27. **FCKEditor**
28. **FFmpeg**
29. **FusionAuth**
30. **GhostScript**
31. **Git**
32. **Gitea**
33. **Gitlab**
34. **Gitlist**
35. **GlassFish**
36. **GoAhead**
37. **Gogs**
38. **Gopherus**
39. **Grafana**
40. **Hadoop**
41. **Harbor**
42. **Hikvision**
43. **HttpBasic**
44. **Httpd**
45. **HttpFileServer**
46. **IIS**
47. **ILO4**
48. **ImageMagick**
49. **InfluxDB**
50. **Intellian-Aptus-Web**
51. **JacksonDatabind**
52. **Java**
53. **Jboss**
54. **Jellyfin**
55. **Jenkins**
56. **Jetty**
57. **Jira**
58. **JumpServer**
59. **Jupyter**
60. **Kibana**
61. **Libssh**
62. **Liferay**
63. **LiferayPortal**
64. **Linux**
 - **CVE-2015-1328**
 - **CVE-2019-14287**
 - **CVE-2021-22555**
 - **CVE-2021-3156**
 - **CVE-2021-33909**
 - **CVE-2021-3493**
 - **CVE-2021-4034**
 - **CVE-2022-0847-1**
 - **CVE-2022-0847-2**
 - **CVE-2022-23222**
 - **CVE-2024-1086**
 - **...**
65. **Mail**
 - **Coremail**
 - **Exchange**
 - **Zimbra**
66. **Metabase**
67. **MetaCRM**
68. **MiniHttpd**
69. **MinIO**
70. **ModSecurity**
71. **Mojarra**
72. **Nacos**
73. **Nexus**
74. **Nginx**
75. **Node.js**
76. **Ntopng**
77. **OA**
 - **Seeyon**
 - **Tongda**
 - **Weaver**
78. **Office**
79. **Open-AudIT**
80. **OpenSmtpd**
81. **OpenSSH**
82. **OpenSSL**
83. **Others**
84. **PHP**
85. **PHPMailer**
86. **phpMyadmin**
87. **PHPStudy**
88. **Polkit**
89. **Python**
90. **Rails**
91. **Rconfig**
92. **RocketChat**
93. **Rsync**
94. **Ruby**
95. **Ruoyi**
96. **SaltStack**
97. **Sangfor**
98. **SAP**
99. **Shiro**
100. **ShowDoc**
101. **Solarwinds**
102. **Spring**
103. **Struts2**
104. **Sunlogin**
105. **Supervisord**
106. **TeamViewer**
107. **TikiWiki**
108. **Tomcat**
109. **Tools**
 - **[Aakian-FaCai](https://github.com/zangcc/Aakian-FaCai): VUE 漏洞扫描工具**
 - **[AliyunAKTools](https://github.com/mrknow001/aliyun-accesskey-Tools): 阿里云利用工具**
 - **AptTools: 综合漏洞利用工具**
 - **[Cloud Exploitation Framework](https://github.com/teamssix/cf): 云环境利用框架**
 - **[EquationToolsGUI](https://github.com/abc123info/EquationToolsGUI): 方程式工具包图形界面版**
 - **[ExpDemo](https://github.com/yhy0/ExpDemo-JavaFX): 综合漏洞利用工具**
 - **[Exp-Tools](https://github.com/cseroad/Exp-Tools): 综合漏洞利用工具**
 - **[Gr33k](https://github.com/lijiaxing1997/Gr33k): 综合漏洞利用工具**
 - **[HeapdumpTool](https://github.com/wyzxxz/heapdump_tool): HeapDump 敏感信息提取工具**
 - **[HVVExploitApply](https://github.com/ExpLangcn/HVVExploitApply): 综合漏洞利用工具**
 - **[Hyacinth](https://github.com/pureqh/Hyacinth): 综合漏洞利用工具**
 - **[IWannaGetAll](https://github.com/R4gd0ll/I-Wanna-Get-All): OA 漏洞利用工具**
 - **[JDumpSpider](https://github.com/whwlsfb/JDumpSpider): HeapDump 敏感信息提取工具**
 - **[JNDI-Exploit](https://github.com/welk1n/JNDI-Injection-Exploit): JNDI 注入测试工具**
 - **[JNDI-Injection-Exploit](https://github.com/welk1n/JNDI-Injection-Exploit): JNDI 注入测试工具**
 - **[LiqunKit](https://github.com/Liqunkit/LiqunKit_): 综合漏洞利用工具**
 - **[MYExploit](https://github.com/achuna33/MYExploit): 综合漏洞利用工具**
 - **[NSudoLG](https://github.com/Thdub/NSudo_Installer): Windows 提权工具**
 - **[Nuclei](https://github.com/projectdiscovery/nuclei): 漏洞扫描利用工具**
 - **TheLostWorld: OA 漏洞利用工具**
 - **[Poc2jar](https://github.com/f0ng/poc2jar): 综合漏洞利用工具**
 - **[R-Knife](https://github.com/qianxiao996/R-Knife): 综合漏洞利用工具**
 - **SearchSploit: (Kali)**
 - **[SuperXray](https://github.com/4ra1n/super-xray): Xray 图形化版本**
 - **[Unauthorized](https://github.com/xk11z/unauthorized): 未授权漏洞检测工具**
 - **[Windows Exploit Suggester - NG](https://github.com/bitsadmin/wesng): Windows 提权工具**
 - **[Windows Exploit Suggester](https://github.com/0xToast/Windows-Exploit-Suggester-Py-3): Windows 提权工具**
 - **Wiki: 零组文档库 & 漏洞文档库**
 - **[Xray](https://github.com/chaitin/xray): 漏洞扫描利用工具**
 - **[Ysoserial](https://github.com/frohoff/ysoserial): Java 反序列化利用工具**
110. **TPLink**
111. **uWSGI**
112. **V2board**
113. **VMware**
114. **Vue**
115. **Weblogic**
116. **Webmin**
117. **Windows**
 - **CVE-2003-0352**
 - **CVE-2005-1983**
 - **CVE-2006-3439**
 - **CVE-2008-1084**
 - **...**
 - **CVE-2021-42287**
 - **CVE-2022-21907**
 - **CVE-2022-26923**
 - **...**
 - **MS03-026**
 - **MS05-039**
 - **MS06-040**
 - **...**
 - **MS17-017**
118. **XenMobile**
119. **XStream**
120. **XXL-job**
121. **YApi**
122. **Zabbix**
123. **Zoho**
124. **Zyxel**
> <font color=green>**漏洞库综合了下列项目:**</font>
 - **[CMS-Hunter](https://github.com/SecWiki/CMS-Hunter)**
 - **[expHub](https://github.com/zhzyker/exphub)**
 - **[Middleware-Vulnerability-Detection](https://github.com/mai-lang-chai/middleware-vulnerability-detection)**
 - **[System-Vulnerability](https://github.com/mai-lang-chai/system-vulnerability)**
 - **[Vulnerability](https://github.com/edgesecurityteam/vulnerability)**
> <font color=green>**更多漏洞 EXP & POC 请善用 Everything 搜索**</font>

### <font color=orange>**[+] 取证工具 (C:\Penetration\ForensicsTools):**</font>

1. **[AlternateStreamView](https://www.nirsoft.net/utils/alternate_data_streams.html): NTFS 数据流工具**
2. **[AutoSpy](https://www.autopsy.com/)**
3. **[FireKylin](https://github.com/MountCloud/FireKylin): 系统痕迹采集工具**
4. **Gather: 信息收集工具**
 - **Windows:**
 - **GetWinInfo** 
 - **Linux:**
 - **[Gather](https://github.com/wwl012345/gather)**
5. **[GoWxDump](https://github.com/SpenserCai/GoWxDump): 微信取证工具**
6. **[Hema](https://www.shellpub.com/): Webshell 查杀**
7. **[KunWu](https://github.com/kunwu2023/kunwu): Webshell 查杀**
8. **[LogParser](https://www.microsoft.com/en-us/download/details.aspx?id=24659): Windows 日志工具**
9. **[LogParserLizard](https://lizard-labs.com/log_parser_lizard.aspx): LogParser 图形化版本**
10. **[LogParserStudio](https://techcommunity.microsoft.com/t5/exchange-team-blog/introducing-log-parser-studio/ba-p/601131): LogParser 图形化版本**
11. **[Magnet AXIOM](https://breachforums.cx/Thread-Magnet-Axiom-7-8-crack): 取证工具**
12. **[MemProcFS](https://github.com/ufrisk/MemProcFS): 内存取证工具**
13. **[NTFSStreamsEditor](https://www.nirsoft.net/utils/alternate_data_streams.html): NTFS 数据流工具**
14. **[NTPWEdit](https://github.com/patrickgill/ntpwedit): SAM 文件编辑工具**
15. **[oletools](https://github.com/decalage2/oletools): OLE 文件分析工具**
16. **[qemu-img](https://www.qemu.org/download/): 镜像分析工具**
17. **[SharpWxDump](https://github.com/AdminTest0/SharpWxDump): 微信取证工具**
18. **[Volatility2](https://github.com/volatilityfoundation/volatility)**
19. **[Volatility3](https://github.com/volatilityfoundation/volatility3)**
20. **[WindowsBaselineAssistant](https://github.com/DeEpinGh0st/WindowsBaselineAssistant): Windows 安全基线加固助手**
21. **[WindowsLogsAnalysis](https://github.com/dogadmin/windodws-logs-analysis): 日志分析工具**
22. **[WinPmem](https://github.com/Velocidex/WinPmem): Windows 内存取证工具**

### <font color=orange>**[+] 内网工具 (C:\Penetration\IntranetTools):**</font>

1. **[3Gstudent](https://github.com/3gstudent): 三好学生脚本**
2. **AddUser:添加用户工具**
3. **[ADExplore](https://learn.microsoft.com/en-us/sysinternals/downloads/adexplorer): LDAP 工具**
4. **[ADinfo](https://github.com/lzzbb/Adinfo): 内网信息搜集工具**
5. **[Aoratos](https://github.com/PinoyWH1Z/AoratosWin): 软件运行痕迹清理工具**
6. **[BloodHound](https://github.com/BloodHoundAD/BloodHound): 域渗透分析工具**
7. **[BloudyAD](https://github.com/CravateRouge/bloodyAD): 域渗透利用工具**
8. **ClearLogs: Windows 日志清除工具**
9. **[ContextMenuHijack](https://github.com/RistBS/ContextMenuHijack): 右键菜单劫持工具**
10. **[CrackMapExec](https://github.com/Porchetta-Industries/CrackMapExec): 内网综合利用工具**
11. **[DomainInfoFind](https://github.com/wangfly-me/DomainInfo_Find): 获取域内机器的桌面文件**
12. **[DomainTools](https://github.com/SkewwG/domainTools): 域渗透综合利用工具**
13. **[EarthWorm](https://github.com/rootkiter/Binary-files):内网穿透工具**
14. **[Evil-WinRM](https://github.com/Hackplayers/evil-winrm): WinRM 利用工具**
15. **[Frp](https://github.com/fatedier/frp): 内网穿透工具**
16. **[FScan](https://github.com/shadow1ng/fscan): 内网扫描工具**
17. **[Gorailgun](https://github.com/lz520520/railgun): 内网渗透综合利用工具**
 - <font color=green>**password: 三个空格**</font>
18. **[GoToHTTP](https://gotohttp.com/): 远控工具**
19. **[Hoaxshell](https://github.com/t3l3machus/hoaxshell): 远控工具**
20. **[imPacket](https://github.com/SecureAuthCorp/impacket): 内网协议工具**
 - **[impacket-gui](https://github.com/Suq3rm4n/java-impacket-gui)**
 - **[impacket-windows](https://github.com/maaaaz/impacket-examples-windows)**
 - **[wmiexec-pro](https://github.com/XiaoliChan/wmiexec-Pro)**
21. **[Kerbrute](https://github.com/ropnop/kerbrute): 域枚举爆破工具**
22. **Ladon: 内网扫描工具(12.4版)**
23. **[LdapAdmin](http://www.ldapadmin.org/): LDAP 工具**
24. **[LDAPDomainDump](https://github.com/dirkjanm/ldapdomaindump): LDAP 工具**
25. **Mimikatz:密码抓取工具**
 - <font color=green>**文件夹下集成下列密码抓取工具**</font>
 - **[CallBackDump](https://github.com/seventeenman/CallBackDump)**
 - **[DumpHash](https://github.com/Avienma/DumpHash)**
 - **[GoSecretsDump](https://github.com/C-Sto/gosecretsdump)**
 - **HKLM**
 - **[KEKEO](https://github.com/gentilkiwi/kekeo)**
 - **[LaZagne](https://github.com/AlessandroZ/LaZagne)**
 - **[LsassSilentProcessExit](https://github.com/deepinstinct/LsassSilentProcessExit)**
 - **[LsassUnhooker](https://github.com/roberreigada/LsassUnhooker)**
 - **[Mimipenguin](https://github.com/huntergregal/mimipenguin)**
 - **[NTDSDumpEx](https://github.com/zcgonvh/NTDSDumpEx)**
 - **[Procdump](https://learn.microsoft.com/en-us/sysinternals/downloads/procdump)**
 - **[Pwdump](https://www.openwall.com/passwords/windows-pwdump)**
 - **[Quarkspwdump](https://blog.quarkslab.com/quarks-pwdump.html)**
26. **[Moonwalk](https://github.com/mufeedvh/moonwalk): Linux 痕迹恢复工具**
27. **[Nacs](https://github.com/u21h2/nacs): 内网扫描工具**
28. **[Neo-reGeorg](https://github.com/L-codes/Neo-reGeorg): reGeorg 重构版**
29. **[NetSpy](https://github.com/shmilylty/netspy): 内网网段探测工具**
30. **[NPS](https://github.com/ehang-io/nps): 内网代理工具**
31. **[OpenRDP](https://github.com/lengjibo/RedTeamTools): 开启远程桌面工具**
32. **[PE](https://www.wepe.com.cn/): WeiPE ISO 镜像**
33. **[PEASS-ng](https://github.com/carlospolop/PEASS-ng): Linux 取证工具**
34. **[PowerProxy](https://github.com/get-get-get-get/PowerProxy): Powershell 代理工具**
35. **[PowerShdll](https://github.com/p3nt4/PowerShdll): Powershell 执行工具**
36. **[PS2EXE](https://github.com/MScholtes/PS2EXE): Powershell 转 EXE 工具**
37. **[PSTools](https://learn.microsoft.com/en-us/sysinternals/downloads/pstools): 微软 psexec 工具**
38. **[PyStinger](https://github.com/FunnyWolf/pystinger): 流量代理工具**
39. **[RedPersist](https://github.com/mertdas/RedPersist): 权限持久化工具**
40. **[RevSH](https://github.com/emptymonkey/revsh): 内网穿透工具**
41. **[Scan4all](https://github.com/hktalent/scan4all): 内网扫描工具**
42. **[ScheduleRunner](https://github.com/netero1010/ScheduleRunner): 计划任务利用工具**
43. **[SeachAll](https://github.com/Naturehi666/searchall): 内网扫描工具**
44. **SharpTools:**
 - **[CatchBrowser](https://github.com/SD-XD/Catch-Browser): 浏览器密码抓取工具**
 - **[ListRDPConnections](https://github.com/Heart-Sky/ListRDPConnections): 远程桌面连接记录枚举工具**
 - **[SharpAdiDnsDump](https://github.com/b4rtik/SharpAdidnsdump): 域 DNS 枚举工具**
 - **[SharpEventLog](https://github.com/uknowsec/SharpEventLog): 日志分析工具**
 - **[SharpHide](https://github.com/outflanknl/SharpHide): 创建隐藏注册表运行键**
 - **[SharpHound](https://github.com/BloodHoundAD/SharpHound): 域渗透分析工具**
 - **[SharpNetCheck](https://github.com/uknowsec/SharpNetCheck): 出网探测工具**
 - **[SharpRDPLog](https://github.com/Adminisme/SharpRDPLog): 远程桌面连接记录枚举工具**
 - **[SharpStrike](https://github.com/iomoath/SharpStrike):CobaltStrike 工具**
 - **[SharpToken](https://github.com/BeichenDream/SharpToken): 令牌窃取工具**
45. **[StopDefender](https://github.com/lab52io/StopDefender): 关闭defender工具**
46. **[Stowaway](https://github.com/ph4ntonn/Stowaway): 内网穿透工具**
47. **[Suo5](https://github.com/zema1/suo5): HTTP 代理隧道工具**
48. **[Traitor](https://github.com/liamg/traitor): Linux 提权工具**
49. **[WindowsCredentialsEditor](https://github.com/returnvar/wce): Windows 凭证编辑工具**
50. **[WMIHacker](https://github.com/rootclay/WMIHACKER): WMI 渗透工具**
51. **[Yasso](https://github.com/sairson/Yasso): 内网漏扫利用工具**

### <font color=orange>**[+] 影音图像 (C:\Penetration\MediaTools):**</font>

1. **Acrobat DC: PDF 编辑工具**
2. **Adobe Photoshop 2022**
3. **[Bandicam](https://ghxi.com/bandicam.html): 屏幕录像工具(注册版)**
4. **[FormatFactory](https://ghxi.com/formatfactory-2.html): 格式工厂(注册版)**
5. **[Goldwave](https://www.goldwave.com/): 音频编辑工具**
6. **[Honeyview](https://www.bandisoft.com/honeyview/): 图片查看工具**
7. **[K-Lite](https://codecguide.com/download_kl.htm): 播放器**
8. **[Meitu](https://mt.meipai.com/): 美图秀秀**
9. **[PotPlayer](https://ghxi.com/potplayer.html): 播放器**
10. **[Snipaste](https://ghxi.com/snipaste.html): 截图工具**

### <font color=orange>**[+] 网络工具 (C:\Penetration\NetworkTools):**</font>

1. **[Chrome](https://ghxi.com/chrome.html): 122.0.6261.95 绿色修改版**
 - <font color=green>**主要集成插件:**</font>
 - **Adblock: 广告拦截工具**
 - **Charset: 修改网页编码工具**
 - **Chrome清理大师: chrome清理工具**
 - **DuckDuckGo Privacy Essentials: 隐私保护**
 - **Editthiscookie: cookie编辑工具**
 - **FindSomething: 敏感文件搜集工具**
 - **Hackbar**
 - **Hack-Tools: 红队综合小工具**
 - **IE Tab: ie兼容模式工具**
 - **Imagus: 图片预览工具**
 - **Infinity: 标签页工具**
 - **IP address and domain inf: ip & domain 探测工具**
 - **IP whois: whois 探测工具**
 - **Neater bookmarks: 书签管理工具**
 - **Octotree: github资源树查看工具**
 - **Onetab: 标签管理工具**
 - **OWASP Penetration Testing Kit: 浏览器渗透测试工具**
 - **Postwoman: 接口调试工具**
 - **Proxy switchyomega: 代理切换工具**
 - **Seoquake: 网页统计工具**
 - **Shodan**
 - **Supercopy: 超级复制**
 - **Tampermonkey: 脚本工具**
 - **User-Agent Switcher: 浏览头切换工具**
 - **Vulners Web Scanner: 漏洞扫描工具**
 - **Toolbox 常用工具: 集成常用小工具**
 - **Vulners Web Scanner: 微型漏洞扫描工具**
 - **Wappalyzer: 网页技术分析工具**
 - **WebSocket Test Client: websocket工具**
 - **Whatruns: 网页技术分析工具**
 - **XSS辅助工具**
 - **X情报查询助手:微步社区**
 - **YetAnotherDragAndGo: 超链接拖拽新窗口打开**
 - **ZoomEye Tools**
 - **图片另存为JPG/PNG/WebP**
 - **类似的网站**
 - **草料二维码**
2. **[FDM](https://www.freedownloadmanager.org/): 下载工具**
3. **[Telegram](https://telegram.org/)**

### <font color=orange>**[+] 办公工具 (C:\Penetration\OfficeTools):**</font>

1. **Office: Word + Excel + Powerpoint + Access + Onenote + Outlook**
2. **[WPS](https://ghxi.com/wps2019pro.html): 11.8.2.12195 专业增强版**

### <font color=orange>**[+] 编程工具 (C:\Penetration\ProgramTools):**</font>

1. **[Go](https://go.dev/)**
2. **Java:**
 - **jre1.8.0: 已配置环境变量，系统默认调用 Java8**
 - **jre15.0.2: 绿色版，如有软件需要java15环境运行可直接调用/bin/java.exe即可**
 - **jdk21: 绿色版，如有软件需要java21环境运行可直接调用/bin/java.exe即可**
3. **JetBrains: 2024.1(注册版)**
 - **CLion**
 - **DataGrip**
 - **GoLand**
 - **IntelliJ**
 - **PhpStorm**
 - **PyCharm**
 - **Rider**
 - **WebStorm**
 - <font color=green>**如遇到激活状态失效，请手动运行/JetBrains/破解补丁/目录下的破解脚本。**</font>
4. **[MinGW64](https://www.mingw-w64.org/)**
5. **[Nim](https://nim-lang.org/)**
4. **[Nodejs](https://nodejs.org/)**
5. **[Python](https://www.python.org/):**
 - **python2: python2命令启动(python2 test.py)**
 - **python3: python3命令启动(python3 test.py)**
 - **已集成本镜像所有工具的 pip 依赖库**<font color=green>**(如有遗漏未安装的库请自行安装)**</font>
 - **使用 pip 命令调用 python3 pip**
6. **[TDM-GCC](https://jmeubank.github.io/tdm-gcc/)**
7. **VisualStudio 2022: 社区版**

### <font color=orange>**[+] 逆向工具 (C:\Penetration\ReverseTools):**</font>

1. **[bat2exe](https://bat2exe.net/): BAT 转 EXE 工具**
2. **[DetectItEasy](https://ghxi.com/die.html): 查壳工具**
3. **[dnSpy](https://github.com/dnSpy/dnSpy): .Net 逆向工具**
4. **exeScope: EXE 编辑工具**
5. **[Ghidra](https://github.com/NationalSecurityAgency/ghidra): 逆向工具**
6. **[GhostExplore](https://symantec-ghost-explorer.software.informer.com/): GHO 文件编辑工具**
5. **[GreenHelper](https://ghxi.com/gscript.html): EXE 绿化工具**
6. **[HashTool](https://github.com/KiyanYang/HashTool): Hash 计算工具**
1. **[Html2exe](http://szhnnas.abitsoft.com:8081/): Html 打包工具**
7. **[IDAPro](https://ghxi.com/pcida.html)**
8. **[ILSpy](https://github.com/icsharpcode/ILSpy): .Net 逆向工具**
10. **[OllyDebug](https://ghxi.com/ollydug.html): 1.10 吾爱破解修复增强版**
11. **[PeiD](https://www.aldeid.com/wiki/PEiD): 查壳工具**
12. **SignTool: 签名伪造工具**
13. **[UPX](https://upx.github.io/): 加壳工具**
14. **[vbs2exe](https://github.com/eimon96/vbs2exe): VBS 转 EXE 工具**
15. **[x64Debug](https://ghxi.com/x64_dbg.html): EXE 调试工具**

### <font color=orange>**[+] 扫描工具 (C:\Penetration\ScanTools):**</font>

1. **Acunetix: 24.2.240226074(注册版)**
  - <font color=green>**username: admin@awvs.com**</font>
  - <font color=green>**password: Admin@awvs.com**</font>
  - <font color=green>**如需使用请先运行开启服务快捷方式**</font>
2. **AppScan: 10.4.0(注册版)**
3. **[EasySpider](https://www.easyspider.net/): 爬虫工具**
4. **Nessus: 10.7.1(注册版)**
 - <font color=green>**username: admin**</font>
 - <font color=green>**password: password**</font>
 - <font color=green>**如需使用请先运行开启服务快捷方式**</font>
 - <font color=green>**Nessusd 服务开启后会自动编译插件，CPU 占用率较高，编译完成后恢复正常，具体进度可在Nessus Web 后台中查看。**</font>
5. **Invicti Netsparker: 24.3(注册版)**
5. **[Nmap](https://nmap.org/)**
6. **RouterScan: C段扫描工具**
7. **ScanBox**
> **AVScan 杀毒软件检测工具:**
 - **CheckAntivirus(自己写的，如有需要可随便使用)**
> **CDNScan CDN 扫描工具:**
 - **[CDNCheck-go](https://github.com/projectdiscovery/cdncheck)**
 - **[CDNCheck-python](https://github.com/wwl012345/CDNCheck)**
> **LeakScan 敏感文件扫描工具:**	
 - **[BBScan](https://github.com/lijiejie/BBScan)**
 - **[Caesar](https://github.com/thunderbarca/Caesar)**
 - **[dirMap](https://github.com/H4ckForJob/dirmap)**
 - **[dirPro](https://github.com/coleak2021/dirpro)**
 - **[dirSearch](https://github.com/maurosoria/dirsearch)**
 - **[DudeSuite](https://github.com/x364e3ab6/DudeSuite)**
 - **[DumpAll](https://github.com/0xHJK/dumpall)**
 - **[GitHack](https://github.com/lijiejie/GitHack)**
 - **[GitHacker](https://github.com/WangYihang/GitHacker)**
 - **[Gobuster](https://github.com/OJ/gobuster)**
 - **[Golin](https://github.com/selinuxG/Golin)**
 - **[ihoneyBakFileScan](https://github.com/sry309/ihoneyBakFileScan)**
 - **JoomScan: Kali**
 - **[JSFinder](https://github.com/Threezh1/JSFinder)**
 - **[密探](https://github.com/kkbo8005/mitan)**
 - **[PackerFuzzer](https://github.com/rtcatc/Packer-Fuzzer)**
 - **[SSRFmap](https://github.com/swisskyrepo/SSRFmap)**
 - **[svnExploit](https://github.com/admintony/svnExploit)**
 - **[TscanPlus](https://github.com/TideSec/TscanPlus)**
 - **[URLFinder](https://github.com/pingc0y/URLFinder)**
 - **[wFuzz](https://github.com/xmendez/wfuzz)**
 - **WPScan: Kali**
 - **御剑**
> **SubDomain 子域名探测工具:**
 - **百川**
 - **[FofaView](https://github.com/wgpsec/fofa_viewer): Fofa 查询工具**
 - **[InfoSearchAll](https://github.com/ExpLangcn/InfoSearchAll)**
 - **Layer: 子域名挖掘机**
 - **[OneforAll](https://github.com/shmilylty/OneForAll)**
 - **Securitytrails: Securitytrails 官方 API 脚本**
 - **[SnowShadow](https://github.com/jinsezlb/SnowShadow)**
 - **[Subfinder](https://github.com/projectdiscovery/subfinder)**
 - **[Sublist3r](https://github.com/aboul3la/Sublist3r)**
 - **[WebBatchRequest](https://github.com/ScriptKid-Beta/WebBatchRequest)**

### <font color=orange>**[+] 权限工具 (C:\Penetration\ShellTools):**</font>

1. **[Antsword](https://github.com/AntSwordProject/AntSword-Loader): 蚁剑(已集成插件)**
2. **[Behinder](https://github.com/rebeyond/Behinder): 冰蝎**
 - **behinder 3.0 beta11**
 - **behinder 4.1**
3. **[ByPassBehinder](https://github.com/czz1233/GBByPass): JSP 免杀工具**
4. **[Cobaltstrike](https://github.com/TryGOTry/CobaltStrike_Cat_4.5): 猫猫二开**
 - **使用[CSAgent](https://github.com/Twi1ight/CSAgent)汉化**
 - <font color=green>**集成插件 (C:\Penetration\ShellTools\CobaltStrike\Scripts)**</font>
 - **[ADCollection](https://github.com/lengjibo/RedTeamTools)**
 - **[bypassav](https://github.com/hack2fun/BypassAV)**
 - **[BypassUserAdd](https://github.com/crisprss/BypassUserAdd)**
 - **[CobaltStrike_CNA](https://github.com/yanghaoi/CobaltStrike_CNA)**
 - **[CobaltStrikeShellcodeGenerator](https://github.com/RCStep/CSSG)**
 - **[erebus](https://github.com/DeEpinGh0st/Erebus)**
 - **[eventlogmaster](https://github.com/QAX-A-Team/EventLogMaster)**
 - **[LSTAR](https://github.com/lintstar/LSTAR)**
 - **[mikasa](https://github.com/Mikasazero)**
 - **mr.xie: 谢公子插件**
 - **[OLA](https://github.com/Sec-Fork/OLa)**
 - **[Pillager](https://github.com/qwqdanchun/Pillager)**
 - **[taowu](https://github.com/pandasec888/taowu-cobalt-strike)**
5. **[DNSCat2](https://github.com/iagox86/dnscat2)**
6. **[GBBypass](https://github.com/czz1233/GBByPass): 冰蝎 & 哥斯拉 Webshell 免杀**
7. **[Godzilla](https://github.com/BeichenDream/Godzilla): 哥斯拉**
8. **Kali:WSL Kali Linux 2024.1**
 - <font color=green>**username: kali password: kali**</font>
 - <font color=green>**username: root password: root**</font>
 - <font color=green>**修改软件源为阿里云**</font>
 - <font color=green>**图形化模式非常占用系统资源，建议非必要不开启。**</font>
9. **Metasploit-Framework: Kali**
10. **Msfvenom: MSF 木马生成工具**
11. **[Skyscorpion](https://github.com/shack2/skyscorpion): 天蝎**
12. **WebShell: 一句话木马(密码统一为cmd)**
 - **[Webshell](https://github.com/tennc/webshell): Webshell 收集项目**
13. **[WebshellBypassedHuman](https://github.com/Macr0phag3/webshell-bypassed-human): Webshell 免杀**
14. **[WebshellGenerate](https://github.com/cseroad/Webshell_Generate): Webshell 生成工具**
15. **[XG拟态](https://github.com/xiaogang000/XG_NTAI): Webshell 免杀工具**

### <font color=orange>**[+] 社工工具 (C:\Penetration\SocialEngineeringTools):**</font>

1. **[Mip22](https://github.com/makdosx/mip22): 钓鱼工具**
2. **[SocialEngineeringToolkit](https://github.com/trustedsec/social-engineer-toolkit): 社工工具包(Kali)**
3. **[SocialFish](https://github.com/UndeadSec/SocialFish): 钓鱼工具**
4. **[Swaks](https://github.com/jetmore/swaks): 邮件伪造工具**

### <font color=orange>**[+] 系统工具 (C:\Penetration\SystemTools):**</font>

1. **7-Zip: 23.0 单文件版**
2. **[AAct](https://ghxi.com/aact.html): 激活工具**
3. **[Bandizip](https://ghxi.com/bandizip.html): 压缩工具(注册版)**
4. **[curl](https://curl.se/)**
5. **[Dism++](https://github.com/Chuyu-Team/Dism-Multi-language): 系统调节工具**
6. **[Everything](https://ghxi.com/everything.html): 搜索工具**
7. **[Git](https://git-scm.com/)**
8. **[HackBGRT](https://github.com/Metabolix/HackBGRT): Windows 开机 Logo 更换工具**
9. **IOBit:**
 - **[AdvancedSystemcare](https://ghxi.com/advancedsystemcareultimate.html): 优化清理工具(注册版)**
 - **[DriverBooster](https://ghxi.com/iobitdriverbooster.html): 驱动工具(注册版)**
 - **[SmartDefrag](https://ghxi.com/iobitsmartdefrag.html): 磁盘整理工具(注册版)**
 - **[Uninstaller](https://ghxi.com/iobituninstaller.html): 卸载工具(注册版)**
10. **Keyboard2Mouse: 键盘操作鼠标**
11. **[Maye](https://ghxi.com/mayelite.html): 快捷启动工具**
12. **[MenuManager](https://ghxi.com/contextmenumanager.html): 右键菜单管理工具**
13. **[NTLite](https://www.ntlite.com/): 系统调节工具**
14. **[PCMaster](https://ghxi.com/pcmaster.html): 系统调整工具**
 - <font color=green>**已创建右键快捷菜单:**</font>
 - **在此处打开 Terminal 终端**
 - **在此处打开 Kali Linux 终端**
 - **在此处打开 Git 终端**
 - **在此处打开Notepad**
 - **控制面板**
 - **计算器**
 - **注册表**
15. **UltraISO: iso编辑工具**
16. **[wget](https://github.com/rockdaboot/wget2)**

### <font color=orange>**[+] 主题工具 (C:\Penetration\ThemeTools):**</font>

1. **ICON: 图标**
2. **[ICONSext](https://www.nirsoft.net/utils/iconsext.html): 图标提取工具**
3. **[MacType](https://github.com/snowie2000/mactype): 更换字体工具**
4. **OldNewExplorer: 资源管理器调整工具**
5. **Refresh: 图标缓存刷新工具**

### <font color=orange>**[+] 流量工具 (C:\Penetration\TrafficTools):**</font>

1. **BlueTeamTools: 流量解密工具**
2. **BurpSuite: 2024.2.1(注册版)**
 - <font color=green>**集成插件:**</font>
 - **[汉化](https://github.com/funkyoummp/burpsuitecn)**
 - **[BurpFastJsonScan](https://github.com/pmiaowu/BurpFastJsonScan)**
 - **[BurpJSLinkFinder](https://github.com/InitRoot/BurpJSLinkFinder)**
 - **[BurpShiroPassiveScan](https://github.com/pmiaowu/BurpShiroPassiveScan)**
 - **[403Bypasser](https://github.com/sting8k/BurpSuite_403Bypasser)**
 - **[burp-vulners-scanner](https://github.com/vulnersCom/burp-vulners-scanner)**
 - **[ChangeuUnicode](https://github.com/coffeehb/tools/tree/5c7fef3ff99ac4f80dcb52c73f70181848053315/burpUnicode)**
 - **[ChunkedCodingConverter](https://github.com/c0ny1/chunked-coding-converter)**
 - **[DomainHunterPro](https://github.com/bit4woo/domain_hunter_pro)**
 - **[FakeIP](https://github.com/TheKingOfDuck/burpFakeIP)**
 - **[FransLinkfinder]()**
 - **[Hackbar](https://github.com/d3vilbug/HackBar)**
 - **[Log4j2Scan](https://github.com/whwlsfb/Log4j2Scan)**
 - **[Sqlmap4burp](https://github.com/c0ny1/sqlmap4burp-plus-plus)**
 - **[TsojanScan](https://github.com/Tsojan/TsojanScan)**
 - **[TurboIntruder](https://github.com/PortSwigger/turbo-intruder)**
3. **[FiddlerDebugger](https://ghxi.com/fiddler.html): 流量抓包工具(汉化版)**
4. **[FiddlerEverywhere](https://github.com/msojocs/fiddler-everywhere-enhance): 流量抓包工具(注册版)**
5. **Firefox:firefox 49.0 集成插件版**
6. **ftpServers: FTP 开启工具**
7. **[LiqunShield](https://github.com/Liqunkit/LiqunShield): Webshell流量分析工具**
8. **[Netcat](https://netcat.sourceforge.net/): NC**
9. **[NetSetMan](https://ghxi.com/netsetman.html): 网络参数设置工具**
10. **[OpenVPN](https://openvpn.net/): VPN 工具**
10. **[phpStudy](https://www.xp.cn/): 集成环境**
11. **[Proxifier](https://www.proxifier.com/): 流量代理工具(注册版)**
12. **[ShadowSocks](https://github.com/shadowsocks/shadowsocks-windows): 科学上网工具**
13. **[TorBowser](https://www.torproject.org/): 洋葱浏览器**
14. **[v2rayN](https://github.com/2dust/v2rayN): 科学上网工具**
15. **[WireShark](https://www.wireshark.org/): 流量抓包分析工具**
16. **[Yakit](https://github.com/yaklang/yakit)**

# <font color=blue>**全套虚拟机镜像:**</font>

1. **Windows 7 x64**
2. **Windows 8 x64**
3. **Windows 10 x64**
4. **Windows Server 2008 x64**
5. **Windows Server 2012 x64**
6. **Windows Server 2016 x64**
7. **Windows Server 2019 x64**
8. **Ubuntu 20 x64**

**所有虚拟机镜像均安装：**

 - **VMTools**
 - **7z**
 - **Microsoft Visual C++ 2008-2022 运行库**
 - **密钥或激活工具激活**

**可供测试软件，环境搭建等用途。**
<font color=green>**虚拟机账号密码已备注在 VMware 描述栏处，请注意查看。**</font>

# <font color=blue>**下载链接:**</font>
 - **[v5.0](https://github.com/makoto56/penetration-suite-toolkit/releases/tag/v5.0)**

# <font color=blue>**参考截图:**</font>
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/%E6%88%AA%E5%9B%BE/%E5%BC%80%E5%A7%8B%E8%8F%9C%E5%8D%95.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/%E6%88%AA%E5%9B%BE/%E5%BF%AB%E6%8D%B7%E5%90%AF%E5%8A%A8.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/%E6%88%AA%E5%9B%BE/%E7%A8%8B%E5%BA%8F%E5%8F%82%E6%95%B0.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/%E6%88%AA%E5%9B%BE/%E7%A8%8B%E5%BA%8F%E7%9B%AE%E5%BD%95.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/%E6%88%AA%E5%9B%BE/%E8%B5%84%E6%BA%90%E5%8D%A0%E7%94%A8.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/%E6%88%AA%E5%9B%BE/kali.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/%E6%88%AA%E5%9B%BE/kali%E5%9B%BE%E5%BD%A2%E5%8C%96.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/%E6%88%AA%E5%9B%BE/%E5%9B%BE%E6%A0%87%E7%BE%8E%E5%8C%961.png)
![image](https://github.com/makoto56/penetration-suite-toolkit/blob/main/%E6%88%AA%E5%9B%BE/%E5%9B%BE%E6%A0%87%E7%BE%8E%E5%8C%962.png)
