此示例演示了使用profile+resource的方式来满足不同运行环境的差异化配置需求；
此方法适用于不同运行环境的配置差异化比较大，可能包括配置文件数量、配置结构的差异的情况，
此方案的优势在于能最大限度的兼容不同差异，缺点是公共配置配置文件发生变更时需要多处修改；
注意：
1)此方案下基础resources下只能存放无差异性的公共配置文件。
2)resources通过targetPath和${basedir}可以把项目中任意目录的任意文件或文件夹copy到任意目录中；
3)maven的resources拷贝默认是不强制覆盖的，也就是说如果目标路径已经存在同名文件则放弃拷贝，如果要强制覆盖需要如下配置：
<properties> 
        <maven.resources.overwrite>true</maven.resources.overwrite> 
</properties> 

通过命令行指定profile的方法是：-P <profile id>
