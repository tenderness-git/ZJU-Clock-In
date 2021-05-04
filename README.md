# 自动打卡教程

 **如果看不到本文的图片，就查看仓库内的pdf文件**
 如果这个脚本帮到了你，请给我一颗star 哈哈。

首先你需要拥有一个github，直接在左上角注册就行了。

### Step1. Fork本仓库

点击本仓库的Fork

![image-20210504141421350](https://tva1.sinaimg.cn/large/008i3skNly1gq6dacfvdjj31yy0u07ed.jpg)

Fork的含义是将本仓库拷贝一份，放到你自己的github账号下，所以只有在第一次观看本教程的时候才需要fork。

然后我们可以看到，左上角这里的Di-Zhipeng已经变成了你自己账号的名字，下面标注着forked from Di-Zhipeng/ZJU-Clock-In.

![image-20210504141632691](https://tva1.sinaimg.cn/large/008i3skNly1gq6dcl2073j31h90o8jv2.jpg)

此时你已经拥有了本仓库的一个拷贝。

### Step2. 添加账户密码

点击仓库的右上角的Settings：

![image-20210504141844386](https://tva1.sinaimg.cn/large/008i3skNly1gq6deuzmfvj31vo0mcdkc.jpg)

点击下面的Secret

![image-20210504141905641](https://tva1.sinaimg.cn/large/008i3skNly1gq6df8l52dj31l90u045g.jpg)

点击New repository，添加一个Secret

![image-20210504142045807](https://tva1.sinaimg.cn/large/008i3skNly1gq6dgz81vpj31n00pwmz0.jpg)

Name必须为ACCOUNT，Value填入自己的浙大通行证账号。然后仿照上面的操作，再添加一个Name为PASSWORD，Value为浙大通行证密码的Secret，自动打卡脚本就配置完成了。

效果和下面的差不多：

![image-20210504142239194](https://tva1.sinaimg.cn/large/008i3skNly1gq6diybkrfj31l10u0wjv.jpg)

### Step3. 如何触发打卡？

有两种方式，第一种是在自己的ZJU-Clock-In仓库里点击Star（已经Star的就取消Star，再重新点击）。

第二种是等待12小时，这个脚本是每隔12小时触发一次的。

### Step4. 如何判断打卡是否成功？

点击仓库的Action：

![image-20210504142536391](https://tva1.sinaimg.cn/large/008i3skNly1gq6dm0ix9vj327o0twteb.jpg)

每次触发打卡就会在右边多出一个记录，比如现在我已经执行过四次打卡脚本了，点击你需要查看的记录，再点击里面的ClockIn按钮，我们就可以看到本次打卡的情况了：

![image-20210504142743921](https://tva1.sinaimg.cn/large/008i3skNly1gq6do8552sj32r80r8wi9.jpg)

非计算机科学的学生只需要关注右侧ClockIn的文字提示内容就行了，点击Clock In：

![image-20210504142839755](https://tva1.sinaimg.cn/large/008i3skNly1gq6dp77angj320v0u079c.jpg)

就可以看到提示信息了，如果打卡失败，就按照提示去操作就好了。

## Q&A

### Q: 这个脚本安全么？

这个脚本是开源的，大家可以自由观看它的代码，内容很简单，没有任何窃取个人信息的操作

我们的账户密码是放入github的secret中的，只有仓库的所有者才能看到你设置的ACCOUNT和PASSWORD。

这个项目的所有者虽然是我，但你是先Fork再操作的，此时Fork得到的仓库所有者是你自己，我们所有的操作都是在Fork后进行的，我是没有办法看到你的secret的。

所以只要保证你自己的github账号密码不泄漏，浙大通行证的密码就是安全的。

