# TikTok iOS 免拔卡教程，tiktok ios ipa 旧版下载（历史版本）

### 最新版的TikTok暂时不支持免拔卡使用，需要下载旧版。

### 操作步骤<br>
1、<a href="http://a.ssv2ray.com/tiktok.html" target="_blank">下载 tiktok ios ipa 旧版 点击下载>></a><br>

2、下载 Shadowrocket<br>

3、打开Shadowrocket → 配置 → default.conf → 编辑配置 → HTTPS解密 → 开启HTTPS解密 → 生成新的CA订书 → 生成新的CA订书 → 安装证书 → 允许 → 打开设置 → 已下载描述文件 → 安装 → 安装 → 安装 → 完成 → 通用 → 关于本机 → 证书信任设置 → 开启信任Shadowrocket证书 → 继续 → 打开Shadowrocket → 关闭 → √ → √ → 配置 → default.conf → 编辑纯文本 → 滚动条拉到最下面 <br>
在最下面粘贴以下代码：

    [URL Rewrite]
    (?<=_region=)CN(?=&) JP 307
    (?<=&mcc_mnc=)4 2 307
    ^(https?:\/\/(tnc|dm)[\w-]+\.\w+\.com\/.+)(\?)(.+) $1$3 302
    (^https?:\/\/*\.\w{4}okv.com\/.+&.+)(\d{2}\.3\.\d)(.+) $118.0$3 302

    [MITM]
    hostname = *.tiktokv.com,*.byteoversea.com,*.tik-tokapi.com
    
再点击保存。

4、在Shadowrocket添加节点，开启科学上网。<br>

5、打开TikTok App 即可实现免拔卡看，可以登录，评论。

### 如何更改国家：
默认是日本区，可以更改这行代码中的JP 【(?<=_region=)CN(?=&) JP 307】<br>
美国示例： (?<=_region=)CN(?=&) US 307<br>
英文简写 JP（日本）｜KR（韩国）｜UK（英国）｜US（美国）｜TW（台湾）
