下载 [nssm-2.24.zip](https://nssm.cc/release/nssm-2.24.zip)

将所需启动的软件注册为windows系统服务
下载解压后找到电脑对应的架构在此处打开命令提示符
键入 `nssm.exe install <服务名>` 

接着会弹出一个GUI框 选中启动程序所在路径
在第三行可以配置启动应用时的启动参数
最后点`install service`完成配置
如没有其他需求其他标签页可以不配置

如需删除服务则执行 `nssm.exe remove <服务名>`即可