---
layout: document
title: 更新日志
categories: docs
---
# 更新日志

## Altman 2.2.1
1. 修改右键菜单显示方式（修复在Mac下的菜单不显示Bug）（2014.07.28）
	- ShellManager1.2.1
	- FileManager1.2.1
2. 修复某些情况下插件不能加载的Bug（2014.07.28）
3. 修正了之前数据库连接语句更改以后，_func.tree对应信息未更改的错误，`<connection>` -> `<sqlConnection>`（2014.08.04）


## Altman 2.2.0
1. 修改了phpEval，phpEval_BuiltIn，将echo更换为print（2014.07.08）
2. 修正了phpEval_Cookie未添加->||<-的错误（2014.07.08）
3. 添加了phpAssert类型，支持Assert函数及其变形函数（2014.07.08）
4. 程序目录结构进行局部调整（2014.07.18）
5. 数据库层代码重构，使用参数化查询方式，远离注入（2014.07.20）
6. 插件版本升级，新增数据库api与Host部分api（2014.07.20）
7. 主程序与插件支持多语言，目前为包含中英文（2014.07.22）
8. 插件PluginManager，支持安装/卸载插件（2014.07.23）


## Altman 2.1.0
新增:

1. 插件版本升级，新增部分api（2014.06.25）
2. 新增脚本类型pythonEval（2014.06.20）
3. 实现了pythonEval的shellCmder和FileManager功能（2014.06.20）
4. 将原shellmanager功能模块提取为shellmanager插件（2014.06.24）
5. 新增插件PluginManager，用于管理插件（2014.06.26）
6. DbManager插件中，添加了将查询结果保存csv功能（2014.06.27）
7. DbManager插件中，添加了右键复制节点功能（2014.06.29）
8. FileManager插件中,添加文件后缀的图标显示（2014.07.06）
9. 新增局部HttpHeader设置，可以为单个shell配置独立的HttpHeader，优先于全局HttpHeader设置（2014.07.02）

修改:

1. 修正了在linux下状态栏版本号未右对齐的bug（2014.06.24）
2. Host程序中，实现了以ShadowCopyFiles方式启动（2014.06.26）
3. aspxEval_Db.func中，修复了ExecuteReader方法某些情况下发生"Object requied"的错误（2014.06.27）
4. DbManager插件中，调大了SQL查询语句窗口的字体（2014.06.29）
5. ShellManager插件中，编辑保存shell时，添加对ini属性的xml格式合法性的检查（2014.06.30）
6. FileManager插件中：
	* 单击刷新改为双击刷新（2014.07.01）	
	* 优化了数据的显示效果（2014.07.03）
	* 对代码进行了优化（2014.07.05）
	* 修复了一些比较严重的bug（2014.07.05）
	* 重构了FileManagerService部分代码（2014.07.05）
	* 调大了列表的竖直方向的宽度（2014.07.06）


## Altman 2.0.10
1. 修复了某些时候会提示"417 expectation failed"的bug（感谢Charles Qin）（2014.06.11）
2. 修复了EditShell的数据库连接示例初始化未检查的bug（2014.06.15）
3. 修复了CmdResult部分返回结果不显示的bug（2014.06.15）
4. 修复了自定义控件TextBoxShell中，如果当前路径中包含非空字符可能会导致错误的bug（2014.06.15）
5. shellManager主窗口右键添加了复制服务端代码的功能（2014.06.15）
6. 新增脚本类型jspBig（有别于eval，功能函数均定义在服务端脚本中）（2014.06.14）
7. 实现了jspFull的shellCmder和FileManager功能（2014.06.14）


## Altman 2.0.9
1. 添加了免责声明，在程序运行前会打开免责声明（2014.06.05）
2. 添加了批量检测存活功能（2014.06.04）
3. 添加了双击直接进入FileManager插件界面的功能（如果不存在FileManager插件，则忽略）（2014.06.05）
4. 改进了新建标签页的显示方式，改为插件名|targetName，如shellcmder|TestA（2014.06.05）
5. 改进了标签页的关闭方式，关闭当前标签页会自动定位到前一个选项卡（2014.06.05）


## Altman 2.0.8
1.在主窗口添加了Altman Docs按钮，打开帮助文档。（2014.06.03）
2.文件管理插件中，使新建文件/文件夹功能全局可用（2014.06.03）


## Altman 2.0.7
1. 在主窗口添加了help按钮，包括about和developer mode选项（开发者模式可用于插件测试）（2014.06.02）
2. 添加menu菜单，提供reload shelltype和reload setting（2014.06.03）
3. 暂时屏蔽卸载插件功能（2014.06.03）
3. 数据库插件中，实现了asp的access（2014.06.02）
4. 数据库插件中，实现了php的sqlsrv（2014.06.03）


## Altman 2.0.6
1. 修复了数据库插件DataGridView显示的一个bug（2014.05.26）
2. 修复了读取.func时未设置info信息的bug（2014.05.31）
3. editshell界面中，添加了获取数据库连接字符串示例的方法（2014.05.31）
4. 数据库插件中，修改初始化逻辑为自动连接数据库、手动获取所有数据库（2014.06.01）
5. 数据库插件中，添加了ShowMsgInStatusBar方法，将结果显示在StatusBar上（2014.06.01）
6. 数据库插件中，实现了aspx的access_oldb（2014.06.01）


## Altman 2.0.5
1. 明确了免责条款（2014.05.25）
2. 完善了主程序界面（插件按钮、方法树，关于）（2014.05.25）
3. 数据库插件中，实现了asp的mssql方法（2014.05.24）


## Altman 2.0.4
1. 修改了customShellType类，在FuncCode中添加path，表示绑定的节点路径。（2014.05.23）
2. 修改了customShellType类，添加了方法树FuncTreeNode，可以以xpath（/cmder/systeminfo）方式访问。（2014.05.23）
3. 修改了customshelltypexmlhandle中customShellType配置文件的读取。（2014.05.23）
4. 根据前几条变化，更新了已有customShellType配置文件。（2014.05.23）


## 2014.05.19
1. 修改了customShellType容器的注册方法,以树节点方式注册、访问FuncCode。默认FuncCode注册到default。（2014.05.18）
2. 添加了aspxEval_Db.func和phpEval_Db.func。（2014.05.19）
3. 数据库插件中，实现php的mysql，aspx的mssql_oledb，注册方式为aspxEval/mssql_oledb和phpEval/mysql。（2014.05.19）


## 2014.05.18
1. 修复了开启随机参数名后，未判断pass是否和随机参数名相等的bug（2014.05.13）
2. 添加了数据库插件,描绘了数据库界面，和增加了一些类（2014.05.18）


## 2014.05.12
1. 创建了分支feature-DbManager（2014.05.11）
2. 修改了插件接口，将shellBaseType换成ShellStruct（2014.05.11）
3. 由于插件接口的改变，修改了插件shellcmder和fileManager（2014.05.11）
4. DbManager插件编写，实现了apsx的oledb模式的数据库、数据库表、数据库字段获取（2014.05.12）
5. 发现一个bug：开启随机参数名以后，未判断pass是否和随机参数名相等，会导致较高几率的500错误（未修复）（2014.05.12）


## 2014.05.10
1. 添加了新的脚本类型（基于Cookie通信方式）（2014.05.10）
2. 更改了README.md的一个不当描述（2014.05.10）


## 2.0.3
1. 实现了参数随机化功能（2014.05.09）
2. 修复了HttpHeader保存配置时的bug（2014.05.09）
3. 删除了工程文件中不需要的文件（2014.05.09）
4. 添加了CHANGELOG.txt文件（2014.05.09）
5. 添加了README.md文件（2014.05.09）
6. 添加了LICENSE文件，申明程序使用GPL协议（2014.05.09）


## 2.0.2
1. 修复了一个切换代理设置的bug(2014.05.07)
2. 修复了FileManager插件中下载方法中的参数个数传递错误的问题（2014.05.08）
3. 修改ShellCmder、FileManager插件中Version属性，改为自动获取Application.ProductVersion（2014.05.08）


## 2.0.1
(本版本开始采用MEF的插件架构，对之前版本进行了重构)

1. 添加了setting.xml,用于程序读取和保存配置（2014.05.07）

## Older Version
### 1.1.9
1. 将自定义脚本分为.type和.func两类（2014.04.20）
2. 修改customshelltype类型，增加了type和param,将每一个功能类的所类型和参数设置分离（2014.04.26）
3. 添加函数，处理shelltype中Item字段内容，替换$par$为par（2014.04.26）


### 1.1.8正式版本
1. 添加了about弹窗，包括一些免责声明（2014.04.08）
2. 重新添加之前版本中未引入的FileUploadOrDownloads.cs文件（2014.04.17）
3. 将程序图标和Mono.Data.Sqlite.dll引入（2014.04.17）
4. 添加了应用程序图标（2014.03.27）


### 1.1.8
1. 对ResultMatch中一些方法重构，优先判断是否匹配到了错误（ERROR://）（2014.03.26）
2. 对ResultMatch中的正则规则进行了适当修改，根据实际结果进行修改（2014.03.26）
3. 对FileEdit的构造函数进行了修改，添加了AutoLoadContent属性，判断是否需要自动加载文件内容（解决新建文件时会自动读文件的bug）（2014.03.26）
4. 添加了aspEval类型，所有功能测试通过（2014.03.26）


### 1.1.7
1. 修改了SqliteHelper中的GetDataTable方法，不使用SqliteDataAdapter，而改用SqliteDataReader（之前会报一个错误）（2014.03.19）
2. 添加了文件下载功能。使用正则匹配十六进制的方式。(实际使用string发现会有数据丢失)（2014.03.22）
3. 对ResultMatch中的正则规则进行了修改，去掉了^和$。（因为在->|，|<-之前或者之后可能会出现无用数据，比如当webshell插入在一个正常的网页中时）（2014.03.22）
4. 整理了http类（2014.03.17）
5. 更改了原来的上传下载处理类，改为FileUploadOrDownload（下载保存文件功能还没写）（2014.03.17）
6. 把上传下载进度条暂时注释掉（2014.03.17）

bug：

1. 在上传文件的时候，http连接无法及时回应，疑似http连接等待（php的存在这个问题，aspx正常）（2014.03.18）


### 1.1.6
1. 清理了一些不属于工程的无用文件。（2014.03.16）
2. 将部分界面语言暂时换为英文。（在linux下，中文字体有问题。）（2014.03.03）
3. 经过windows和linux的测试，在两个平台上解析一致，故使用sqlite3作为数据库。
（windows平台需要sqlite3.dll和Mono.Data.Sqlite.dll，linux平台需要libsqlite3.so.0和Mono.Data.Sqlite.dll）（2014.03.15）
4. 不使用xml作为数据库保存，原因在于mono和.net对于xml架构的处理结果不一致，会造成问题。(2014.03.10)
5. 将customType添加到svn

Bug：

1. 当打开本地代理，进行监控时，如果打开cmdshell，则会出现长时间无法响应，待解决。


### 1.1.5
1. 将dataset的数据和架构全都保存到xml(2014.02.27)
2. 修复了xml首次打开时，未实例化的问题(2014.02.27)


### 1.1.5
1. 实现了一个xmlHelper类，可以实现xml加密/解密，读取/修改功能(2014.02.24)
2. 考虑到跨平台问题，将本地access数据库换成了xml数据库（linux下ole支持有点问题）(2014.02.27)
3. 暂未将（1和2）功能整合起来(2014.02.27)


### 1.1.4
1. 修改了http提交类，将webClient改为httpWebRequest(2014.02.18)
2. 添加了httpProxy类，增加http/https代理功能，以及监视数据功能(2014.02.20)
3. 在主窗口添加了监视功能，即当代理地址设定为127.0.0.1：8081时，可以监视程序发送的数据和接收的数据


### 1.1.3
1. 修改了custemShellType格式，将子功能独立开，并统一由contianer进行注册管理(2014.02.09)
2. 添加了php的shellcmder功能(2014.02.09)


### 1.1.2
1. 修复完善了php/aspx类型的某些功能(2014.02.09)

	```
	PHP/ASPX（body）
	WWWRootPathCode              ok/ok
	FileTreeCode                 ok/ok
	ReadFileCode                 ok/ok
	WriteFileCode                ok/ok
	DeleteFileOrDirCode          ok/ok
	DownloadFileCode             -/-
	UploadFileCode               -/-
	CopyFileOrDirCode            ok/ok
	RenameFileOrDirCode          ok/ok
	CreateDirCode                ok/ok
	ModifyFileOrDirTimeCode      ok/ok
	WgetCode                     ok/ok
	```

2. 采用customShellType模式，启动程序时自动注册可用customShellType。由于代码调整，DownloadFileCode/UploadFileCode功能暂时不可用(2014.02.09)
3. 发现了几个隐性问题，可能会导致错误,asp内部采用unicode编码，request.write()时默认采用unicode格式。采用serverEncode/webEncode可以解决(2014.02.09)


### 1.1.1
1. 添加了aspx类型的code资源(2014.01.27)
2. 完善了customShellType向导的功能(2014.02.07)
3. 在向导中添加了新建/编辑customShellType的功能


### 1.1.0
1. 添加了有关customShellType的各种struct，enum和class(2013.12.16-20)
2. 添加了customShellType向导(2013.12.26)


### 1.0.6
1. 添加了全局设置（请求头设置和代理设置）（2013.12.01）
2. 添加了全局设置保存/载入的功能（2013.12.01）
3. 添加自定义控件（ControlRequestHeaderSetting和ControlProxySetting）（2013.12.01）
4. 暂时隐藏了main窗体下的进度条（2013.12.01）


### 1.0.5
1. 添加了header
2. 添加了模块ControlCore，主要包含自定义控件（ListViewPlus,ProgressBarPlus,ShellTextBox）（2013.11.24）
3. fileManager中的重命名，修改时间，创建文件夹改用ListViewPlus控件实现，不再用子窗体实现。（2013.11.25）
4. 修复当文件夹为空时，仍然显示匹配错误的问题（2013.11.25）

Bugs:

1. 上传文件时，最大限制为4M，超过大小就会上传失败（2013.11.16）


### 1.0.4
1. 添加全局代理设置（无代理、ie代理设置、自定义代理设置）（2013.11.19）
代码：
2. 对程序进行分层，分为几个模块：

	```
	Altman（UI层）、LogicCore（逻辑层）、WebCore（网络操作层）、DatabaseCore（数据库层）、ModelCore（数据结构共享层）。
	他们的关系为：
	Altman    <==>    LogicCore    <==>    DatabaseCore
									||
									WebCore
	```
（2013.11.22）

Bugs:

1. 上传文件时，最大限制为4M，超过大小就会上传失败（2013.11.16）


### 1.0.3
代码：

1. 重写命令传输的方式，改用继承于WebClient的HttpClient类。普通命令采用同步上传方式；下载文件采用异步下载方式；上传大文件采用异步上传方式。（2013.11.15）
2. 统一命令参数模板，改用static方式，配合后期全局设置（2013.11.16）
3. 新增了自定义的异常类，包括local，request和response三个阶段的错误提示（2013.11.16）
4. 重写上传下载文件类；文件上传分两个阶段：文件准备阶段和文件上传阶段，对于大文件上传进度更加直观（2013.11.17）

Bugs:

1. 上传文件时，最大限制为4M，超过大小就会上传失败（2013.11.16）


### 1.0.2
fileManager：

1. 下载文件到本地（2013.11.14）


### 1.0.1
现有功能:

shellManager：

1. 添加shell功能（2013.11.06）
2. 删除shell功能（2013.11.06）
3. 编辑shell功能（2013.11.06）
4. 打开虚拟终端功能（2013.11.06）
5. 打开文件管理功能（2013.11.06）

shellCmder：

1. 系统基本信息检查功能（2013.11.06）
2. 执行cmd或/bin/sh功能（2013.11.06）
3. 手动设置shell属性功能（包括shellUrl，shellPwd，shellType，shellCoding，shellTimeOut等）（2013.11.06）

fileManager：

1. 刷新功能（2013.11.06）
2. 文件上传功能（包括拖动上传和右键选择上传）（2013.11.06）
3. 文件编辑保存功能（2013.11.06）
4. 文件复制粘贴功能（2013.11.06）
5. 文件（夹）重命名功能（2013.11.06）
6. 文件（夹）修改时间功能（2013.11.07）
7. 新建文件夹功能（2013.11.07）
8. 新建文件功能（2013.11.07）
9. 下载文件到服务器（2013.11.07）