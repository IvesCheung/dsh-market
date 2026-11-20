# dsh-market

DSH（DeepSeek Harness）插件市场索引。在 **插件 → 发现 → 索引源** 里加这个地址即可：

```
https://raw.githubusercontent.com/IvesCheung/dsh-market/main/index.json
```

国内网络可用镜像前缀（jsDelivr 走 CDN）：

```
https://cdn.jsdelivr.net/gh/IvesCheung/dsh-market@main/index.json
```

## 收录

| 插件 | 说明 |
| --- | --- |
| [dsh-sidebar-shrink](https://github.com/IvesCheung/dsh-sidebar-shrink) | 把很久不点的侧栏面板收进「更多」并记住；工作区一键全部折叠 |

## 格式

索引格式 1，由 `@deepseek-ai/dsh-plugin-market-index` 校验。每个版本的 `source.commit` 是固定到 40 位 SHA 的 Git 来源，安装时 pnpm 会解析成：

```
git+https://github.com/IvesCheung/dsh-sidebar-shrink.git#<commit>
```

发新版本时改 `versions`（新加一条，`version` 升号、`commit` 换成新 SHA、`publishTimestamp` 更新），再跑一次校验。
