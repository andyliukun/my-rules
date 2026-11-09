# my-rules

用于整理和维护个人规则与约定。

## 使用

在仓库中添加或更新规则文档，并通过 Git 提交管理变更。

## Clash 规则配置

配置地址：

```text
https://raw.githubusercontent.com/andyliukun/my-rules/refs/heads/main/Clash-Full-US-auto.ini
```

`Clash-Full-US-auto.ini` 的域名组规则文件均保存在本仓库的 `rule-set/` 下。修改对应的 `.list` 文件即可维护规则；策略组和节点组保持原配置。

规则是上游文件的静态副本，不会自动同步上游更新。`rules-sources.json` 记录当前文件对应的上游来源地址及原始副本 SHA-256，供溯源；校验值不代表合并或修改后的当前文件。Steam 和 YouTube 已分别合并多个来源的规则。原文件中的来源和版权注释予以保留。

已删除未使用的备用 Global 注释引用。节点测速使用的 `www.gstatic.com` 地址用于连通性检测，保持原样。

无需安装依赖或启动服务。

## Steam 下载分流

`Steam下载.list` 中列出的国内下载 CDN 优先直连，商店和社区使用 `🛒 Steam商店` 策略组，其他已匹配的 Steam 流量使用 `🎮 Steam游戏` 策略组（均默认节点选择，可分别选择具体节点或直连）。请勿将整个 `steampowered.com` 设为直连。未列入的下载 CDN 仍按后续规则处理；实际使用的 CDN 由 Steam 分配。

`SteamStore.list` 在通用 Steam 规则前匹配商店、结账、帮助、Web API、社区及常用静态资源。该分流基于域名，无法严格按客户端功能区分共享域名上的每个请求；未单独列出的服务按后续规则处理。
