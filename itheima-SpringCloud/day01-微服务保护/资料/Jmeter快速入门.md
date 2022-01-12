[TOC]

# Jmeter快速入门



# 1.安装Jmeter

Jmeter依赖于JDK，所以必须确保当前计算机上已经安装了JDK，并且配置了环境变量。



## 1.1.下载

可以Apache Jmeter官网下载，地址：http://jmeter.apache.org/download_jmeter.cgi

![image-20210715193149837](https://tva1.sinaimg.cn/large/008i3skNly1gyb8kltl42j30ql0dpdhl.jpg)



当然，我们课前资料也提供了下载好的安装包：

![image-20210715193224094](https://tva1.sinaimg.cn/large/008i3skNly1gyb8kkdlwfj30g609ojsk.jpg)



## 1.2.解压

因为下载的是zip包，解压缩即可使用，目录结构如下：

![image-20210715193334367](https://tva1.sinaimg.cn/large/008i3skNly1gyb8kjex3qj30gh0933yz.jpg)

其中的bin目录就是执行的脚本，其中包含启动脚本：

![image-20210715193414601](https://tva1.sinaimg.cn/large/008i3skNly1gyb8kigtfzj30bf076gly.jpg)

### 1.3.运行

双击即可运行，但是有两点注意：

- 启动速度比较慢，要耐心等待
- 启动后黑窗口不能关闭，否则Jmeter也跟着关闭了

![image-20210715193730096](https://tva1.sinaimg.cn/large/008i3skNly1gyb8khiin1j31660nogox.jpg)



# 2.快速入门



## 2.1.设置中文语言

默认Jmeter的语言是英文，需要设置：

![image-20210715193838719](https://tva1.sinaimg.cn/large/008i3skNly1gyb8kfoelnj30tv0dedi0.jpg)

效果：

![image-20210715193914039](https://tva1.sinaimg.cn/large/008i3skNly1gyb8ke90alj31690m3q61.jpg)



> **注意**：上面的配置只能保证本次运行是中文，如果要永久中文，需要修改Jmeter的配置文件



打开jmeter文件夹，在bin目录中找到 **jmeter.properties**，添加下面配置：

```properties
language=zh_CN
```

![image-20210715194137982](https://tva1.sinaimg.cn/large/008i3skNly1gyb8kds0lij30rv066mym.jpg)



> 注意：前面不要出现#，#代表注释，另外这里是下划线，不是中划线





## 2.2.基本用法

在测试计划上点鼠标右键，选择添加 > 线程（用户） > 线程组：

![image-20210715194413178](https://tva1.sinaimg.cn/large/008i3skNly1gyb8kccxolj30lq0cf76a.jpg)

在新增的线程组中，填写线程信息：

![image-20210715195053807](https://tva1.sinaimg.cn/large/008i3skNly1gyb8kbkppqj30vr0am40i.jpg)



给线程组点鼠标右键，添加http取样器：

![image-20210715195144130](https://tva1.sinaimg.cn/large/008i3skNly1gyb8kah2okj30o308rgnj.jpg)



编写取样器内容：

![image-20210715195410764](https://tva1.sinaimg.cn/large/008i3skNly1gyb8k9kbhrj314s0dxgop.jpg)



添加监听报告：

![image-20210715195844978](https://tva1.sinaimg.cn/large/008i3skNly1gyb8k84xr1j30mk0cm76s.jpg)

添加监听结果树：

![image-20210715200155537](https://tva1.sinaimg.cn/large/008i3skNly1gyb8k7p9ogj30ll0cgjtt.jpg)



汇总报告结果：

![image-20210715200243194](https://tva1.sinaimg.cn/large/008i3skNly1gyb8k6ah8dj30sy036gm3.jpg)

结果树：

![image-20210715200336526](https://tva1.sinaimg.cn/large/008i3skNly1gyb8k5uostj30oz0hl0uu.jpg)

