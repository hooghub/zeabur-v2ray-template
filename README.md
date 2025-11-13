# 🌐 V2Ray + Nginx (Zeabur Edition)

**一键部署到 Zeabur 的 V2Ray + Nginx WebSocket 代理模板**

> ✅ 自动 HTTPS  
> ✅ 自定义 UUID  
> ✅ 伪装网页（静态文件）  
> ✅ 一键部署，无需命令行  

---

## 🚀 一键部署

点击下方按钮直接部署到你的 Zeabur：

[![Deploy to Zeabur](https://zeabur.com/button.svg)](https://zeabur.com/templates/new?template=https://github.com/你的GitHub用户名/zeabur-v2ray-template)

> ⚠️ 请替换上面链接中的 `你的GitHub用户名` 为你自己的 GitHub 用户名。

---

## ⚙️ 配置参数

| 变量名 | 类型 | 说明 |
|--------|------|------|
| `NGINX_DOMAIN` | 域名 | 要绑定的域名，Zeabur 会自动签发 HTTPS 证书 |
| `V2RAY_UUID` | 字符串 | 你要使用的 V2Ray 用户 ID，可在 [uuidgenerator.net](https://www.uuidgenerator.net/) 生成 |

---

## 🧩 服务结构

- **v2ray**：负责 vmess 协议代理  
- **nginx**：提供伪装网页与 WebSocket 转发  

访问结构：

---

## 🔌 客户端连接示例

| 参数 | 值 |
|------|----|
| 协议 | vmess |
| 地址 | 你的域名 |
| 端口 | 443 |
| UUID | 你部署时填写的 UUID |
| 传输 | ws |
| 路径 | /ws |
| TLS | 开启 |

---

## 🧠 注意事项

- 不得在中国大陆服务器上部署此模板。  
- 此模板仅供个人隐私、学习用途。  
- Zeabur 将自动为域名签发 TLS 证书，无需手动设置。  

---

## 🛠️ 自定义网页伪装

你可以在 Zeabur 的 nginx 服务中，  
上传你自己的 `index.html` 文件到 `/usr/share/nginx/html/` 目录，  
用来伪装成任意普通网站首页。

---

## 🧰 原理图


---

## 🪄 项目信息

- 作者：你自己  
- 镜像来源：teddysun/v2ray、library/nginx  
- 平台：Zeabur  
