# 备份策略
云数据库 MariaDB 实例自动备份会有一个默认触发时间，并且支持自定义这个触发时间点。

## 注意事项
* 请确保在业务低峰期进行自动备份。
* 自动备份：每天备份，备份保留7天。

## 修改备份策略
1. 登录 [云数据库 RDS 控制台](https://rds-console.jdcloud.com/database)。
2. 选择需要进行设置自动备份策略的目标实例，点击目标实例的名称，进入到实例详情页。
3. 选择 **备份管理** 标签，点击 **备份策略** 标签进入实例备份策略的详情页，点击 **修改策略** 按钮，修改备份策略弹出框参数说明如下：
    * 自动备份时间：选择你需要进行自动备份的时间段，系统自动会在这个时间段内的任意时间点开始执行备份操作；由于备份的时间会根据实例的数据量的增加而增加，所以不确保在指定时间段内可以完成备份操作。
    * Binlog本地保留时长：输入binlog在本地的保留时长，支持的时长范围在1-168小时；超过指定时长的Binlog将被自动清理；
    * Binlog本地空间占用率上限：输入binlog本地空间占用率的上限，支持的范围时1-50；设置后binlog在本地占用的空间百分比不超过指定值；
    * 点击 **确认** 按钮，完成备份策略的修改。
    * 点击 **取消** 按钮，放弃备份策略的修改。
    
    ![备份策略](../../../../../../image/RDS/Create-Backup-policy.png)

4. 点击 **确定** 按钮，返回到备份策略详情页。
