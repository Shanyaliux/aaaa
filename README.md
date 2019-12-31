# 使用v2ray实现科学上网


### 首先购买一个海外的VPS

这里我用的是vultr家的vps

[网址在这里](https://www.vultr.com/)

自行注册账号登录

**接下来就是消费了^_^**

1. 充钱先这里

   ![20191231165334.png](https://i.loli.net/2019/12/31/OldnX7ay5RSg3Ck.png)

2. 自行填写相关信息、选择支付方式和金额（可用微信、支付宝）
   ![20191231165504.png](https://i.loli.net/2019/12/31/LFlqVRt1fTiC2Y7.png)

3. 充完后点击红圈中内容去选择你要购买服务器

   ![3.png)](https://i.loli.net/2019/12/31/xzLOH42mTC8eslu.png)

4. 点击加号添加服务器

   ![4.png)](https://i.loli.net/2019/12/31/er3PmX1wMZVRdN4.png)

5. 选择 
   ![20191231165852.png](https://i.loli.net/2019/12/31/pcIbnv2hRsaSXZz.png)
   ![20191231170324.png](https://i.loli.net/2019/12/31/CWQdezGMxfshr4U.png) ​				
   ![20191231170404.png](https://i.loli.net/2019/12/31/xl4RbJtwCuMSNgG.png)

6. 去往服务列表会看到服务器正在安装

   ![3.png)](https://i.loli.net/2019/12/31/xzLOH42mTC8eslu.png)
   ![20191231170618.png](https://i.loli.net/2019/12/31/kNbxhZgUp71i5vo.png)

7. 装完后点击这里会显示出服务器的信息

  ![20191231170704.png](https://i.loli.net/2019/12/31/cI1J8zYwneqx94d.png)
  ![20191231170758.png](https://i.loli.net/2019/12/31/Jp6wNSsGITDV1Y9.png)

### 到这里消费就基本完成了，我们开始配置 v2ray服务端 

1. 百度搜索XShell并下载安装

   [下载网址在这里](https://xshell.en.softonic.com/)

   安装后打开 Xshell 点击这里
   ![20191231171104.png](https://i.loli.net/2019/12/31/ntkaiPghHzBWG8V.png)

2. 会出现这个界面，在主机处输入我们的服务器IP地址
   ![20191231171356.png](https://i.loli.net/2019/12/31/Vub95PA68KyMfED.png)

   **IP地址在这里**
   ![20191231171459.png](https://i.loli.net/2019/12/31/MxzKiIoP3Xb4ULy.png)

3. 接下来远程连接我们的服务器
   ![20191231171651.png](https://i.loli.net/2019/12/31/v9DxnCBU1KSedGr.png)

   出现这个页面点这里
   ![20191231171802.png](https://i.loli.net/2019/12/31/aBqRtGgTFZnpJVc.png)
   之后会让我们输入用户名和密码
   ![20191231171836.png](https://i.loli.net/2019/12/31/xeZGkBVX4NKoAn3.png)


    **在找IP地址的下面找**
    ![20191231171934.png](https://i.loli.net/2019/12/31/9tzU3YE4asVpDdM.png)
    
    出现如下字样代表连接成功
    ![20191231172200.png](https://i.loli.net/2019/12/31/hs3ImKoWGv6abqX.png)

### 开始安装服务端

1. 在XShell 输入 `wget https://install.direct/go.sh`   回车
   ![20191231172421.png](https://i.loli.net/2019/12/31/UcxAPHtrChVvDGN.png)

   ![Snipaste_2019-12-31_17-26-26.png](https://i.loli.net/2019/12/31/B62lQqNUrjaRXML.png)

2. 输入 `sudo bash go.sh`  回车
   ![20191231173730.png](https://i.loli.net/2019/12/31/DzKWNiPjoykeUBd.png)

   安装成功，记住PORT和UUID，后面本地配置需要用。
   ![20191231174020.png](https://i.loli.net/2019/12/31/ZlBuaCd89cAKq4f.png)

3. 服务器启动v2ray 输入 `sudo systemctl start v2ray` 回车
   ![20191231174147.png](https://i.loli.net/2019/12/31/x4vSUohg5actPjD.png) 

### 现在就可以安装客户端使用了

#### [Windows客户端下载](https://github.com/Cenmrev/V2RayW/releases/download/v1.0.0-beta2/V2RayW.zip)

下载后解压打开
![20191231175017.png](https://i.loli.net/2019/12/31/amTJyPiQSBDv3kA.png)
若弹出点是
![20191231175104.png](https://i.loli.net/2019/12/31/Vr6I2g5WhLZjYHv.png)
之后右击托盘图标选择配置点增加
![20191231175327.png](https://i.loli.net/2019/12/31/9UW3mlurRzSZ215.png)
![20191231180053.png](https://i.loli.net/2019/12/31/4CRupVOHh3qL2JQ.png)

填写信息后保存
![20191231180226.png](https://i.loli.net/2019/12/31/u9dHU3SpjAmB87V.png)
右击托盘图标选择自动模式PAC、加载v2ray
![20191231180329.png](https://i.loli.net/2019/12/31/gpBdMfGHIKV4mTr.png)

**OK 你已经可以访问Goolgle、Youtube了**
![20191231180556.png](https://i.loli.net/2019/12/31/JNxZzD3sn2LVI1j.png)


#### [Android客户端下载](https://github.com/2dust/v2rayNG/releases/download/1.1.14/v2rayNG_1.1.14.apk)

配置方法跟电脑大致相同自行配置即可

# 尽情遨游吧
