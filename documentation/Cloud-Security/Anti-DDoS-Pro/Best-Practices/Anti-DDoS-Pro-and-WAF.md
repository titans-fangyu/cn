# DDoS IP高防结合Web应用防火墙方案说明

DDoS IP高防+Web应用防火墙提供三层到七层安全防护体系，应用场景包括游戏、金融、电商、互联网、政企等京东云内和云外的各类型用户。

# 部署架构
![部署架构](https://github.com/jdcloudcom/cn/blob/edit/image/Advanced%20Anti-DDoS/Best-Practice02.png)<Br/>
DDoS IP高防+Web应用防火墙的最佳部署架构如下：
- 京东云的安全调度中心，通过DNS解析，将用户域名解析到DDoS IP高防CNAME。
- 用户正常访问流量和DDoS攻击流量经过DDoS IP高防清洗，回源至Web应用防火墙。
- 攻击者恶意请求被Web应用防火墙过滤后返回用户源站。
- Web应用防火墙可以保护任何公网的服务器，包括但不限于京东云，其他厂商的云，IDC等

# 方案优势
1. 用户源站在DDoS IP高防和Web应用防火墙之后，起到隐藏源站IP的作用。
2. CNAME接入，配置简单，减少运维人员工作。
