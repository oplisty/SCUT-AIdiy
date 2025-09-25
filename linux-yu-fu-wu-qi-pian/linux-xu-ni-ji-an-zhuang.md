# Linux虚拟机安装

**1 下载ubuntu的iso文件**
* https://releases.ubuntu.com/22.04.4/
电脑是amd64架构的，下载以下这个

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image1.png" alt=""><figcaption></figcaption></figure>

**2 安装VirtualBox**

* <https://www.virtualbox.org/wiki/Downloads>
选择合适的版本

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image2.png" alt=""><figcaption></figcaption></figure>

* 选好安装的位置，之后一直下一步就行

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image3.png" alt=""><figcaption></figcaption></figure>

* 点击新建

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image4.png" alt=""><figcaption></figcaption></figure>

* ISO Image中选择Ubuntu的iso文件，设置虚拟机名称、存储路径，取消勾选自动安装

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image5.png" alt=""><figcaption></figcaption></figure>

* 按需要设置内存、CPU核数、硬盘大小

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image6.png" alt=""><figcaption></figcaption></figure>

* 确认一下信息

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image7.png" alt=""><figcaption></figcaption></figure>

* 双击打开虚拟机，进入Ubuntu安装

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image8.png" alt=""><figcaption></figcaption></figure>

**3 安装Ubuntu**

* 选择Try or Install Ubuntu，按enter

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image9.png" alt=""><figcaption></figcaption></figure>

* 下划选择中文（简体），安装Ubuntu

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image10.png" alt=""><figcaption></figcaption></figure>

* 键盘布局，选择Chinese，Chinese-Hanyu Pinyin（with AltGr dead keys）

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image11.png" alt=""><figcaption></figcaption></figure>

* 选择网络（安装过程中不要断网）

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image12.png" alt=""><figcaption></figcaption></figure>

* 如果找不到“继续”，按Alt+F7后移动鼠标，拖动页面

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image13.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image14.png" alt=""><figcaption></figcaption></figure>

* 选择正常安装，其他选项都勾选上

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image15.png" alt=""><figcaption></figcaption></figure>

* 安装类型选择其他选择

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image16.png" alt=""><figcaption></figcaption></figure>

* 双击设备，创建新的空分区表

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image38.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image39.png" alt=""><figcaption></figcaption></figure>

* 点击空闲，“+”号，创建第一个分区，大小500MB，用于EFI系统分区

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image17.png" alt=""><figcaption></figcaption></figure>

* 创建第二个分区，大小为（内存\*1000）MB，用于交换空间

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image18.png" alt=""><figcaption></figcaption></figure>

* 创建第三个分区，大小为你的ubuntu系统总空间的四分之一存储
（G到MB换算乘1000），用于Ext4 日志文件系统，挂载点：/

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image19.png" alt=""><figcaption></figcaption></figure>

* 创建第四个分区，大小为剩余所有空间，用于Ext4 日志文件系统，挂载点：/home

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image20.png" alt=""><figcaption></figcaption></figure>

* 找到efi分区对应的编号，在安装启动引导器的设备中选择它

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image21.png" alt=""><figcaption></figcaption></figure>

* 继续，确定一下四个分区是否正确

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image22.png" alt=""><figcaption></figcaption></figure>

* 地区填Guangzhou

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image23.png" alt=""><figcaption></figcaption></figure>

* 设置一下账号密码

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image24.png" alt=""><figcaption></figcaption></figure>

* 等待

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image25.png" alt=""><figcaption></figcaption></figure>

* 安转完毕，点击现在重启

<figure><img src="../.gitbook/assets/Linux虚拟机安装picture/image26.png" alt=""><figcaption></figcaption></figure>