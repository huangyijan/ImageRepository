
### 黑苹果折腾心得
----------

先贴一下本人机子的配置：

>* 配置
>* cpu: i5 8400
>* 显卡：技嘉1050ti

剩下的配置其实都不太有关，黑苹果的主要问题在我看来一般都是显示，声音，上网，USB,这四个能驱动基本问题就不大了。
当然我说的是针对台式机来说，如果是笔记本，还有触摸板，电池，睡眠，亮度调节等等各种问题需要解决。建议如果是新人的话，急切想吃一口的话，可以考虑加入自己电脑
品牌的黑苹果群，寻找一样配置或者差不多的EFI(colver)版本代替。往往比自己折腾出来省事很多，甚至一步到位，当然能折腾的例外啦。

#### 1、先截图（zhuangbi）看看



<table>
<tr>
<th ><img src="https://raw.githubusercontent.com/huangyijan/ImageRepository/master/Image/1.jpg" width = "50%" /></th>
<th><img src="https://raw.githubusercontent.com/huangyijan/ImageRepository/master/Image/1.jpg" width = "50%" /></th>
</tr>
<tr>
<th ><img src="https://raw.githubusercontent.com/huangyijan/ImageRepository/master/Image/1.jpg" width = "50%" /></th>
<th><img src="https://raw.githubusercontent.com/huangyijan/ImageRepository/master/Image/1.jpg" width = "50%" /></th>
</tr>
</table>

#### 2、过程

##### 2.1 试装虚拟机VMare mac 12.6

黑苹果的过程比较曲折吧，一开始的时候也没有想转移到mac系统，所以只是在window的VMare虚拟机里面转了一个，问题也并不是很大，
在虚拟机上面装黑苹果的主要问题就是开启VMare的mac系统选项，这里是使用unlock最新版本解决的问题（好像是209来的，很久之前装的，记不太清楚。）,
总体还行，因为在虚拟机里面没有显卡驱动，有些东西打开卡卡的，我给虚拟机分配了8G内存，所以也不怎么卡，估计用来测试软件是没什么问题的。

##### 2.2 真机安装

ps:本人是一个前端，学习有两年了吧，最近团队这边需要学习了解react-native的知识，但说实话本人只是学了mvvc框架里面的vue,angular(稍有涉猎，之前有过做过一个相关的项目，模块化的思想真的很不错)。
但是react还没学过，JSX都甚至不是很熟，我选择从视频来进行避免走些弯路，视频里面老师推荐用mac进行开发，这也是真机安装的契机。以上都是闲言碎语。下面介绍具体过程

一点一点讲吧，真机调试并不是很顺利（下载我就不讲了，如果要资源可以网上找，一大堆，我使用的是在远景论坛版主修改过的版本，如果有需要可以私聊我发给你，安装的是13.4，本人当前的系统是升级后13.5，无痛升级，就换了webdriver最新的版本，其他的都是没有问题的）。

>* 镜像烧录

这里使用的transmac工具，不会使用的可以上B站搜一下黑苹果安装教程前面有一个张云道的人录的，本人也是差不多在那里入门的，烧录就像烧window的镜像，问题不大
[链接]（https://www.bilibili.com/video/av19235761?from=search&seid=14657848923029564329）

>* EFI引导

因为现在流行的黑苹果的安装方式需要EFI来引导四叶草安装，本人的电脑因为一开始是bios引导MBR进入window10系统。这里如果有朋友碰到我的问题，先别急，先用U盘来进行黑苹果系统的引导，问题可以在晚一点解决
