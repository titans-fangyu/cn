# 计费规则
- [包年包月](Billing-Rules#user-content-1)
- [按配置计费](Billing-Rules#user-content-2)
- [按流量计费](Billing-Rules#user-content-3)
 
## 包年包月

<div id="user-content-1"></div>

包年包月为预付费，先支付后使用，一次性至少支付一个月，支持支付多个月或多年的费用，适用于提前预估弹性公网IP带宽需求的场景，价格相比按配置计费更低廉。

#### 规则

- 提前支付数月或数年的费用，目前购买时间段支持1个月~9个月、1年(按年购买会有相应的折扣)、2年、3年；费用在您创建资源时一次性扣除；

- 包年包月的资源在到期前不支持删除操作，为了保障您的使用权益，请确认业务需求后进行购买，更多限制请参考[使用限制](../Introduction/Restrictions.md)

- 包年包月计费订单的到期时间为订单开始时间当日起向后第N个自然月或自然年的 23:59:59；
例如：订单的开始时间为2016年1月1日 15:00:00，购买时长为1个月，则到期时间为2016年月2日1日 23:59:59。



#### 到期说明
- 当您的包年包月付费网络资源到期时间早于或等于当前时间，则您的付费网络资源状态会变为过期。到期后您的付费网络资源（弹性公网IP）将被停止服务，不能继续使用；

- 您的包年包月付费网络资源到期前，京东云会向您[绑定的邮箱及手机号](https://docs.jdcloud.com/cn/account-management/change-jdcloud-phone-number)发送邮件、短信，提醒您的资源即将到期，请您注意查看并及时续费；

- 您的付费网络资源到期后，会向您发送邮件和短信通知您的资源已到期，请您务必注意查看通知并及时充值，以免造成不必要的损失；

- 从停止服务时刻起，您的付费网络资源和资源中的数据保留7天，7天后系统回收资源，数据无法找回；

- 在资源被释放前续费，被停用的资源可正常使用。

#### 示例
您在2017-8-2 10:00:00购买1个月1M带宽的BGP弹性公网IP，月单价为23元，则您需要支付的费用为23=23\*1元，您可以使用该资源至2017-9-2 23:59:59。

## 按配置

<div id="user-content-2"></div>

按配置计费为后付费方式，先使用后支付，最早扣费时间为创建公网IP后的整点时刻，计费周期为一小时，根据您购买的弹性公网IP配置情况，以及计费周期内的实际使用时长（精确到秒），在每整点计算前一周期的费用并扣费。

#### 规则
- 按资源的实际购买配置计费，统计时间精确到秒，适用于业务量波动较大的场景；

- 开通说明：为保证您的正常使用，开通按配置计费的资源时您的账户余额不得少于50元。如账户金额少于50元，需充值后方可使用。

- 付费模式：采用先使用后付费方式，按资源配置及实际使用时长每小时生成账单并结算费用。

- 计费模式转换：按配置计费可通过续费转成包年包月计费类型，计费类型转换不可逆，具体操作请参考[续费流程](Renew-Process.md)。

#### 欠费说明

- 当您的账户中余额加可用于支付该付费网络资源的代金券的总和不足以支付下一计费周期费用时，导致扣款不成功，您的付费网络资源（弹性公网IP）的状态会变为欠费；

- 当您的付费网络资源欠费后，将停止服务且停止扣费；

- 当您的付费网络资源欠费后，京东云会向您[绑定的邮箱及手机号](https://docs.jdcloud.com/cn/account-management/change-jdcloud-phone-number)发送邮件和短信，通知您的资源已欠费，请您务必注意查看通知并及时充值，以免造成不必要的损失；

- 从停止服务时刻起，您的付费网络资源和资源中的数据保留7天，7天后系统回收资源，数据无法找回；

- 当您补缴欠费金额后，被停用的付费网络资源方可正常使用；

- 如您不想继续使用按配置的付费网络资源，请及时将该资源进行删除。

#### 示例
您在2017-8-2 10:30:00购买的按配置计费的BGP弹性公网IP，带宽为1M，每小时价格0.06元/小时，则在2017-8-2 11:00:00结算上一小时（实际使用了半小时）的费用（0.06\*0.5=0.03元），在后续的每个整点结算费用（0.06元），在您删除弹性公网IP时结算该周期的尾款。




## 按用量

<div id="user-content-3"></div>

按用量计费为后付费方式，计费周期为一天，每天每个弹性公网IP收取保有费，并按照每天实际使用出方向流量结算流量费用。

#### 详细说明
- 按公网IP的实际使用流量付费，统计时间精确到秒，适用于单日内公网业务流量波动较大的场景。

- 开通说明：为保证您的正常使用，开通按用量计费的公网IP时您的账户余额不得少于50元。如账户金额少于50元，需充值后方可使用。

- 计费采用后付费模式，开通时无须支付费用，创建后的每个自然日的00:00:00会根据资源保有时间和实际使用流量出账单并结算费用。

- 删除公网IP时，按账单周期内实际保有时长和使用流量出账单并结算费用。

- 计费模式转换：按用量计费可通过续费转成包年包月计费类型，计费类型转换不可逆，具体操作请参考[续费流程](Renew-Process.md)。

#### 欠费说明
- 出账单时，当您的账户中余额加可用于支付该付费网络资源的代金券的总和不足，导致扣款不成功，您的付费网络资源（弹性公网IP）的状态会变为欠费；

- 当您的付费网络资源欠费后，将停止服务且停止扣费；

- 当您的付费网络资源欠费后，京东云会向您[绑定的邮箱及手机号](https://docs.jdcloud.com/cn/account-management/change-jdcloud-phone-number)发送邮件和短信，通知您的资源已欠费，请您务必注意查看通知并及时充值，以免造成不必要的损失；

- 从停止服务时刻起，您的付费网络资源和资源中的数据保留7天，7天后系统回收资源，数据无法找回；

- 当您补缴欠费金额后，被停用的付费网络资源方可正常使用；

- 如您不想继续使用按配置的付费网络资源，请及时将该资源进行删除。

#### 示例
您在2017-8-2 10:30:00购买的按用量计费的BGP弹性公网IP，假设当天出流量为1GB，则在2017-8-3 00:00:00结算上一天的费用(0.48+0.8\*1=1.28元)，在您删除弹性公网IP时结算该周期的尾款。


## 相关参考

- [计费概述](Billing-Overview.md)
- [产品概述](../Introduction/Product-Overview.md)
- [创建公网IP](../Operation-Guide/Elastic-IP-Management/Create-Elastic-IP.md)
- [价格总览](Price-Overview.md)
- [计费类型转换](Change-Billing.md)
- [续费公网IP](../Operation-Guide/Elastic-IP-Management/Renew-Elastic-IP.md)
- [常见计费问题](Bill-FAQ.md)

