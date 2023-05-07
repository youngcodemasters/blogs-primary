> 推荐几个我在用的Android源码在线阅读网站，方便随时随地学习Android代码。

# [AOSPXRef](http://aospxref.com/)

> 代码比较齐全，由深圳次元空间网络科技有限公司部署服务。

## 用户输入

- Project(s)

​	指定搜索的仓库，select all选择所有的仓库，invert selection对当前选中进行取反操作

- Full Search

​	查找特定的文本片段

- Definition

​	在代码环境中查找类、方法、变量定义

- Symbol

​	在代码环境中查找符号

- File Path

​	指定查找路径特征

- Type

​	指定查找的文件类型

## 测试用例

- 查找短语（phrase）

​	引号包裹，如查找Bill Joy在Full Search中输入"Bill Joy"，查找foo =短语在Full Search中输入"foo ="

- 在指定文件中查找特定内容

​	如查找streace的Android.bp文件，Full Search中输入strace，File Path输入Android.bp

- 查找所有.c文件中的main函数

​	在Symbol中输入main，选择Type为C

- 正则表达式查找

​	文件路径、文件名中包含test开头的，在Fill Path中输入/test[a-zA-Z]+/

- 通配符

​	*，如查找包含interface的路径，在Fill Path中输入\*interface\*

- 包含特定文件但是不包含某个特定文本

​	查找/bin/perl但是不包含/usr/bin/perl的文本，在Full Search中输入-"/usr/bin/perl" +"/bin/perl"，多个过滤字段以空格分隔，且的关系

## 代码阅读

以[strace.c](http://aospxref.com/android-10.0.0_r47/xref/external/strace/strace.c)为例：

当光标放在函数名字上时，按下1显示intelligence window，按下2 3 4高亮，按下5取消所有高亮

# [androidxref](http://androidxref.com/)

> 和[AOSPXRef](http://aospxref.com/)一样，都是opengrok提供服务，操作逻辑基本一致，最新版本为android-9，访问速度不如[AOSPXRef](http://aospxref.com/)，网页响应速度也不如[AOSPXRef](http://aospxref.com/)，可以作为[AOSPXRef](http://aospxref.com/)无服务时的备选方案。

# [ANDROID社区](https://www.androidos.net.cn/sourcecode)

> 最新版本为android-10，可以认为是文件树，查找不是很方便，可以作为备选方案。
