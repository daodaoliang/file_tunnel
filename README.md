README.妈蛋
=============================================
file_tunnel
顾名思义：文件传输隧道
1.通过配置,可以方便的把一台机器一个目录下的指定模式的文件自动同步到另一台机器的指定目录下(rsync实现的) ,机器之间不需要打通信任关系(当然，打通了更好) ,一个文件同步到目标文件夹完成后该文件会自动按小时备份到源文件夹下的.bak 文件夹中并从源文件夹中删除.(注意自己定时清理备份文件夹)
2.目前支持一对一/一对多/多对一,并可自动监测机器宕机,在主备模式下主机宕机后会把文件自动同步到备机上
3.特别适合大批量文件的自动同步
4.理论支持无线多组推送隧道
5.高级功能：
    把n台机器上的日志自动拉取到本地机器上,并按照本地磁盘容量/磁盘数目分类按天散列到n(n>2)块磁盘上
    所有散列后的文件会通过软链的方式在你指定的view_disk 下建立统一视图，方便你按天对日志进行统计

