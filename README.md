# WechatIntegrateExchange
微信集成Exchange AD登录邮箱，验证的架构如左图和下面说明。其中“微信扫码入口”，“微信账户验证中心”和“AD FS”需要自行开发。

![WCADFSF](https://github.com/FL-LearningGroup/WechatIntegrateExchange/blob/main/WeChatIntegrateADFSFramework.JPG)

## 主要功能说明
### 微信扫码入口

1. 扫描二维码，微信接收扫码信息

2. 微信将接收的信息（微信openId）转发给微信账户验证中心

3. 接收微信账户验证中心返回的验证结果，如果成功则直接进入企业邮箱

4. 绑定微信账户和企业邮箱账户

### 微信账户验证中心

1. 接收微信账户信息，转发给AD FS

2. 将验证结果转发给微信扫码入口


### AD FS

1. 微信账户验证，返回验证结果​
