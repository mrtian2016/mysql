# RDS与自建数据库对比优势 {#concept_u4w_sy5_tdb .concept}

## 特性对比 {#section_ukk_wy5_tdb .section}

|对比项|云数据库RDS|自购服务器搭建数据库服务|
|---|-------|------------|
|服务可用性|99.95%|需自行保障，自行搭建主备复制，自建RAID等。|
|数据可靠性|99.9999%|需自行保障，自行搭建主备复制，自建RAID等。|
|系统安全性|防DDoS攻击，流量清洗；及时修复各种数据库安全漏洞。|自行部署，价格高昂；自行修复数据库安全漏洞。|
|数据库备份|自动备份。|自行实现，但需要寻找备份存放空间以及定期验证备份是否可恢复。|
|软硬件投入|无软硬件投入，按需付费。|数据库服务器成本相对较高，对于SQL Server还需支付许可证费用。|
|系统托管|无托管费用。|每台2U服务器每年超过5000元（如果需要主备，两台服务器需超过10000元/年）。|
|维护成本|无需运维。|需招聘专职DBA来维护，花费大量人力成本。|
|部署扩容|即时开通，快速部署，弹性扩容。|需硬件采购、机房托管、机器部署等工作，周期较长。|
|资源利用率|按实际结算，100%利用率。|由于业务有高峰期和低峰期，资源利用率很低。|

## 价格对比 {#section_kkj_t1v_tdb .section}

|费用|云数据库RDS|自购服务器搭建数据库服务|
|--|-------|------------|
|硬件费用和备品配件费用|RDS实例的费用。例如，内存1200 MB、存储空间50 GB（IOPS能力可达到600）的实例费用是2040元/年。| -   至少需要2台数据库服务器。每台IOPS能力达到600的服务器费用大约是6000元。
-   1台用于连接前端Web服务器的内网交换机（便宜的1U非网管交换机为1000元左右）。
-   后期硬件损坏和更换至少还要消耗30%费用。
-   硬件花费：（6000 × 2 + 1000）× 130% = 16900元。

每年费用：16900元/3 = 5633元（硬件按照3年折旧计算）。


 |
|机房托管费用|服务商负责，无需付费。|1U机柜空间托管费用为3000元/年，共有2台1U服务器和1台1U内网交换机需要计费，机房托管费用：3000 × 3 = 9000元|
|带宽费用| -   同一地域内，ECS和RDS可以通过内网互通，且不收取费用。
-   若在不同地域，ECS和RDS可以通过外网互通，需收取外网流量费用，详细收费标准请参见[云数据库RDS详细价格信息](https://www.alibabacloud.com/zh/product/apsaradb-for-rds?spm=a2c63.o282931.a3.1.11fb6ddbLf1nuC#pricing)。

 |只用于内网，不产生公网费用。|
|数据库运维工程师费用|数据库维护由服务商负责，无人员成本。|1个初级DBA工程师月薪至少5000/月，假设当前项目占用该工程师30%的工作量，则人员成本为5000 × 12× 30% = 18000元。|
|每年总费用|2040元/年。|32633元/年。|

**相关主题**

-   [便宜易用](intl.zh-CN/产品简介/产品优势/便宜易用.md#)
-   [高性能](intl.zh-CN/产品简介/产品优势/高性能.md#)
-   [高安全性](intl.zh-CN/产品简介/产品优势/高安全性.md#)
-   [高可靠性](intl.zh-CN/产品简介/产品优势/高可靠性.md#)

