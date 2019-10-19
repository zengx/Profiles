库位置：https://github.com/limbopro/Profiles/tree/master/limbopro/Gift

## 主理人说
### 20.10.2019 更新

**教程步骤虽多，但足够清晰**

本配置文件，相当于提前为Quantumult`预设策略`（10个策略）及其`策略图标`，`去广告规则`，`主流站点`分流规则，以及无需拔卡看，`Tiktok`，解锁`VSCO`会员；可自用，下载即可使用，各个`策略`下的节点，自己配置自己配置即可（务必删除所有无用节点）；

如下图；

![QX.jpg][1]

## 注意注意
*可备份配置文件，以防止后悔；

1. 进入`QuantumultX`，点击右下角`三菱`按钮；
2. 找到`配置文件`模块下`导出`，点击，选择`存储到文件`；
3. 备份完毕；

## 本配置文件使用方法
### 1.备份你的订阅链接
1. 进入`QuantumultX`，点击右下角`三菱`按钮；
2. 找到`配置文件`模块下`编辑`，点击；
3. 找到`[server-remote]`，下方就是你已经配置好的节点订阅链接；
4. 复制，留作备用（不然等下又要一个个添加（如果持有机场多的话））；

### 2.下载预设配置文件
0. 复制`https://raw.githubusercontent.com/limbopro/Profiles/master/limbopro/Gift/QuantumultX4limbopro.conf`；
1. 进入`QuantumultX`，点击右下角`三菱`按钮；
2. 找到`配置文件`模块下`下载`，点击；
3. 粘贴刚刚复制的配置链接，点击右上角`确定`按钮；
4. 保存完毕，进入`QuantumultX`主界面，就可以看到配置好的10个`策略`图标了；

### 3.删除无用节点，配置你的节点
1. 复制之前备份的`机场订阅`粘贴到`[server-remote]`后或从`节点`->`订阅/引用`处添加订阅；
2. 例如当你试图开启 QuantumultX 的时候，界面提示`未知策略或节点`... 找到对应`名字`的`策略`图标（例如Twitter）；
3. 长按 `策略`图标，然后弹出选择框，请删掉下面带`感叹号`的`节点`，并添加你的节点；

### 4.重新配置证书以使得Tiktok/去广告实现
1. 如果之前有配置证书，可进入 iOS 系统`设置`-` 通用`-`描述文件`-`已下载的描述文件`-选中，`移除描述文件`，输入密码...完成描述文件安装；
2. 进入QuantumultX，点击页面右下角三菱`按钮`，找到`MinM`模块，点击`生成证书`，提示生成成功，点击`安装证书`此时会跳转至` Safari`，提示`此网站...下载一个配置描述文件。您要允许吗？`，点击`允许`，网页提示`已下载描述文件`；
3. 进入 iOS 系统`设置`-` 通用`-`描述文件`-`已下载的描述文件`-选中，并安装，输入密码...完成描述文件安装；
4. 进入 iOS 系统`设置`-` 通用`-`关于本机`-`证书信任设置`-`针对根证书启用完全信任`-选中刚刚安装的并启用即可；

### 5.Enjoy

1. 进入`QuantumultX`，开启`Rewrite` & `MitM`，开启 QuantumultX；
2. 完事！

### 6.试玩配置文件修改策略模式
1. 进入`QuantumultX`，点击右下角`三菱`按钮；
2. 找到`配置文件`模块下`编辑`，点击；
3. 可以修改各个`策略`的`策略模式`；# available 为健康检查模式，round-robin 为负载均衡模式，static 为静态策略模式，可以通过把 available 改为 static 的方式以切换至静态策略模式，其他同理；

### 小技巧
#### 查看网络活动
**网络连不上？Twitter打不开？ins加载慢？**

1. 进入`QuantumultX`，找到`网络活动`模块（长得像记事本那个）；
2. 你就可以知道，最近打开某个APP例如ins/Twitter/在走哪个分流规则/走哪个策略了/哪个节点了，是直连还是代理还是拒绝连接服务器；
3. 日志可以详细到时间/节点/策略/；
4. 相应调整节点/策略/即可

## FAQ
### 如何删除无用策略组
1. 进入`QuantumultX`，点击右下角`三菱`按钮；
2. 找到`配置文件`模块下`编辑`，点击；
3. 找到`[policy]`，找到要删除的`策略`，删除即可；
4. 玩法参考：QuantumultX 进阶教程：[组策略&分流规则&自定义图标的进阶玩法](https://limbopro.xyz/archives/3846.html)  

### 关于名叫CN策略
1. 进入`QuantumultX`，可以看到一个中国地图样式的策略，CN；
2. 该策略没有绑定分流规则；
3. 如果你在国内，可以任意在该策略下添加节点；
4. 本意是留作出国时用回国节点的；
5. 如果你在国外，可在分流模块订阅/订阅`https://raw.githubusercontent.com/limbopro/Profiles/master/Quantumult/BacktoCN.conf`；
6. 策略偏好选择`CN`即可；

### 是否还会更新
会的，或增加策略（概率很小），优化分流规则（只需更新分流订阅即可），~~优化图标~~；正常情况下，我个人认为，10个策略基本上已经足够；

### 想自定义图标或策略或新加去广告规则？
参考：https://t.me/limboprossr/843

## 鸣谢
NobyDa https://github.com/NobyDa/Script 脚本及去广告支持

ConnersHua https://github.com/ConnersHua/Profiles 主流网站分流规则支持

## 联系主理人

1. 关注频道 https://t.me/limboprossr 不失联；
2. `毒奶粉`们（我管我的Fans）可联系 [TG机器人](https://limbopro.xyz/usr/uploads/2019/10/3453243330.png) 或发送 [邮件](https://limbopro.xyz/usr/uploads/2019/10/3453243330.png) 获取帮助；

  [1]: https://raw.githubusercontent.com/limbopro/Profiles/master/limbopro/Gift/QX.jpg
