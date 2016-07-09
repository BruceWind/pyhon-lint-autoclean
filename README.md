# pyhon-lint-autoclean

android开发中往往由于apk包过大，需要删除一些多余的资源文件，来缩小apk
使用lint工具生成了lint.xml之后， 发现里面的文件太多了，lint并没有提供一次性删除unuse resource的文件。

对于一个个手动操作删除文件的方式，始终觉得太傻逼了。

需要一种自动化方案。
这个python代码，可以用命令，帮助我们一次性删除所有的**unuse resource**。

```
sudo python ./autoclean_resource.py -i ./lint-results.xml  -e ./excep.xml
```
