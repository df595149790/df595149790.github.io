

这几天在尝试 AkShare （ [https://github.com/jindaxiang/akshare](https://github.com/jindaxiang/akshare) )

遇到一个问题

例子中是用 Docker 运行的，但是执行 hist_df.to_csv 时，始终无法在 mac 下找到对应的文件


```
print ( hist_df.to_csv("tmp/x.csv") )
```

猛然想到，docker 的目录需要映射才可以

原始的启动代码如下

```
docker run  -it registry.cn-hangzhou.aliyuncs.com/akshare/akdocker python
```

调整为如下启动代码后，世界恢复了正常

```
docker run --mount type=bind,source=/tmp,target=/tmp -it registry.cn-hangzhou.aliyuncs.com/akshare/akdocker python
```

 

