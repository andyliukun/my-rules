# my-rules

用于整理和维护个人规则与约定。

## 使用

在仓库中添加或更新规则文档，并通过 Git 提交管理变更。

## Clash 规则配置

配置地址：

```text
https://raw.githubusercontent.com/andyliukun/my-rules/refs/heads/main/Clash-Full-US-auto.ini
```

`Clash-Full-US-auto.ini` 的域名组规则文件均保存在本仓库的 `rules/` 下，按原作者、仓库和文件路径分目录，避免同名文件冲突。修改对应的 `.list` 文件即可维护规则；策略组和节点组保持原配置。

规则是上游文件的静态副本，不会自动同步上游更新。`rules-sources.json` 记录首次复制时的来源地址及 SHA-256，供溯源；后续本地修改后，初始校验值不再代表当前文件。原文件中的来源和版权注释予以保留。

配置中的注释规则链接也已迁移。节点测速使用的 `www.gstatic.com` 地址用于连通性检测，保持原样。

无需安装依赖或启动服务。
