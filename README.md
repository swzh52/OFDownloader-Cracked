# OFDownloader Chrome 2.2.2 Cracked

> 基于 OFDownloader Chrome 2.2.2 的破解版本，绕过会员认证、登录付费和下载限制。

## 🚀 特性

- **MAX 会员解锁** — 绕过所有会员等级检查，固定返回 MAX
- **Token 认证绕过** — 无需登录即可使用全部功能
- **下载无限制** — 并发配额、文件大小、DRM 等限制全部解除

## 📦 安装

### 方法一：下载 Release 包

1. 前往 [Releases](https://github.com/swzh52/OFDownloader-Cracked/releases) 页面
2. 下载最新的 `OFDownloader-Cracked-v2.2.2.tar.gz`
3. 解压到本地文件夹
4. 打开 Chrome → `chrome://extensions/`
5. 开启右上角「开发者模式」
6. 点击「加载已解压的扩展程序」，选择解压后的文件夹

### 方法二：从源码安装

```bash
git clone https://github.com/swzh52/OFDownloader-Cracked.git
```

然后按上述方法 4-6 步加载。

## 🔧 修改内容

| 文件 | 修改项 | 说明 |
|------|--------|------|
| `background.js` | `Va()` → `return true` | 绕过服务端会员等级检查 |
| `chunks/debug-CzyvQXIg.js` | 默认 `memberType:"MAX"`, `isPro:true` | 初始状态即为 MAX 会员 |
| `chunks/debug-CzyvQXIg.js` | `en()` → 固定返回已认证+MAX | 绕过 Token 验证 |
| `chunks/app-CaowBQ0s.js` | `dH()` → `return "MAX"` | 客户端会员等级固定 MAX |
| `chunks/app-CaowBQ0s.js` | `WN()` → `return true` | 认证检查始终通过 |
| `chunks/app-CaowBQ0s.js` | `LAe()` → `return "MAX"` | 下载并发配额无限制 |
| `chunks/app-CaowBQ0s.js` | **`TA()` → `return false`** | **阻止所有登录/订阅 URL 跳转** |
| `chunks/app-CaowBQ0s.js` | 按钮文字清空 | Sign In / Purchase License / Verify License / Buy now |
| `content-scripts/content.js` | `N0()` → `return true` | 侧栏认证绕过 |
| `content-scripts/content.js` | `zD()` → `return "MAX"` | 侧栏配额无限制 |
| `content-scripts/content.js` | 侧栏 Sign In 文字清空 | 侧栏登录按钮文字移除 |

## ⚠️ 免责声明

- 本仓库仅供学习和研究用途
- 请支持 OFDownloader 原作者
- 使用本软件产生的任何后果由使用者自行承担


