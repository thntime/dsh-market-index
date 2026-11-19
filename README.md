# dsh-market-index

thntime 的 DSH（DeepSeek Harness）插件市场索引，给插件管理器的「发现」（Discover）用。

## 怎么用

1. 打开 **Plugins**，在 **Experimental plugins** 旁点 **More**，打开 **Custom plugin markets**
2. 进 **Discover** 标签，选 **Add index source**，填：

```
https://thntime.github.io/dsh-market-index/index.json
```

3. 列表里出现插件后点 **Install**，DSH 会自己检查兼容性再装

## 收录

| 插件 | 说明 |
| --- | --- |
| [dsh-new-api-model-sync](https://www.npmjs.com/package/dsh-new-api-model-sync) | 把 new-api 的 `/v1/models` 清单同步成 DSH 模型条目，写入走 configEditor，不用重启 |

## 格式

`index.json` 是市场索引，`format: 1`。每条插件带 `name`（npm 包名）、`repository`、`versions[].source`（`type: npm`）和 `engines.dsh` 兼容区间。

## License

MIT
