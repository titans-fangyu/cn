# 版本说明


## 2021年Q3

| 动态名称 | 动态描述  | 发布时间	  | 相关文档   |
|   :---  |  :---   |  :---  |:---  |
|   提供failover主从切换监控和通知	|   4.0提供了主从节点的异常监控，并可以在监控报警中，配置failover通知。	|   2021-07	|  [节点异常监控](../Operation-Guide/Monitoring/Node-Notice.md)  |  
|   提高故障切换速度	|   代理和master节点同时故障时，优先拉起代理节点，更快恢复流量。	|   2021-07  |   -   |   


## 2021年Q2
| 动态名称 | 动态描述  | 发布时间	  | 相关文档   |
|   :---  |  :---   |  :---  |:---  |
|   创建时增加规格预览	|   创建时增加规格预览,方便用户查看所选实例的分片、容量、节点个数、所需ip等信息。	|   2021-06	|  [创建实例](../Getting-Started/Create-Instance.md)  |   
|   批量导出实例列表	|   支持全量、按找分页的方式，批量导出实例列表。  |   	2021-05	|  [批量导出实例列表](../Operation-Guide/Instance-Management/Export-Instance.md)   |   
|   pipeline使用事务	|   代理支持在pipeline中使用事务相关命令。	|   2021-05 |  -    |   
|   代理性能优化	|   避免在极端情况下代理程序内存使用率高的问题。	|   2021-05  |  -    |    
|   优化设置实例密码	|   已设置免密码登录的实例，可在集群详情页，修改密码和免密模式。  |   	2021-04	|  [修改密码](../Operation-Guide/Instance-Management/Change-Password.md)   |   
|   增加监控指标	|   分类改为：实例监控、代理节点监控、Redis数据节点监控。每类监控下的指标按照CPU、内存、网络、请求、响应进行了分类并进行了指标补充。 	|   2021-04	|   [实例监控](../Operation-Guide/Monitoring/Monitoring.md)    |   

## 2021年Q1
| 动态名称 | 动态描述  | 发布时间	  | 相关文档   |
|   :---  |  :---   |  :---  |:---  |
|   集群实例开放支持2分片 | Redis4.0集群实例新增支持2分片。  | 2021-03	|  -   |   
|   变配进度可查询	|   在用户操作变配时，实例列表页将展示变配进度、耗时等进度信息。 	|   2021-03	|  [实例变配进度可查询](../Operation-Guide/Instance-Management/Change-Configuration.md)  | 
|   提高故障切换速度	|   故障切换时间降低到最多100秒。 	|   2021-03     |  -    |   
|   增加通过URL检索实例	|   列表页新增支持通过实例链接URL地址搜索实例信息。 |   	2021-02	|  -    |   
|   增加监控指标	|   增加带过期时间的key监控。 		|   2021-01	|  [实例监控](../Operation-Guide/Monitoring/Monitoring.md)    |   



## 2020年Q4
| 动态名称 | 动态描述  | 发布时间	  | 相关文档   |
|   :---  |  :---   |  :---  |:---  |
|   集群版4.0支持128分片	|   集群版4.0，新增支持 128 分片。 		|   2020-12	|  -   |   
|   支持ipv6  |   	集群版4.0支持ipv6。 		|   2020-11 | - |   
|   监控指标优化  |   	监控指标增加聚合方式包含avg，max，min等，方便客户分析监控情况。 		|   2020-11	|  -  |   
|   集群版4.0支持128分片+4096G  |   	集群版4.0，新增支持4096G 、128分片。 	|   	2020-10	|    -  |   
|   查看客户端 IP 列表	  |   提供查看Redis实例上的连接统计功能。可以查看动态的,也可以查看一段时间的连接情况、某个ip一段时间的连接日志。   |     2020-10	|    [查看客户端IP列表](../Operation-Guide/Instance-Management/ClientIPList.md)  


## 2020年Q3
| 动态名称 | 动态描述  | 发布时间	  | 相关文档   |
|   :---  |  :---   |  :---  |:---  |
|   调整命令支持的图表	|   增加2.8/4/0支持命令、不支持的命令集合。	|   2020-09	|    [Redis命令支持](../Getting-Started/Command-Supported.md)	| 
|   支持自定义分片  |   	对于集群版4.0的产品，在创建资源/变更配置时，支持用户自定义分片数量。	|   2020-09	|   [创建实例](../Getting-Started/Create-Instance.md)  |   
|   增加性能测试手册和测试结果	  |  性能测试手册和测试结果。 		  |  2020-08  |  	 [性能测试](../Performance-Test/Test-environment.md)  |  
|   Redis 2.8 产品暂停支持	|   基于目前架构和资源情况，Redis2.8产品计划未来不再提供支持。如的确有需要使用，请联系客服。 |   2020-08	|   -   | 

## 2020年Q2
| 动态名称 | 动态描述  | 发布时间	  | 相关文档   |
|   :---  |  :---   |  :---  |:---  |
|   支持大Key热Key分析	|  帮助用户对实例的大Key和热Key分析统计，并优化性能。	|   2020-06	|    [大Key热Key分析](../Operation-Guide/Cache-Analysis/Key-Analysis.md)	| 
|   支持缓存分析	|  帮助用户对实例进行访问分析，用户可根据分析结果进行性能调优。	|   2020-04	|    [缓存分析](../Operation-Guide/Cache-Analysis/Cache-Analysis.md)	| 

## 2020年Q1
| 动态名称 | 动态描述  | 发布时间	  | 相关文档   |
|   :---  |  :---   |  :---  |:---  |
|   支持慢日志查询	|  通过慢日志查询功能，用户可查找性能变慢原因，并优化性能。	|   2020-03	|    [慢日志查询](../Operation-Guide/Cache-Analysis/SlowLog.md)	| 
|   开放参数修改	|  帮助用户对当前Redis实例的参数进行配置调优。	|   2020-01	|    [参数修改](../Operation-Guide/Instance-Management/Modify-Instancename.md)	| 


## 2019年及之前
| 动态名称 | 动态描述  | 发布时间	  | 相关文档   |
|   :---  |  :---   |  :---  |:---  |
|   开放scan命令 |   开放scan命令，各版本的命令支持情况请参考Redis命令支持页。 		|   2019-11	|     [Redis命令支持](../Getting-Started/Command-Supported.md)    |   
|   支持事务	|   支持事务，但禁用命令不能放在事务中执行。|   	2019-10	|   -   |   
|   新增备份恢复	|      新增备份恢复、访问控制等功能。  |   2019-09	|     [备份恢复](../Operation-Guide/Backup-And-Recovery.md)    |   
|   新增4.0版本	|      redis 4.0版 正式上线。 	  |   2019-08	|   -   |   
|   支持命令		|  redis 2.8版 丰富监控项，新增Keys、String、Hashes、Lists、Sets、Zset监控组。	|   2019-07	 |   [Redis命令支持](../Getting-Started/Command-Supported.md) |   
|   上线公测|   	redis 4.0版  开放公测。 	|   	2019-01 |  -    |   
|   新增Web Cli	|   控制台新增Web Cli工具，方便用户在线使用数据库。 		|   2018-11	|      [使用 Web Cli 连接实例](../Getting-Started/Connect-Instances.md)     |   
|   Redis2.8公测上线|   	Redis2.8公测上线。 	 |   	2017-04	|  - |   


