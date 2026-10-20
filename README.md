# QX 全量分流规则

Quantumult X 分流规则，**一个订阅搞定全部**。

## 订阅地址

```
https://cdn.jsdelivr.net/gh/YueBtt/qx-rules@v4/qx.filter
```

## 覆盖范围

| 分类 | 策略 | 条数 |
|---|---|---|
| **广告拦截**（最优先） | reject | 970 |
| **运营商劫持** | reject | 69 |
| 社交 / Google / 流媒体 | proxy | 66 |
| 开发工具 / 资讯 / 其他 | proxy | 53 |
| AI 服务 | proxy | 74 |
| 国内网站 | direct | 3704 |
| 国内 IP | direct | 5666 |
| 内网 | direct | 9 |
| 兜底 | proxy | 1 |

**合计 10612 条**

## 数据来源

- ConnersHua/RuleGo — 广告拦截
- blackmatrix7/ios_rule_script — 运营商劫持、国内网站、国内IP
- ddgksf2013 — AI 合集
- 自建 — 境外常用服务

## 使用

Quantumult X → 设置 → 分流 → 引用 → `+` → 粘贴订阅地址

**导入后请把其他分流资源全部取消勾选**，只保留这一条，避免规则冲突。

## 更新

以 v4 标签锁定版本，避免 CDN 缓存问题。更新时改标签重新推送。
