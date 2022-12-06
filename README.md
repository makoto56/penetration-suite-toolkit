# **Windows10 Penetration Suite Toolkit within Kali Linux v4.0**
![image](https://img.shields.io/badge/Author-Makoto56-blueviolet.svg) ![image](https://img.shields.io/badge/Platform-Windows-red.svg) ![image](https://img.shields.io/badge/WSL-Kali-9cf.svg) ![image](https://img.shields.io/badge/Property-%E6%AD%A6%E5%99%A8%E5%BA%93-brightgreen.svg) ![image](https://img.shields.io/badge/Version-4.0-yellow.svg) ![image](https://img.shields.io/badge/Update-2022.12.06-blue.svg)

# **2022.12.06 更新说明：**

1. **由于Kali的图形化模式占用资源造成卡顿，且使用率不高，~~特此去除图形化模式~~。**
> **如有需要可参照 https://blog.csdn.net/weixin_44285782/article/details/107442217**
2. **补充了大量实用工具，升级部分软件为最新版；**
3. **重构了“漏洞工具” 的目录分类，查找更方便快捷；**
4. **重构了开始菜单及快捷启动索引；**
5. **特别鸣谢：**
> **@棉花糖网络安全圈 @利刃信安 @果核剥壳 @雨苁 @狐狸说安全 @暗魂攻防实验室**

# **系统简介：**

1. **基于Win10 Workstation 21H2 x64 原版镜像制作（不适用于ARM设备）；**
2. **完整安装WSL Kali Linux 2022.3；**
3. **精简系统自带软件，美化字体及部分图标，适度优化；**
4. **使用单磁盘文件存储，提升性能；**
 - **推荐运行环境：**
 - **vmware：16.x（vmware图形内存1G）**
 - **运行内存：8G**
 - **固态硬盘：200G**
# **制作声明：**

1. **所有的安装类软件均下载自软件对应的官方网站；**
2. **所有的绿色类软件均下载自果核剥壳 https://www.ghxi.com**
3. **所有的脚本类工具均下载自github。**
4. **部分授权类工具（破解版）及优秀的渗透工具来自微信公号分享；**
 - **排名不分先后，同时也推荐大家关注，一起变得更强。**
> **雾晓安全、果核剥壳、归零安全、潇湘信安、学蚁致用、谢公子学安全、利刃信安、棉花糖网络安全圈、狐狸说安全、HACK技术沉淀营、无尾熊安全、T00ls、渗透攻击红队、洛米唯熊、雷石安全实验室、酒仙桥六号部队、InBug实验室、鸿鹄实验室、黑白之道、HACK之道、GobySec、Gcow安全团队、Gamma实验室、CobaltStrike实战、网络安全与黑客技术、QZ的安全悟道、菜鸟学信安、乌雲安全、白帽子飙车路、信安之路、chaosec、鸟哥谈安全、安全小飞侠、moonsec、系统安全运维、天驿安全、零组攻防实验室、Lemonsec、橘猫学安全、Hacking黑白红、渗透安全团队、渗透xiao白帽、白帽子社区、HACK学习呀、猪猪谈安全、开普勒安全团队、吾爱破解论坛、WhITECat安全团队、寻云安全团队、Khan安全攻防实验室、Bypass、天億网络安全、关注安全技术、玄魂工作室、边界骇客、零度安全攻防实验室、WgpSec狼组安全团队、黑白天实验室、靶机狂魔、渗透云笔记、TeamsSix、hijackY、重生信息安全、TimeLine Sec、GobySec、Gcow安全团队、冰蚕实验室。**
5. **本集成环境是根据本人渗透工作和学习中的侧重点进行制作，不可能做到满足所有人的需求。**
6. **本项目制作的初衷是帮助渗透新手快速搭建工作环境，工欲善其事，必先利其器；**
7. **本项目由于后期调试原因可能会遗留部分本人的信息，请直接忽视；**
8. **本项目坚决不接受也从未曾接受任何形式的赞助。**
9. **如果您有好的意见或者建议，请联系邮箱 burpsuite@qq.com。**

# **免责声明：**

1. **本镜像仅面向合法授权的企业安全建设行为，如您需要测试本镜像的可用性，请自行搭建靶机环境；**
2. **在使用本镜像进行检测时，您应确保该行为符合当地的法律法规，并且已经取得了足够的授权；**
3. **如您在使用本镜像的过程中存在任何非法行为，您需自行承担相应后果，作者将不承担任何法律及连带责任。**
4. **本镜像所使用的工具资源均来自于网友投稿及互联网整理，作者仅提供分享交流平台，不为其版权负责。如果您发现本镜像中有侵犯您（或贵司）知识产权的资源，请及时反馈，作者会第一时间进行修改或删除。**

# **软件及工具介绍：**

## **系统环境类：**

1. **Directx**
2. **Net Framework 3.5**
3. **Net Framework 4.8**
4. **Microsoft C runtime library**
5. **Microsoft visual C++ 2005-2022**
6. **集成常用字库**

## **WindowsApp类：**

1. **WSL Kali Linux**
2. **Windows Terminal（已替换默认cmd）**

## **其他工具类 （C:\Softwares）：**

1. **AAct: 激活工具（激活windows & office）**
2. **Bandicam: 视频录制工具（注册版）**
3. **Bandizip: 压缩工具（注册版）**
4. **Chrome: 108.0.5359 绿色修改版**
 - **主要集成插件:**
 - **Adblock: 广告拦截工具**
 - **Charset：修改网页编码工具**
 - **Chrome清理大师: chrome清理工具**
 - **Editthiscookie: cookie编辑工具**
 - **FindSomething：敏感文件搜集工具**
 - **Fofa view：fofa工具**
 - **Funnel search：google搜索工具**
 - **Hackbar**
 - **Hack-Tools：红队综合小工具**
 - **Heimdallr：指纹识别、蜜罐特征告警工具**
 - **IE Tab：ie兼容模式工具**
 - **Infinity：标签页工具**
 - **IP address and domain inf: ip&domain探测工具**
 - **IP whois: whois 探测工具**
 - **Neater bookmarks: 书签管理工具**
 - **Octotree: github资源树查看工具**
 - **Onetab：标签管理工具**
 - **Penetration Testing Kit：红队综合小工具**
 - **Postwoman：接口调试工具**
 - **Proxy switchyomega：代理切换工具**
 - **Seoquake：网页统计工具**
 - **Supercopy：超级复制**
 - **Tampermonkey：脚本工具**
 - **User-Agent Switcher：浏览头切换工具**
 - **Toolbox 常用工具: 集成常用小工具**
 - **Vulners Web Scanner：微型漏洞扫描工具**
 - **Wappalyzer：网页技术分析工具**
 - **WebSocket Test Client：websocket工具**
 - **Whatruns：网页技术分析工具**
 - **XSS辅助工具**
 - **X情报查询助手：微步社区**
 - **YetAnotherDragAndGo: 超链接拖拽新窗口打开**
 - **ZoomEye Tools**
 - **类似的网站**
5. **Contextmenumanager：右键菜单管理工具**
6. **Dism++: 系统调节工具**
7. **Everything: 搜索工具（已禁用windows自带搜索）**
8. **Goldwave：音频编辑工具**
9. **GoogleEarth：谷歌地球**
10. **Honeyview: 看图工具**
11. **Huorong: 杀毒工具（C:\Penetration 为白名单）**
12. **ICON：第三方图标包**
13. **Internet Download Manager：6.41.6（注册版）**
14. **IOBit:**
 - **AdvancedSystemcare: 优化清理工具（注册版）**
 - **DriverBooster：驱动工具（注册版）**
 - **SmartDefrag: 磁盘整理工具（注册版）**
 - **Uninstaller: 卸载工具（注册版）**
15. **Mactype：字体管理工具（已修改系统默认字体为Mac苹方体）**
16. **Maye: 快捷启动工具**
17. **Meitu：美图秀秀**
18. **OldNewExplorer: 资源管理器调节工具**
19. **PCMaster: 系统调整工具**
 - **已创建右键快捷菜单：**
 - **在此处打开Terminal终端**
 - **在此处打开KaliLinux终端**
 - **在此处打开Notepad**
 - **控制面板**
 - **计算器**
 - **注册表**
20. **Potplayer: 视频播放工具**
21. **Refresh：刷新图标缓存**
22. **Snipaste: 截图工具**
23. **Telegram：电报客户端**
24. **UltraISO：iso编辑工具**
25. **WPS：WPS（注册版）**

## **渗透测试类（C:\Penetration）：**

1. **常用的python、C#及java类工具均配有start.bat或start.vbs。**
2. **注明工具版本及更新时间**
3. **注明依赖环境**
4. **注明主要参数**
5. **注明简要用法（给工具不给用法的都是耍流氓）**

### **[+] 安卓工具:**

1. **AndroidHelper：apk逆向工具**
2. **AndroidKiller：apk综合工具**
3. **Apkinfo：apk分析工具 https://github.com/bihe0832/Android-GetAPKInfo**
4. **Apktool：apk反编译工具 https://github.com/iBotPeaches/Apktool**
5. **ApkToolbox：apk综合工具**
6. **ApkToolPlus：apk反编译分析工具 https://github.com/linchaolong/ApkToolPlus**
7. **AppMessenger：apk分析工具 https://github.com/sulab999/AppMessenger**
8. **Dex2jar：dex打包工具 https://github.com/pxb1988/dex2jar**
9. **Nox：夜神安卓模拟器（安卓9.0）**
 - **已安装:**
 - **Debug Proxy**
 - **HttpCanary**
 - **JuiceSSH**
 - **MT**
 - **Net Capture**
 - **NP**
 - **Packet Capture**
 - **ProxyDroid**
 - **Terminal Emulator**
 - **开发者助手**
10. **Yaazhini：apk漏洞扫描工具 https://www.vegabird.com/yaazhini/**

### **[+] 免杀工具：**

1. **Aniya：https://github.com/piiperxyz/AniYa**
2. **AVevasion：https://github.com/1y0n/av_evasion_tool**
3. **Bypass-antivirus：免杀教程**
4. **Charlotte：https://github.com/9emin1/charlotte**
5. **Cool：https://github.com/ed1s0nz/cool**
6. **DarkArmour：https://github.com/bats3c/darkarmour**
7. **GLLloader：https://github.com/INotGreen/Gllloader**
8. **Invoke-Obfuscation：https://github.com/danielbohannon/Invoke-Obfuscation**
9. **Loader：https://github.com/Avienma/shellcode_loader**
10. **Powershell-Obfuscation：https://github.com/H4de5-7/powershell-obfuscation**
11. **Sandboxie：沙盒工具**
12. **ShellcodeLoader：https://github.com/knownsec/shellcodeloader**
13. **VMProtect: 加壳工具**
14. **VProtect: 加壳工具**
15. **ZheTian：遮天shellcode加载工具 https://github.com/yqcs/ZheTian**

### **[+] 连接工具：**

1. **Anydesk**
2. **Filezilla**
3. **Finalshell**
4. **MobaXterm**
5. **Putty**
6. **Teamviewer**
7. **WinSCP**
8. **Xmanager**

### **[+] 破解工具：**

1. **AccessCrack：access密码破解工具**
2. **Advanced Archive Password Recovery: 压缩包密码破解工具**
3. **Advanced Office Password Recovery: office密码破解工具**
4. **Advanced PDF Password Recovery: pdf密码破解工具**
5. **DecryptPassword**
 - **文件夹下集成下列密码破解工具：**
 - **finalshell-decoder：https://github.com/passer-W/FinalShell-Decoder**
 - **finalshellPasswordDecoder：https://github.com/qurikuduo/finalshellPasswordDecoder**
 - **firefox_decrypt：https://github.com/unode/firefox_decrypt**
 - **FireFox-Thief：https://github.com/LimerBoy/FireFox-Thief**
 - **hack-browser-data-windows：https://github.com/moonD4rk/HackBrowserData**
 - **how-does-navicat-encrypt-password：https://github.com/HyperSine/how-does-navicat-encrypt-password**
 - **how-does-SecureCRT-encrypt-password：https://github.com/HyperSine/how-does-SecureCRT-encrypt-password**
 - **how-does-Xmanager-encrypt-password：https://github.com/HyperSine/how-does-Xmanager-encrypt-password**
 - **Safe360Browsergetpass**
 - **SharpDecryptPwd：https://github.com/uknowsec/SharpDecryptPwd**
 - **teamviewer-dumper：https://github.com/attackercan/teamviewer-dumper**
 - **vcenterExsi_PwdDecrypt**
 - **winscppasswd：https://github.com/anoopengineer/winscppasswd**
6. **Hydra: 口令爆破工具 https://github.com/vanhauser-thc/thc-hydra**
7. **MD5Crack：md5碰撞工具**
8. **SNETCracker：超级弱口令破解工具**
9. **WebshellCrack：一句话密码破解工具**
 - **K8_FuckOneShell**
 - **K8_OneShellCrack**
 - **T00ls综合一句话爆破工具**

### **[+] 数据工具：**

1. **AnotherRedisDesktopManager：redis管理工具**
2. **DatabaseBrowser：mdb & xls数据库查看工具**
3. **DatabaseUtilizationTools：数据库利用工具**
4. **HeidiSQL：数据库连接管理工具**
5. **Microsoft SQL Server：2019专业版**
 - **username：sa**
 - **password：sqladmin**
6. **Microsoft SQL Server Management：mssql连接工具**
7. **Navicat: 数据库连接管理工具**
8. **Neo4j：neo4j数据库管理工具**
9. **OracleShell：oracle利用工具**
10. **RedisDesktopManager：redis管理工具**
11. **SharpSqlTools：mssql数据库利用工具**
12. **Sqlite：sqlite数据库管理工具**
13. **Sqlknife：mssql数据库利用工具**
14. **Sqlmap: 注入工具**
15. **SQLTools：mssql利用工具**
16. **Sylas：mssql & orcle & postgresql数据库利用工具**
17. **ToadOracle：oracle数据库管理工具**

### **[+] 夺旗工具（CTF）：**

1. **ASCII**
2. **BehinderDecode**
3. **BerylEnigma**
4. **Binwalk**
5. **BlindWatermark**
6. **CaptfEncoder**
7. **Converter**
8. **CRCCalculator**
9. **CTFEditor**
10. **CTFTools**
11. **CTFcrack**
12. **CyberChef**
13. **DesTool**
14. **F5Steganography**
15. **FindFlag**
16. **Foremost**
17. **GifTools**
18. **GNUplot**
19. **JPHS**
20. **MossTool**
21. **LSBSteganography**
22. **MP3Steno**
23. **NamoGif Animator**
24. **Outguess**
25. **PcapTool**
26. **PixRecovery**
27. **PNGCalculator**
28. **PNGCheck**
29. **PNGDebugger**
30. **QRResearch**
31. **QRCode**
32. **Regular**
33. **RSATool**
34. **RSA_N**
35. **SM4**
36. **Steganography**
37. **Stegdetect**
38. **Steghide**
39. **Stegsolve**
40. **Taowa Tool**
41. **Tweak PNG**
42. **Volatility**
43. **Volatility Workbench**
44. **wbStego**
45. **WinHex**
46. **Xiaokui**
47. **ZZYQR**
48. **ctf 密码学知识点总结**
49. **ctf 逆向知识点总结**
50. **ctf 隐写术知识点总结**

### **[+] 字典工具：**

1. **DictMaker：字典生成工具**
 - **PwdBUD：https://github.com/ort4u/PwdBUD**
 - **黑刀字典生成工具**
 - **火花字典生成工具**
 - **木头字典生成工具**
 - **品轩字典生成工具**
 - **易优字典生成工具**
2. **fuzzDicts：https://github.com/TheKingOfDuck/fuzzDicts**
3. **pentestdicts：https://github.com/ppbibo/pentesterspecialdict**

### **[+] 磁盘工具：**

1. **Diskgenius: 注册版（可恢复硬盘数据）**
2. **SSDfresh：ssd优化工具**

### **[+] 编辑工具：**

1. **010Editor: 十六进制编辑工具（注册版）**
2. **BeyondCompare：文件对比工具**
3. **eSearch：截屏、录屏、OCR、搜索、翻译、贴图、以图搜图（已集成离线OCR库）**
4. **FFRename：菲菲更名宝贝（专业版）**
5. **FindStr: 文本检索工具**
6. **FireKylin：系统痕迹采集 https://github.com/MountCloud/FireKylin**
7. **Fortify：代码审计工具22.1.0（已集成rules）（注册版）**
8. **JavaDecompiler: java查看编辑工具**
9. **Jsonview: json查看编辑工具**
10. **LogParse：windows日志分析工具**
11. **LogParseLizard：windows日志分析工具（图形化）**
12. **myBase：个人数据库编辑工具（注册版）**
13. **Notepad++: 编辑工具**
14. **PSTConverter：pst邮件转换工具**
15. **Seay：php代码审计工具**
16. **SeayDzend：php zend解密工具**
17. **SharpSword：csharp版本word查看工具**
18. **Sublime: 编辑工具（注册版）**
19. **Typora：MarkDown编辑工具（注册版）**  
20. **VSCode：VisualCode编辑工具**
21. **WindowsLogsAnalysis：windows日志分析工具（图形化）**
22. **XMind：思维导图工具**
23. **YoudaoDict：有道词典（注册版）（已集成离线翻译库）**

### **[+] 漏洞工具：**

1. **AlibabaNacos**
2. **Apache**
3. **Cacti**
4. **Cas**
5. **Chrome**
6. **Citrix**
7. **CMSHunter**
8. **Confluence**
9. **D-Link**
10. **Database**
 - **mongo**
 - **mssql**
 - **mysql**
 - **redis**
11. **Elasticsearch**
12. **F5-BIG-IP**
13. **FastAdmin**
14. **Fastjson**
15. **FCKEditor**
16. **FusionAuth**
17. **Gitlab**
18. **Harbor**
19. **HTTPBasic**
20. **HTTPFileServer**
21. **IIS**
22. **ILO4**
23. **Intellian-Aptus-Web**
24. **Jboss**
25. **Jellyfin**
26. **Jenkins**
27. **Jira**
28. **JumpServer**
29. **Kibana**
30. **Liferay**
31. **Linux**
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
 - **...**
32. **Mail**
 - **coremail**
 - **exchange**
 - **zimbra**
33. **MetaCRM**
34. **ModSecurity**
35. **Nexus**
36. **Node.js**
37. **OA**
 - **seeyon**
 - **tongda**
 - **weaver**
38. **Office**
39. **Open-AudIT**
40. **Others**
41. **PHP-FPM**
42. **PHP**
43. **phpMyadmin**
44. **PHPStudy**
45. **Rconfig**
46. **SaltStack**
47. **Sangfor**
48. **SAP**
49. **Shiro**
50. **ShowDoc**
51. **Solarwinds**
52. **Spring**
53. **Struts2**
54. **Sunlogin**
55. **TeamViewer**
56. **Tomcat**
57. **Tools**
 - **AliyunAKTools：阿里云利用工具**
 - **AptTools：综合漏洞利用工具**
 - **CF：云环境利用框架 https://github.com/teamssix/cf**
 - **CodeTest：综合漏洞利用工具 https://github.com/codeyso/CodeTest**
 - **docs-0sec：零组文档库**
 - **docs-base：漏洞文档库**
 - **Fuxploider：漏洞扫描工具 https://github.com/almandin/fuxploider**
 - **Gr33k：综合漏洞利用工具 https://github.com/lijiaxing1997/Gr33k**
 - **~~HVVExploitApply：寻云安全团队1.5 综合漏洞利用工具（未取得授权，特此删除）~~**
 - **LiqunKit：综合漏洞利用工具**
 - **MYExploit：综合漏洞利用工具 https://github.com/achuna33/MYExploit**
 - **NSudoLG：windows提权工具 https://github.com/Thdub/NSudo_Installer**
 - **Nuclei：内网扫描工具 https://github.com/projectdiscovery/nuclei**
 - **OATools：OA漏洞利用工具**
 - **POCbomber：综合漏洞利用工具 https://github.com/tr0uble-mAker/POC-bomber**
 - **poc2jar：综合漏洞利用工具 https://github.com/f0ng/poc2jar**
 - **Ruoyi-All：综合漏洞利用工具 https://github.com/thelostworldFree/Ruoyi-All**
 - **Shenji：综合漏洞利用工具 https://github.com/yhy0/ExpDemo-JavaFX**
 - **SuperXray：综合漏洞利用工具 https://github.com/4ra1n/super-xray**
 - **Vulmap：综合漏洞利用工具 https://github.com/zhzyker/vulmap**
 - **WinExpSuggester-NG：windows提权工具 https://github.com/bitsadmin/wesng**
 - **WinExpSuggester：windows提权工具 https://github.com/0xToast/Windows-Exploit-Suggester-Py-3**
 - **Xray：漏洞扫描工具 https://github.com/chaitin/xray**
 - **Ysoserial**
58. **TPLink**
59. **VMware**
60. **Weblogic**
61. **Webmin**
62. **Windows**
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
63. **XenMobile**
64. **XStream**
65. **XXL-job**
66. **Ysuserial**
67. **Zoho**
68. **Zyxel**
> **漏洞库综合了下列项目：**
 - **CMSHunter：https://github.com/SecWiki/CMS-Hunter**
 - **expHub：https://github.com/zhzyker/exphub**
 - **Middleware-Vulnerability-Detection：https://github.com/mai-lang-chai/middleware-vulnerability-detection**
 - **System-Vulnerability：https://github.com/mai-lang-chai/system-vulnerability**
 - **Vulnerability：https://github.com/edgesecurityteam/vulnerability**
> **更多漏洞exp见 C:\Penetration\ExpolitTools（漏洞exp较多，请善用everything搜索）**

### **[+] 内网工具：**

1. **3Gstudent：三好学生powershell & python脚本 https://github.com/3gstudent**
2. **ABPTTS：内网穿透工具 https://github.com/nccgroup/ABPTTS**
3. **AddUser: 添加用户工具**
4. **ADExplore：ldap工具**
5. **ADinfo：内网信息搜集工具 https://github.com/lzzbb/Adinfo**
6. **Aoratos：软件运行痕迹清理工具 https://github.com/PinoyWH1Z/AoratosWin**
7. **BloodHound：域渗透分析工具**
8. **BloudyAD：域渗透利用工具**
9. **BruteLogon：windows口令爆破工具**
10. **ClearLogs：windows日志清除工具**
11. **CrackMapExec：内网综合利用工具 https://github.com/Porchetta-Industries/CrackMapExec**
12. **DefeatDefender：关闭defender工具 https://github.com/Back-X/Defeat-Defender**
13. **DomainTools：域渗透综合利用工具 https://github.com/SkewwG/domainTools**
14. **DomainInfoFind：获取域内机器的桌面文件 https://github.com/wangfly-me/DomainInfo_Find**
15. **EarthWorm: 内网穿透工具**
16. **Frp: 内网穿透工具 https://github.com/fatedier/frp**
17. **FScan：内网扫描工具 https://github.com/shadow1ng/fscan**
18. **GetWinInfo：windows信息搜集工具**
19. **Gorailgun：内网渗透综合利用工具**
 - **password：三个空格**
19. **GoToHTTP：远控工具 https://gotohttp.com/**
20. **Hoaxshell：远控工具 https://github.com/t3l3machus/hoaxshell**
21. **impacket：内网协议工具 https://github.com/SecureAuthCorp/impacket**
22. **iox：流量代理工具 https://github.com/EddieIvan01/iox**
23. **Ladon：内网扫描工具（小密圈9.3版本）**
24. **LCX：端口转发工具**
25. **LdapAdmin：ldap工具**
26. **LDAPDomainDump：ldap工具 https://github.com/dirkjanm/ldapdomaindump**
27. **Mimikatz：密码抓取工具**
> **文件夹下集成下列密码抓取工具**
 - **gosecretsdump：https://github.com/C-Sto/gosecretsdump**
 - **hklm**
 - **kekeo：https://github.com/gentilkiwi/kekeo**
 - **lazagne：https://github.com/AlessandroZ/LaZagne**
 - **mimipenguin：https://github.com/huntergregal/mimipenguin**
 - **ntdsdumpex：https://github.com/zcgonvh/NTDSDumpEx**
 - **procdump**
 - **pwdump：https://www.openwall.com/passwords/windows-pwdump**
 - **quarkspwdump：https://blog.quarkslab.com/quarks-pwdump.html**
28. **Mip22：网页钓鱼工具 https://github.com/makdosx/mip22**
29. **Moonwalk：linux取证工具 https://github.com/mufeedvh/moonwalk**
30. **Nacs：内网扫描工具 https://github.com/u21h2/nacs**
31. **NC: 监听工具**
32. **Neo-reGeorg：regeorg重构版 https://github.com/L-codes/Neo-reGeorg**
33. **NetSpy：内网网段探测工具 https://github.com/shmilylty/netspy**
34. **NPS：内网代理工具 https://github.com/ehang-io/nps**
35. **OpenRDP：开启远程桌面工具**
36. **OpenSSH：ssh工具**
37. **Pack：打包工具**
 - **7z（单文件版）**
38. **PE：WeiPE镜像 https://www.wepe.com.cn/**
39. **PEASS-ng：linux取证工具 https://github.com/carlospolop/PEASS-ng**
40. **PowerProxy：powershell代理工具 https://github.com/get-get-get-get/PowerProxy**
41. **PowershDLL：powershell工具 https://github.com/p3nt4/PowerShdll**
42. **PS2EXE：powershell转exe工具**
43. **PSTools：微软psexec工具 https://learn.microsoft.com/en-us/sysinternals/downloads/pstools**
44. **PyStinger：流量代理工具 https://github.com/FunnyWolf/pystinger**
45. **ReverseShell：反弹shell工具**
46. **revsh：内网穿透工具 https://github.com/emptymonkey/revsh**
47. **Scan4all：内网扫描工具 https://github.com/hktalent/scan4all**
48. **ScheduleRunner：计划任务利用工具 https://github.com/netero1010/ScheduleRunner**
49. **SharpTools：**
 - **CatchBrowser：浏览器密码抓取工具**
 - **SharpAdiDnsDump：域dns枚举工具 https://github.com/b4rtik/SharpAdidnsdump**
 - **SharpDecryptPwd：浏览器密码解密工具 https://github.com/RowTeam/SharpDecryptPwd**
 - **SharpEventLog：日志分析工具 https://github.com/uknowsec/SharpEventLog**
 - **SharpHound：域渗透分析工具 https://github.com/BloodHoundAD/SharpHound**
 - **SharpListRDPConnections：rdp连接记录枚举工具**
 - **SharpNetCheck：出网探测工具 https://github.com/uknowsec/SharpNetCheck**
 - **SharpRDPLog：rdp连接记录枚举工具 https://github.com/Adminisme/SharpRDPLog**
 - **SharpStrike：cobaltstrike工具 https://github.com/iomoath/SharpStrike**
 - **SharpWxDump：微信解密工具 https://github.com/AdminTest0/SharpWxDump**
50. **StopDefender：关闭defender工具 https://github.com/lab52io/StopDefender**
51. **Stowaway：内网穿透工具 https://github.com/ph4ntonn/Stowaway**
52. **SweetBabyScan：内网扫描工具 https://github.com/inbug-team/SweetBabyScan**
53. **Traitor：linux提权工具 https://github.com/liamg/traitor**
54. **WCE：windows凭证编辑工具 https://github.com/returnvar/wce**
55. **Wget：下载工具**
56. **wmiHacker：wmi渗透工具 https://github.com/rootclay/WMIHACKER**
> **更多内网工具见 C:\Penetration\IntranetTools**

### **[+] 办公工具：**

1. **Adobe Acrobat DC 2022：PDF编辑工具**
2. **Office: Word + Excel + Powerpoint + Access + Onenote + Outlook**
3. **WPS：Word + Excel + Powerpoint + PDF**

### **[+] 编程工具：**

1. **GCC**
2. **Golang**
3. **Java：**
 - **jre1.8.0：已配置环境变量，系统默认调用java8**
 - **jre15.0.2：绿色版，如有特殊软件需要java15环境运行可直接调用/bin/java.exe即可**
4. **Nodejs**
5. **Python：**
 - **python2：python2命令启动（python2 test.py）**
 - **python3：python3命令启动（python3 test.py）**
 - **已集成本镜像所有python3工具的pip依赖库（如有遗漏未安装的库请自行安装）**
 - **使用pip命令调用python3 pip**
6. **VisualStudio 2022：社区版**

### **[+] 逆向工具：**

1. **bat2exe：bat转exe工具**
2. **DetectItEasy：查壳工具**
3. **dnSpy：.Net逆向工具**
4. **exeScope：exe编辑工具**
5. **GreenHelper：exe绿化工具**
6. **HashMaker：hash工具**
7. **IDAPro：吾爱破解版**
8. **ILSpy：.Net逆向工具**
9. **jadx：java反编译工具**
10. **OllyDebug：exe调试工具**
11. **peidTool：查壳工具**
12. **SignTool：签名伪造工具**
13. **upxShell：upx加壳工具**
14. **vbs2exe：vbs转exe工具**
15. **x64dbg：exe调试工具**

### **[+] 扫描工具：**

1. **Acunetix: 15.1.221109177（注册版）**
 - **username: admin@awvs.com**
 - **password: Admin@awvs.com**
2. **AppScan：10.0.7（注册版）**
3. **Goby：2.0.5红队专版（含1288 poc）**
4. **Nessus：10.3.1（注册版）**
 - **username: admin**
 - **password: password**
5. **Nmap：端口扫描工具**
6. **RouterScan: C段扫描工具**
7. **ScanBox:**
> **AVScan 杀毒软件检测工具：**
 - **CheckAV（自己写的辣鸡代码，如有需要可以随便使用）**
> **LeakScan 敏感文件扫描工具：**	
 - **dirMap：https://github.com/H4ckForJob/dirmap**
 - **dirSearch：https://github.com/maurosoria/dirsearch**
 - **PackerFuzzer：https://github.com/rtcatc/Packer-Fuzzer**
 - **ScanTools：https://gitee.com/windyjxx/ScanTools**
 - **Yujian**
 - **GitHack**
 - **7KB WebPath Brute**
 - **7KB Ucenter Sniper**
 - **7KB WordPress Sniper**
 - **...**
> **SubDomain 子域名探测工具：**
 - **FofaView：fofa查询工具**
 - **InfoSearchAll：https://github.com/ExpLangcn/InfoSearchAll**
 - **Layer：子域名挖掘机**
 - **OneforAll：https://github.com/shmilylty/OneForAll**
 - **Securitytrails：Securitytrails官方api脚本**
 - **SnowShadow：https://github.com/jinsezlb/SnowShadow**
 - **Sublist3r：https://github.com/aboul3la/Sublist3r**
 - **Subfinder：https://github.com/projectdiscovery/subfinder**
 - **ThunderSearch：https://github.com/xzajyjs/ThunderSearch**
 - **WebBatchRequest：https://github.com/ScriptKid-Beta/WebBatchRequest**
 - **WebFinder：https://github.com/Liqunkit/webfinder-next**
 - **...**
> **更多扫描工具见 C:\Penetration\ScanTools\ScanBox**

### **[+] 权限工具：**

1. **AntSword: 蚁剑（已集成插件）https://github.com/AntSwordProject/AntSword-Loader**
2. **Behinder: 冰蝎（shell密码统一为rebeyond）https://github.com/rebeyond/Behinder**
 - **behinder 3.0 beta11**
 - **behinder 4.0.6**
3. **cobaltstrike: Dog 4.4 汉化版https://github.com/TryGOTry/DogCs4.4**
 - **使用csagent汉化 https://github.com/Twi1ight/CSAgent**
 - **vps启动teamserver：sudo ./teamserver your_ip your_password random.profile**
 - **集成插件（C:\Penetration\ShellTools\CobaltStrike\Scripts）**
 - **adcollection**
 - **bypassav：https://github.com/hack2fun/BypassAV**
 - **erebus：https://github.com/DeEpinGh0st/Erebus**
 - **eval**
 - **eventlogmaster：https://github.com/QAX-A-Team/EventLogMaster**
 - **ladon**
 - **mikasa：https://github.com/Mikasazero**
 - **taowu：https://github.com/pandasec888/taowu-cobalt-strike**
4. **ByPassBehinder：jsp免杀工具 https://github.com/czz1233/GBByPass**
5. **Godzilla：https://github.com/BeichenDream/Godzilla**
6. **Hema：河马webshell查杀工具**
7. **Kali：WSL Kali Linux 2022.3**
> **用户：**
 - **username：kali password：kali**
 - **username：root password：root**
 - **修改软件源为阿里云**
 - **完整安装Kali Linux所有软件包**
 - **由于Kali的图形化模式占用资源巨大，使用率较低，~~特此去除图形化模式~~。**
8. **Skyscorpion：https://github.com/shack2/skyscorpion**
9. **Shell:免杀一句话木马（密码统一为cmd）**
10. **Webshell: webshell收集项目 https://github.com/tennc/webshell**
11. **WebshellBypassedHuman：webshell免杀 https://github.com/Macr0phag3/webshell-bypassed-human**
12. **WebshellGenerate：webshell生成工具 https://github.com/cseroad/Webshell_Generate**

### **[+] 流量工具：**

1. **BlueTeamTools：流量解密工具**
2. **BurpSuite：2022.1.1** 
 - **汉化插件：https://github.com/funkyoummp/burpsuitecn**
 - **集成插件：**
 - **VulnersScanner**
 - **ChangeU**
 - **ChunkedCodingConverter**
 - **DomainHunter**
 - **FakeIP**
 - **Hackbar**
 - **Sqlmap4burp**
 - **TurboIntruder**
3. **Fiddler: 流量抓包工具（汉化版）**
4. **ftpServers: ftp开启工具**
5. **HackFirefox: firefox 49.0 集成插件版**
6. **ipChanger: ip代理工具**
7. **LiqunShield：webshell流量分析工具**
8. **NetSetMan：网络参数设置工具**
9. **OpenVPN：vpn工具**
10. **phpStudy: 8.1集成环境**
11. **Proxifier: 流量代理工具（汉化版）**
12. **ShadowSocks: 科学上网工具 https://github.com/shadowsocks/shadowsocks-windows**
13. **TorBowser: 洋葱浏览器**
14. **v2ray：科学上网工具 https://github.com/2dust/v2rayN**
15. **WireShark: 流量抓包分析工具**
16. **Yakit：https://github.com/yaklang/yakit**

# 全套虚拟机镜像：

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
**虚拟机账号密码已备注在VMware描述栏处，请注意查看。**

 - **下载链接：**
 - **链接：https://pan.xunlei.com/s/VN2xlbB9pxTo0bWdgdg5vXUtA1**
 - **提取码：fvp3**

# 下载链接：
> **小水管上传中**

# 参考截图：
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/desktop.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/soft.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/intranet-tools.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/exp-tools.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/kali1.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/kali2.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/systeminfo.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/0sec.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/android.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/nessus.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/appscan.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/awvs.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/goby.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/antsword.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/burpsuite.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/yakit.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/chrome.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/cs.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/firefox.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/fortify.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/idapro.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/navicat.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/neo4j.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/office.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/photoshop.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/visualstudio.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/vscode.png)
![image](https://raw.githubusercontent.com/makoto56/penetration-suite-toolkit/main/%E6%88%AA%E5%9B%BE/youdao.png)
