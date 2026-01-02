# 🚀 edgetunnel 2.0
![后台页面](./img.png)

- **edgetunnel 最新教程**：https://www.youtube.com/watch?v=tKe9xUuFODA ***必看内容!必看内容!必看内容!!!***
- **报错 Error 1101 详解**：https://www.youtube.com/watch?v=r4uVTEJptdE

- Telegram交流群：[@CMLiussss](https://t.me/CMLiussss)

## ⚠️ 免责声明

本免责声明适用于 GitHub 上的 “edgetunnel” 项目（以下简称“本项目”），项目链接为：https://github.com/cmliu/edgetunnel 。

### 用途
本项目仅供教育、研究和安全测试目的而设计和开发。旨在为安全研究人员、学术界人士及技术爱好者提供一个探索和实践网络通信技术的工具。

### 合法性
在下载和使用本项目代码时，必须遵守使用者所适用的法律和规定。使用者有责任确保其行为符合所在地区的法律框架、规章制度及其他相关规定。

### 免责
1. 作为本项目的 **二次开发作者**（以下简称“作者”），我 **cmliu** 强调本项目仅应用于合法、道德和教育目的。
2. 作者不认可、不支持亦不鼓励任何形式的非法使用。如果发现本项目被用于任何非法或不道德的活动，作者将对此强烈谴责。
3. 作者对任何人或组织利用本项目代码从事的任何非法活动不承担责任。使用本项目代码所产生的任何后果，均由使用者自行承担。
4. 作者不对使用本项目代码可能引起的任何直接或间接损害负责。
5. 为避免任何意外后果或法律风险，使用者应在使用本项目代码后的 24 小时内删除代码。

通过使用本项目代码，使用者即表示理解并同意本免责声明的所有条款。如使用者不同意这些条款，应立即停止使用本项目。

作者保留随时更新本免责声明的权利，且不另行通知。最新版本的免责声明将发布在本项目的 GitHub 页面上。

## 🔥 风险提示
- 通过提交虚假的节点配置给订阅服务，避免节点配置信息泄露。
- 另外，您也可以选择自行部署 [WorkerVless2sub 订阅生成服务](https://github.com/cmliu/WorkerVless2sub)，这样既可以利用订阅生成器的便利。
   
## 💡 如何使用?
### ⚙️ Workers 部署方法 [视频教程](https://www.youtube.com/watch?v=tKe9xUuFODA&t=191s)

<details>
<summary><code><strong>「 Workers 部署文字教程 」</strong></code></summary>

1. 部署 CF Worker：
   - 在 CF Worker 控制台中创建一个新的 Worker。
   - 将 [worker.js](https://github.com/cmliu/edgetunnel/blob/main/_worker.js) 的内容粘贴到 Worker 编辑器中。
   - 在左侧的 `设置`选项卡中，选择 `变量` > `添加变量`。
     变量名称填写**ADMIN**，值则为你的管理员密码，后点击 `保存`即可。

2. 绑定 KV 命名空间：
   - 在 `绑定`选项卡中选择 `添加绑定 +` > `KV 命名空间` > `添加绑定`，然后选择一个已有的命名空间或创建一个新的命名空间进行绑定。
   - `变量名称`填写**KV**，然后点击 `添加绑定`即可。

3. 给 Workers绑定 自定义域： 
   - 在 workers控制台的 `触发器`选项卡，下方点击 `添加自定义域`。
   - 填入你已转入 CF 域名解析服务的次级域名，例如:`vless.google.com`后 点击`添加自定义域`，等待证书生效即可。
   - **如果你是小白，你现在可以直接起飞，不用再往下看了！！！**

4. 访问后台：
   - 访问 `https://vless.google.com/admin` 输入管理员密码即可登录后台。

</details>

### 🛠 Pages 上传 部署方法 **最佳推荐!!!** [视频教程](https://www.youtube.com/watch?v=tKe9xUuFODA&t=436s)

<details>
<summary><code><strong>「 Pages 上传文件部署文字教程 」</strong></code></summary>

1. 部署 CF Pages：
   - 下载 [main.zip](https://github.com/cmliu/edgetunnel/archive/refs/heads/main.zip) 文件，并点上 Star !!!
   - 在 CF Pages 控制台中选择 `上传资产`后，为你的项目取名后点击 `创建项目`，然后上传你下载好的 [main.zip](https://github.com/cmliu/edgetunnel/archive/refs/heads/main.zip) 文件后点击 `部署站点`。
   - 部署完成后点击 `继续处理站点` 后，选择 `设置` > `环境变量` > **制作**为生产环境定义变量 > `添加变量`。
     变量名称填写**ADMIN**，值则为你的管理员密码，后点击 `保存`即可。
   - 返回 `部署` 选项卡，在右下角点击 `创建新部署` 后，重新上传 [main.zip](https://github.com/cmliu/edgetunnel/archive/refs/heads/main.zip) 文件后点击 `保存并部署` 即可。

2. 绑定 KV 命名空间：
   - 在 `设置`选项卡中选择 `绑定` > `+ 添加` > `KV 命名空间`，然后选择一个已有的命名空间或创建一个新的命名空间进行绑定。
   - `变量名称`填写**KV**，然后点击 `保存`后重试部署即可。

3. 给 Pages绑定 CNAME自定义域：[视频教程](https://www.youtube.com/watch?v=LeT4jQUh8ok&t=851s)
   - 在 Pages控制台的 `自定义域`选项卡，下方点击 `设置自定义域`。
   - 填入你的自定义次级域名，注意不要使用你的根域名，例如：
     您分配到的域名是 `fuck.cloudns.biz`，则添加自定义域填入 `lizi.fuck.cloudns.biz`即可；
   - 按照 CF 的要求将返回你的域名DNS服务商，添加 该自定义域 `lizi`的 CNAME记录 `edgetunnel.pages.dev` 后，点击 `激活域`即可。
   - **如果你是小白，那么你的 pages 绑定`自定义域`之后即可直接起飞，不用再往下看了！！！**
   
4. 访问后台：
   - 访问 `https://lizi.fuck.cloudns.biz/admin` 输入管理员密码即可登录后台。

</details>

### 🛠 Pages GitHub 部署方法 [视频教程](https://www.youtube.com/watch?v=tKe9xUuFODA&t=317s)

<details>
<summary><code><strong>「 Pages GitHub 部署文字教程 」</strong></code></summary>

1. 部署 CF Pages：
   - 在 Github 上先 Fork 本项目，并点上 Star !!!
   - 在 CF Pages 控制台中选择 `连接到 Git`后，选中 `edgetunnel`项目后点击 `开始设置`。
   - 在 `设置构建和部署`页面下方，选择 `环境变量（高级）`后并 `添加变量`
     变量名称填写**ADMIN**，值则为你的管理员密码，后点击 `保存并部署`即可。

2. 绑定 KV 命名空间：
   - 在 `设置`选项卡中选择 `绑定` > `+ 添加` > `KV 命名空间`，然后选择一个已有的命名空间或创建一个新的命名空间进行绑定。
   - `变量名称`填写**KV**，然后点击 `保存`后重试部署即可。

3. 给 Pages绑定 CNAME自定义域：[视频教程](https://www.youtube.com/watch?v=LeT4jQUh8ok&t=851s)
   - 在 Pages控制台的 `自定义域`选项卡，下方点击 `设置自定义域`。
   - 填入你的自定义次级域名，注意不要使用你的根域名，例如：
     您分配到的域名是 `fuck.cloudns.biz`，则添加自定义域填入 `lizi.fuck.cloudns.biz`即可；
   - 按照 CF 的要求将返回你的域名DNS服务商，添加 该自定义域 `lizi`的 CNAME记录 `edgetunnel.pages.dev` 后，点击 `激活域`即可。
   - **如果你是小白，那么你的 pages 绑定`自定义域`之后即可直接起飞，不用再往下看了！！！**

4. 访问后台：
   - 访问 `https://lizi.fuck.cloudns.biz/admin` 输入管理员密码即可登录后台。

</details>

## 🔑 变量说明

| 变量名 | 示例 | 必填 | 备注 |
|--------|---------|-|-----|
| ADMIN | `123456` |✅| 面板登录密码 |
| KEY | `CMLiussss` |❌| 快速订阅密钥，访问`/CMLiussss`即可快读订阅。 |
| HOST | `edt-pages.github.io` |❌| 强制固定伪装域名(支持多元素，使用`换行符`或`,`做间隔) |
| UUID | `90cd4a77-141a-43c9-991b-08263cfe9c10` |❌| 强制固定UUID |
| PATH | `/` |❌| 强制固定路径 |
| PROXYIP | `proxyip.cmliussss.net:443` |❌| 更换默认内置PROXYIP |
| URL | `https://cloudflare-error-page-3th.pages.dev` |❌| 主页反代伪装(乱设容易触发反诈，反代被墙的网站会加速域名被墙) |
| GO2SOCKS5  | `blog.cmliussss.com`,`*.ip111.cn`,`*google.com` |❌| 设置`SOCKS5`或`HTTP`变量之后，可设置强制使用socks5访问名单(设置为`*`可作为全局代理) |

## 核心概念与订阅配置指南

### 1. 项目概述

本项目是一个部署在 Cloudflare 上的 Worker，它作为一个高度可配置的代理和订阅生成器。其核心功能是动态生成适用于Clash、Sing-Box等客户端的代理节点信息，并能利用Cloudflare网络特性优化连接。

### 2. 核心概念

#### 2.1 访问端点

- **域名访问**: Worker没有固定的IP地址。您应当通过其域名（例如 `your-worker-name.your-account.workers.dev` 或您绑定的自定义域名）来访问。Cloudflare的全球网络会自动将您的请求路由到最近的数据中心。
- **客户端配置**: 在Clash等客户端中，服务器地址(`server`)应填写Worker的**域名**。

#### 2.2 代理链 (`PROXYIP`)

- `PROXYIP` 是一个可选的上游代理服务器（IP或域名）。
- 当设置了`PROXYIP`时，Worker会将收到的流量再次转发到这个上游代理，从而形成代理链。
- 可以在环境变量中设置一个全局默认值，也可以在每次请求的URL中动态指定。

### 3. 订阅生成机制

当您访问订阅地址（如 `/sub?token=...`）时，Worker会实时生成订阅内容。其中，节点IP的来源是核心，主要通过以下三种方式配置，由管理后台`config.json`中的 `优选订阅生成.本地IP库.随机IP` 选项控制。

---

#### **方式A：动态随机生成 (默认)**

- **配置**: `随机IP` 设置为 `true`。
- **行为**: 这是默认的工作方式。Worker会根据您访问时所在的网络运营商（ASN），从Cloudflare官方IP段中实时随机生成一批IP地址。
- **优点**: 自动化，无需维护，能动态适应不同网络环境，寻找最优连接。
- **注意**: 在此模式下，`ADD.txt` 文件中的内容会被忽略。

---

#### **方式B：使用自定义IP列表**

- **配置**: `随机IP` 设置为 `false`。
- **行为**: Worker会去读取您在管理后台 `ADD.txt` 文件中保存的IP列表，并使用这些IP来生成节点。
- **优点**: 完全可控，您可以使用自己筛选的、认为最稳定的IP地址。
- **回退机制**: 如果 `ADD.txt` 为空，Worker会自动回退到**方式A**。
- **如何设置**:
    1.  在管理后台将 `随机IP` 设置为 `false`。
    2.  在 `ADD.txt` 编辑框中，填入您自己的IP地址列表（每行一个）。

---

#### **方式C：调用外部API获取IP**

- **配置**: `随机IP` 设置为 `false`。
- **行为**: 这是方式B的扩展。您可以在 `ADD.txt` 文件中填入一个或多个API的URL地址。Worker在读取 `ADD.txt` 时，会自动请求这些URL，获取返回的文本内容作为IP列表，并与 `ADD.txt` 中其他的IP地址合并后使用。
- **优点**: 高度灵活和自动化，可以对接第三方优选IP服务。
- **如何设置**:
    1.  在管理后台将 `随机IP` 设置为 `false`。
    2.  在 `ADD.txt` 编辑框中，填入API的URL（例如 `https://api.example.com/get/ips`），每个URL占一行。也可以与普通IP地址混合使用。

## ⭐ Star 星星走起
[![Stargazers over time](https://starchart.cc/cmliu/edgetunnel.svg?variant=adaptive)](https://starchart.cc/cmliu/edgetunnel)

## 💻 已适配客户端
### Windows
   - [v2rayN](https://github.com/2dust/v2rayN)
   - clash.meta（[FlClash](https://github.com/chen08209/FlClash)，[mihomo-party](https://github.com/mihomo-party-org/mihomo-party)，[clash-verge-rev](https://github.com/clash-verge-rev/clash-verge-rev)，[Clash Nyanpasu](https://github.com/keiko233/clash-nyanpasu)）
### IOS
   - Surge，小火箭
   - sing-box（[SFI](https://sing-box.sagernet.org/zh/clients/apple/)）
### 安卓
   - clash.meta（[ClashMetaForAndroid](https://github.com/MetaCubeX/ClashMetaForAndroid)，[FlClash](https://github.com/chen08209/FlClash)）
   - sing-box（[SFA](https://github.com/SagerNet/sing-box)）
### MacOS
   - clash.meta（[FlClash](https://github.com/chen08209/FlClash)，[mihomo-party](https://github.com/mihomo-party-org/mihomo-party)）


# 🙏 特别鸣谢
### 💖 赞助支持 - 提供云服务器维持[订阅转换服务](https://sub.cmliussss.net/)
- [NodeLoc](https://www.nodeloc.com/)
- [Alice](https://url.cmliussss.com/alice)
- [EasyLinks](https://www.vmrack.net?ref_code=5Zk7eNhbgL7)
- [ZMTO(VTEXS)](https://zmto.com/?affid=1532)

### 🛠 开源代码引用
- [zizifn/edgetunnel](https://github.com/zizifn/edgetunnel)
- [3Kmfi6HP/EDtunnel](https://github.com/6Kmfi6HP/EDtunnel)
- [SHIJS1999/cloudflare-worker-vless-ip](https://github.com/SHIJS1999/cloudflare-worker-vless-ip)
- [Stanley-baby](https://github.com/Stanley-baby)
- [ACL4SSR](https://github.com/ACL4SSR/ACL4SSR/tree/master/Clash/config)
- [股神](https://t.me/CF_NAT/38889)
- [Workers/Pages Metrics](https://t.me/zhetengsha/3382)
- [白嫖哥](https://t.me/bestcfipas)
- [Mingyu](https://github.com/ymyuuu/workers-vless)
- [Alexandre Kojève](https://t.me/Enkelte_notif/784)：stallTCP v1.3
- [eooce](https://github.com/eooce/Cloudflare-proxy)
- [Sukka](https://ip.skk.moe/)