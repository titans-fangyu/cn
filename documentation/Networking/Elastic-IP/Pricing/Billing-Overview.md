# 计费概述

京东云弹性公网IP支持独立计费和续费，本文将介绍弹性公网IP的计费项、计费类型。


### 计费类型

公网IP支持包年包月、按配置和按用量计费，标准公网IP和边缘公网IP分别支持计费类型不同。具体信息如下表：

|计费模式|标准公网IP|边缘公网IP|计量方式|计费项|付费周期|计费类型转换|  
|--- |-- |-- |---|---|----|---|
|包年包月|√|√|按固定带宽计费|带宽费|预付费，每月出一次账单|--|
|按配置|√|√|按固定带宽计费|带宽费|后付费，每小时出一次账单|转包年包月|
|按用量|√|--|按使用流量计费|流量费+IP保有费|后付费，每天出一次账单|转包年包月|

>下表中“√”代表支持，“--”代表不支持。

## 相关参考

- [产品概述](../Introduction/Product-Overview.md)
- [创建公网IP](../Operation-Guide/Elastic-IP-Management/Create-Elastic-IP.md)
- [价格总览](Price-Overview.md)
- [计费类型转换](Change-Billing.md)
- [计费规则](Billing-Rules.md)
- [常见计费问题](Bill-FAQ.md)
