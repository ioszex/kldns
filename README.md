# 洛克二级域名分发系统 （原快乐二级域名分发系统） （kldns v6.8.0）

## 此系统有哪些特点

* 目前支持的域名解析平台有
    * dnspod
    * cloudxns
    * aliyun
    * dnscom
    * dnsla
    * cloudxns
    * DnsDun
    * SRV
* 多用户、多域名、多平台同时存在
* 界面简单、舒适，操作简单
*6.8.0 (20250730)

   * 1、新增SRV解析
   * 2、新增几个首页 登录界面模板
   * 3、新增登录记录ip和登录时间
   * 4、新增积分 会员充值
   * 5、新增卡密兑换 积分转账
   * 6、新增手机号注冊（未完善）
   * 7、home目录更换全新ui模板
   * 8、修复了部分Cloudflare域名出现500错误的问题
   * 9、新增域名续费功能
   * 10、新增邀请码

## 安装说明

### 1、程序的框架是Laravel 5.8，因此需要环境满足以下要求：

* PHP >= 7.1.3
* PHP OpenSSL 扩展
* PHP PDO 扩展
* PHP Mbstring 扩展
* PHP Tokenizer 扩展
* PHP XML 扩展
* PHP Ctype 扩展
* PHP JSON 扩展
*PHP BCMath 扩展
* 2、环境必须支持伪静态

* Apache 伪静态配置
    * 确保 Apache 启用了 mod_rewrite 模块以支持 .htaccess 解析。
* Nginx 伪静态配置

        location / {
            try_files $uri $uri/ /index.php?$query_string;
        }