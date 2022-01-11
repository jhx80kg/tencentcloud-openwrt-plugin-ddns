# 腾讯云DDNS插件

## 1.插件介绍
> OpenWRT TencentDDNS插件是一款腾讯云研发的，自动映射动态公网IP至用户指定的DNSPod域名解析记录的官方插件。

| 标题       | 名称                                                         |
| ---------- | ------------------------------------------------------------ |
| 中文名称   | 腾讯云DDNS插件                                    |
| 英文名称   | luci-app-tencentddns                                   |
| 最新版本   | 0.1.0 (2020.09.17)                                           |
| 适用平台   | [Lean OpenWRT](https://github.com/coolsnowwolf/lede)         |
| 适用产品   | [DNSPod](https://www.dnspod.cn/)|
| GitHub项目 | [tencentcloud-openwrt-plugin-ddns](https://github.com/Tencent-Cloud-Plugins/tencentcloud-openwrt-plugin-ddns)                            |
| 主创团队   | 腾讯云中小企业产品中心（SMB Product Center of Tencent Cloud） |

## 注.本人已经修改
代码如下：

module("luci.controller.tencentddns",package.seeall)


function index()


entry({"admin", "network", "tencentddns"},cbi("tencentddns"),_("TencentDDNS"),2)


end


## 显示位置为 网络-腾讯云ddns
