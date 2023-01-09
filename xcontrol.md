### 开发环境  
Visual Studio 2022

### 单文件打包命令  
dotnet publish -c Release -r win-x64  -p:PublishSingleFile=true --self-contained true /p:IncludeNativeLibrariesForSelfExtract=true /p:DebugType=None

### 开发板说明
1、每块开发板有一个服务器核心+若干个安卓系统核心  

2、开发板自带一个内部交换机，靠近USB口的网口为服务器核心专用网口，其他网口为安卓系统核心用网口。如果需要将服务器和安卓系统的网络隔离开，则需要两根网线分别连接到路由器或者交换机上。如果使用同一个网络则只需要一根网线接安卓系统网口和路由器或交换机，另一根短网线接服务器核心网口和任意一个安装系统网口即可。  

### 使用教程

#### 1、开发板连接电源，按照下图示意连接开发板网络（共用网络） 

![image](https://user-images.githubusercontent.com/24860541/201560542-6b58b5b7-527f-4823-9d26-43faf98321e9.png)
  
  
  
#### 2、连接完成后，下载最新XControl客户端，点击主界面左侧菜单“节点”，然后点击顶部“扫描节点”即可找到开发板并连接。 

![image](https://user-images.githubusercontent.com/24860541/201561697-2d864c2a-ebee-4591-b302-ff228d20ab8a.png)

> 注意：控制电脑必须和开发板服务器核心在同一个网络环境，若网段不是常用的192.168.1则需要登录路由器或在当前电脑的网络设置中查看，找到当前网段回到主界面修改扫码IP段然后再次扫描节点直到发现节点为止。  
  
  
  
#### 3、连接节点，点击左侧菜单“设备”，即可看到所有安卓核心，点击设备即可进行控制。  

![image](https://user-images.githubusercontent.com/24860541/201562441-0d1d754a-e61d-47fe-ad82-1a76c4efcd5c.png)
