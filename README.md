# log2falcon

把日志信息采集到falcon的工具

> * 安装依赖:curl -L update.mydan.org|bash
> * 安装log2falcon: cd /opt/mydan && git clone https://github.com/MYDan/log2falcon.git
> * 安装 sudo /opt/mydan/log2falcon/tools/cron --install
> * 添加配置文件到 /opt/mydan/log2falcon/conf/

###配置文件书写规则
> * /opt/mydan/log2falcon/conf/messages 为例子采集/var/log/messages的日志信息
> * 配置文件第一行为要采集的日志的路径,其余的信息为匹配规则或者falcon中的tags
> * 匹配规则 name: matchstring 
> * 特殊name, 如name为count，会覆盖默认的日志行数统计count
> * 特殊name, 如name为tags，为falcon中的tags