# 使用限制

VPC网段不可与公共服务网段重叠，各地域的公共服务网段如下。




| 所属地域 | 网段 |
| ---- | ---- |
| 华北（北京） | 10.19.192.0/18,10.9.192.0/18,10.10.192.0/18,10.42.192.0/18,100.65.0.0/18|
| 华北（乌兰察布） |100.65.128.0/18|
| 上海金融云 | 10.15.224.0/19,10.15.200.0/24 |
| 上海二 | 10.23.248.0/21,10.25.248.0/21,10.23.200.0/24,10.25.200.0/24,100.64.128.0/18 |
| 广州 | 10.13.192.0/18,100.64.64.0/18 |
| 泉州 | 100.64.32.0/20 |
| 杭州 | 100.64.16.0/20 |
| 香港 | 10.8.192.0/18,10.7.192.0/18,100.65.64.0/18 |
| 洛杉矶 | 10.11.192.0/18 | 
| 华盛顿 | 10.27.192.0/18 |
| 法兰克福 | 10.29.192.0/18 |
| 曼谷 | 10.31.192.0/18 |
| 韩国 | 10.33.192.0/18 |
| 新加坡 | 10.35.192.0/18,100.64.208.0/20 |
| 高雄 | 10.37.192.0/18 |
| 莫斯科 | 10.39.192.0/18 |
| 东京 | 10.40.192.0/18,100.65.192.0/20 |
| 台北 | 10.41.192.0/18 |
| 迪拜 |10.44.192.0/18 |
| 雅加达 | 10.45.192.0/18 |
| 孟买 |10.47.192.0/18 |
| 圣保罗 |10.49.192.0/18 |
| 伦敦 | 10.50.192.0/18 |
| 拉各斯 |10.52.192.0/18 |
| 胡志明 | 100.64.0.0/20 |
| 马尼拉 | 100.64.48.0/20 |

为了保证UCloud内部提供的各种功能正常，ACL将默认放行以上UCloud提供的公共服务网段，ACL的默认行为不会对您的业务安全有任何影响。
