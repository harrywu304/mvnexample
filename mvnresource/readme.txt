该示例演示了如何使用maven resource特性来操控项目资源的拷贝；

注意：
maven的resources拷贝默认是不强制覆盖的，也就是说如果目标路径已经存在同名文件则放弃拷贝。
如果要强制覆盖需要如下配置：
<properties> 
        <maven.resources.overwrite>true</maven.resources.overwrite> 
</properties> 
