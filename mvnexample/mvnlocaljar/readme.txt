该示例项目演示了如何引进本地jar的其中一种方法：
配置本地repository的方式。

同时展示了deploy到远端nexus库的配置方法。用了安全起见，远端nexus库的认证信息不放在pom.xml中，直接配置在
maven的setting.xml中，如：
    <server>
      <id>pubnexus</id>
      <username>admin</username>
      <password>admin123</password>
    </server>
