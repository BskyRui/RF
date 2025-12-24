# RF2.2 配置教程



## RF 相关资料

- 官方配置教程  https://www.rotorflight.org/docs

- GUI 配置工具下载地址 https://github.com/rotorflight/rotorflight-configurator/releases/tag/release%2F2.2.1





## RF 软件和固件更新

### 下载软件并安装

1. 以 Windows 为例，这里我选择的是 x86 绿色版

![image-20251221105533656](.\rf\image-20251221105533656.png)



2. 解压后打开 `rotorflight-configurator.exe`

   ![image-20251221105435533](.\rf\image-20251221105435533.png)



3. 打开后会出现一下界面

   ![image-20251221105708443](.\rf\image-20251221105708443.png)



### 连接并更新固件

1. 准备好陀螺仪并连上 USB，以 FlyDangon pro 举例

   ![image-20251221110403380](.\rf\image-20251221110152569.jpg)

2. 安装驱动

   ![image-20251221112723269](.\rf\image-20251221112723269.png)



4. 点击右上角`更新固件`，选择合适的固件版本然后点击`从网络加载固件`

   ![image-20251221111502366](.\rf\image-20251221111502366.png)



5. 烧录固件

   ![image-20251221113041139](.\rf\image-20251221113041139.png)







## RF 飞行参数设置

### 1. 选择接收机连接方式

根据控不同做相应选择，Futaba 为  UART2 - SBUS

![image-20251221124040555](.\rf\image-20251221124040555.png)



### 2. 陀螺仪安装方向

![image-20251221123601918](.\rf\image-20251221123601918.png)





### 3. 选择接收机协议

注意 AUX1,2 所对应的通道，后续会用来切换 Bank 和解锁

![image-20251224205409599](.\rf\image-20251224205409599.png)



### 4. 电机电调设置

**STANDARD**
 通过标准 PID 控制来稳定旋翼转速，类似于大多数 ESC（电子调速器）。所有辅助功能也处于激活状态。

**MODE1**
 与 STANDARD 模式相似，但带有集体/循环预补偿。这与大多数 FBL（飞行控制系统）中的油门调节器类似。



- 电调定速选择：**PASSTHROUGH** 

- 陀螺仪定速选择：**STANDAER**、**MODE1** （推荐）

  



![image-20251221145442163](C:\Users\BskyRui\AppData\Roaming\Typora\typora-user-images\image-20251221145442163.png)





### 5. 设置舵机

频率控制宽频、窄频

![image-20251221114913303](.\rf\image-20251221114913303.png)



### 6. 十字盘、螺距、尾舵相关设置

1. 校准循环螺距，经验值 12

   ![image-20251221125940976](.\rf\image-20251221125940976.png)



2. 校准集体螺距 13°，循环螺距和集体螺距极限以十字盘步干涉为准调到最大值

   ![image-20251221133030753](.\rf\image-20251221133030753.png)



3. 尾巴相关设置

   - 尾舵摇杆向左，滑块向右，如果不是调整 `航向控制方向`

   - 顺时针 45°，加大`航向校准`让尾桨夹角到 45°
   - 逆时针先从较小的值往上调，直到尾滑块到达右侧的最大行程

   ![image-20251221141841877](.\rf\image-20251221141841877.png)



### 7. 速率

根据个人风格，设置横滚、俯仰、航向参数

![image-20251221144232429](.\rf\image-20251221144232429.png)



### 8. 飞行参数

https://www.rotorflight.org/docs/configurator/tabs/profiles



### 9. 飞行参数切换

类似 Mikado 的 Bank1,2；Futaba 的 Idle1,2

![image-20251224204411087](.\rf\image-20251224204411087.png)





### 9. 解锁

![image-20251224203913731](D:\RF\rf\image-20251224203913731.png)







# 参考资料

- https://www.rotorflight.org/docs/controllers/flydragon2.2
- https://www.rotorflight.org/docs/setup/flashing-the-firmware
- [ROTORFLIGHT 2.1教程](https://www.bilibili.com/video/BV1EUkgYuEtS)