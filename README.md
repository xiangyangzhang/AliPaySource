# AlipaySource
---

## 1.支付宝
开发平台 (找不到iOS sdk)

旧的 :[旧支付宝网址](http://open.alipay.com/index.htm)(这个里面找不到sdk) 需要进入下面的链接
新的:[新的支付宝网址](https://openhome.alipay.com/platform/home.htm)

使用支付宝进行一个完整的支付功能，大致有以下步骤：

####1>先与支付宝签约，获得商户ID（partner）和账号ID（seller）
(这个主要是公司的负责)

####2>下载相应的公钥私钥文件（加密签名用）

####3>下载支付宝SDK
官方sdk页面地址：(藏得很深) 现在在开放平台就可以进入了
[官方sdk页面地址](https://b.alipay.com/order/productDetail.htm?productId=2014110308141993&tabId=4#ps-tabinfo-hash)
里面提供了非常详细的文档、如何签约、如何获得公钥私钥、如何调用支付接口。

####4>生成订单信息
####5>调用支付宝客户端，由支付宝客户端跟支付宝安全服务器打交道
####6>支付完毕后返回支付结果给商户客户端和服务器

**SDK里有集成支付宝功能的一个Demo>  集成支付功能的具体操作方式，可以参考Demo**

![enter image description here](https://github.com/xiangyangzhang/AliPaySource/blob/master/Alipay.png)

**调用支付接口可以参考AlixPayDemoViewController的下面方法
-(void)tableView:(UITableView *)tableView didSelectRowAtIndexPath:(NSIndexPath *)indexPath

如何创建订单 ( 订单根据自己公司看是什么样的)
如何签名
如何调用支付接口
都在这个方法里面了**

###2.微信支付
- [微信支付](https://open.weixin.qq.com/cgi-bin/showdocument?action=dir_list&t=resource/res_list&verify=1&lang=zh_CN)