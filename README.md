#  ***关于Weihoo DB Expert***

- 高效运维数据库需要什么？
- 一个数据库监控维护平台？
- 一个数据库自动化巡检工具？
- 最好再有一个SQL智能优化软件？
- 你只需要一个数据库管理专家

![](https://i.loli.net/2018/06/02/5b117c3b7e813.jpg)
![目的图.PNG](https://i.loli.net/2018/06/06/5b17f7ec4f552.png)





## 产品概述

#### 主要功能
                
#### 1. 数据库性能监控
![整体信息.PNG](https://i.loli.net/2018/06/02/5b117f554535e.png)
![性能概况.PNG](https://i.loli.net/2018/06/02/5b117f7a22f80.png)
   weihooDB Expert可通过集中式的管理方式，无需安装代理，便能够实现数据库软件的整体评估，可快速实现数据库性能评估分析、隐患问题发现及诊断、数据库参数标准化配置、数据库容量趋势分析及数据库事件告警等数据库日常维护管理。实现从数据库事件、性能及隐患发现、参数统一管理、快速定位问题根源等应急事件管理，到问题处理建议及性能优化建议等全程数据库智能分析及全生命周期性能故障管理需求。并可自主设置时间段，生成数据库性能管理报表，便于查看及审计。
   
#### 2. 数据库隐患巡检
  ![数据库扫描仪.PNG](https://i.loli.net/2018/06/02/5b1180a78f9e5.png)
  数据库扫描仪采用代理是数据获取方式，旨在通过扫描报告，直观比对性能变化。可支持对不同操作系统（Linux、AIX、Windows）下的数据库进行扫描。
  
#### 3. SQL风险评估
![SQL智能优化.PNG](https://i.loli.net/2018/06/02/5b1181e1c49fd.png)
Weihoo DB Expert可通过数据库中缓冲池、磁盘、排序等各个模块中所消耗的时间分布、发现存在性能问题的SQL语句，对调用SQL的应用程序指标检测及执行计划分析等多种方法逐层追溯导致性能问题的根源，并给出相应优化建议。还定期对数据库中的相关统计信息，数据库表中的行溢出、页重组、索引分裂等信息快速检索，直接定位引起性能问题的相关对象，便于对问题隐患进行根治并进行相应的运维策略设计。




## 产品部署
#### 1.部署手册
[点击查看部署手册](https://github.com/51weihoo/weihoo-DB-Expert/blob/master/%E9%83%A8%E7%BD%B2%E6%89%8B%E5%86%8Cv0.3.md)
#### 2.体系结构介绍
![体系结构.PNG](https://i.loli.net/2018/06/06/5b17904d3f953.png)
在部署完成后，即可使用Weihoo DB Expert的数据库监控、巡检及SQL审核功能了。添加受控端的资源后（信息包括IP、登陆方式、数据库实例名称、端口、用户名、密码等），进入各功能模块后，关联已添加资源即可，需保证受控端主机与server端网络互通。

用户除了可使用Weihoo DB Expert自带的相关阈值及规则设置外，还可根据自身需求，调整监控阈值；设置巡检规则；以及根据不同的数据库类型，设置对应的SQL巡检规则。

## 产品使用说明
#### 文档链接
[点击查看Weihoo DB Expert使用说明](https://github.com/51weihoo/weihoo-DB-Expert/blob/master/Operating%20instructions.md)

## 联系方式
邮箱：<weihoo_db_expert@51weihoo.com>
#### 交流QQ群
![WeihooDB Expert 交流群群二维码.png](https://i.loli.net/2018/06/26/5b31ba44d740b.png)

## 版本更新 V1.0.1 2018-07-11
1. 修改动态SQL语句、表读写情况及锁数量，显示的单位是MB的错误
2. 生成报告中，增加“索引建议”
3. 导出报告中，删除顶端按钮
4. 选择规则中，修复存在重复规则

## 版本更新 V1.0.1 WEB 2018-07-12
1. 修正.恢复数据缓存文件存储方式为:不使用多级目录
2. 修正.资源管理功能，当无分组时资源页面无法显示问题
3. 新增.SQL风险评估规则，增加“最大索引列数”检查项/字段
## 版本更新 V1.0.1 WEB 2018-07-16
1. 修正.监控功能,点击事件“查看”按钮显示undefined问题
## 版本更新 V1.0.2 WEB 2018-07-17
1. 新增.监控功能,性能页面增加表格数据的实时刷新功能
2. 优化.需要使用缓存的监控项统一配置(部分实现)

## 版本更新 V1.0.2 2018-07-17
1. 修正.无法删除zabbix中mysql相关的主机，zabbix模板更新
2. 修正.“Oracle数据库未开启归档日志”每分钟都会重复生成事件，zabbix模板更新
3. 修正.weihuInstall.sh中，import template xml失败，增加验证及更详细日志输出
4. 修正db2 for v95 巡检脚本 捕获top10 sql异常，用ucase函数替代upper

## 版本更新 V1.0.2 WEB 2018-07-18
1. 优化.监控Oracle页面基本信息内容
2. 优化.巡检报告导出文件名规范
3. 修正.巡检/审核修改关联属性页面无法显示资源信息
4. 修正.巡检/审核已禁用资源仍可点击上传文件/静态SQL审核按钮
5. 优化.巡检报表结果显示

## 版本更新 V1.0.2 WEB 2018-07-20
1. 修正.监控Oracle性能部分趋势图不显示问题
2. 修正.监控性能表部分值显示为undefined问题
3. 修正.监控 事件详细信息无法正常显示标注问题/图刻度单位问题
4. 修正.监控性能表部分session无法正常DataTable解析问题
5. 修正.监控 评分为0问题
