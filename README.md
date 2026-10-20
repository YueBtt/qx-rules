# QX 分流规则

Quantumult X 分流规则集，托管于 jsDelivr CDN（国内可直连）。

## 订阅地址

```
https://cdn.jsdelivr.net/gh/YueBtt/qx-rules@main/qx.filter
```

## 使用方法

Quantumult X → 设置 → 分流 → 引用 → 右上角 `+` → 粘贴上方链接 → 保存

## 规则说明

| 分类 | 策略 | 内容 |
|---|---|---|
| 广告拦截 | reject | 各大广告联盟、统计 SDK |
| AI 服务 | proxy | OpenAI、Claude、Gemini、Perplexity、Grok、Copilot 等 |
| 社交 | proxy | X/Twitter、Telegram、Facebook、Instagram、Reddit、Discord |
| Google | proxy | Google 全家桶 |
| 流媒体 | proxy | YouTube、Netflix、Disney+、Prime Video、HBO、Spotify、Twitch |
| 开发工具 | proxy | GitHub、Stack Overflow、npm、Docker、Vercel |
| 资讯媒体 | proxy | Wikipedia、BBC、NYT、CNN、Bloomberg |
| 国内服务 | direct | 百度、腾讯、阿里、B站、抖音、小红书、银行等 |
| 内网 IP | direct | 10/8、172.16/12、192.168/16、127/8 |
| 中国 IP | direct | geoip, cn |
| 兜底 | proxy | 其余走代理 |

## 更新

规则更新后推送到本仓库，客户端按 profile-update-interval 自动拉取。
