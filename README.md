# XiaomiRouter4-Pandavan

## 测试环境

- Windows11 23H2 专业版
- Python环境 3.11.5
- 小米路由器4（Pandavan固件版本3.4.3.9-099_22-01-4）
- 锐捷客户端V6.85

## 准备工作

- 刷机准备
  - 对应路由器的Breed固件 **[（点此查找Breed固件）](https://breed.hackpascal.net/)**
      ***注意：不同型号的路由器对应的Breed固件不同，切记不要乱刷导致路由器变砖！！！***
  - 对应路由器的Pandavan固件 **[（点此查找Pandavan固件）](https://opt.cn2qq.com/padavan/)**
- 锐捷认证准备
  - 锐捷客户端
  - WinSCP

## 向路由器刷入Breed&Pandavan固件

- 由于大多数博客或者视频网站都有介绍路由器刷Breed&Pandavan的相关教程，这里就不再赘述。（[推荐教程](https://www.bilibili.com/video/BV1wq4y1c7Sc?vd_source=9299b0597ba8d6f604011de5638a2748)）**视频所附文件均已上传GitHub!!!**

## 获取伪装的Mac地址

- 安装锐捷客户端（这里需要记录软件安装路径,比如我的安装路径为`D:\Program Files\Ruijie Networks\Ruijie Supplicant`，如下图所示：）

<center class = 'img'>

<img src = "./PNG/锐捷客户端安装路径.png" width = 90%>

</center>

- 安装WinPcap（`WinPcap 4.1.3.exe`），然后运行抓包工具（`MentoHUST.exe`），将网卡选择为电脑有线网口绑定的网卡，如下图所示：

<center class = 'img'>

<img src = "./PNG/抓包工具配置1.png" width = 90%>

</center>

- 点击开始，手动查找锐捷客户端程序位置（教程所述安装位置为`D:\Program Files\Ruijie Networks\Ruijie Supplicant`），然后登陆我们校园网账号密码进行登录,保存后缀为`mpf`的文件。

<center class = 'img'>

<img src = "./PNG/抓包工具配置2.png" width = 90%>

</center>

- 打开我们的测试软件（`test.exe`），依然将网卡选择为电脑有线网口绑定的网卡；点击设置，填写账号密码，点击+号保存；打开**参数设置**，导入我们所抓的数据包；然后点击确认进行认证；如图：

<center class = 'img'>

<img src = "./PNG/测试软件配置1.png" width = 90%>

</center>

<center class = 'img'>

<img src = "./PNG/测试软件配置2.png" width = 90%>

</center>

<center class = 'img'>

<img src = "./PNG/测试软件配置3.png" width = 90%>

</center>

<center class = 'img'>

<img src = "./PNG/锐捷认证参数输出.png" width = 90%>

</center>

***我们需要保存的是***

## 路由器配置
- 打开浏览器，输入`192.168.1.1`，登录账号：admin，密码：admin，打开**外部网
络**，再打开锐捷认证，填入我们上一步获取到的信息。
- 上传我们的抓包文件

***注意：不同作者编译的Pandavan固件所对应的路由器IP地址和登录后台的管理员账号密码可能不一样，以作者的说明为准***






<center>

**最后，enjoy it😁😁😁**

</center>
