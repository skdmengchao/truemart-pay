#项目结构
```
|-truemart-pay
|   |
|   |-truemart-pay-api------------------api接口定义
|   |-truemart-pay-gateway--------------收银台，支付网关
|   |-truemart-pay-microservice---------支付系统微服务
|   |-truemart-pay-service--------------支付公共服务
|   |-truemart-pay-task-----------------支付相关任务
```
#API编码

```
平台编码（2位）+ 领域编码（2位）+ 模块编码（2位）+ 功能编码（2位）+ 操作编码（2位）

平台编码：13

领域：
    微服务（microservice）:10
        账户信息(account)：01
        保证金(deposit)：02
        基础数据(dic)：03
        支付(payment)：04
        对账(reconcilication)：05
        退款(refund)：06
        服务费(serviceCharge)：07
        结算(settlement):08
        白条(whitebar):09
        对外接口(server):10

    支付网关（gateway）:11
        支付网关：01
        支付通知：02
        支付方式：03
        对外接口：04
        
    定时任务（task）:12

```
# truemart-pay
