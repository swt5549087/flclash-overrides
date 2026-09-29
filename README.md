# FlClash 自定义覆写

个人 FlClash 分组与分流配置。仅包含覆写代码，不包含机场订阅链接、节点密码或访问令牌。

## 固定下载地址

```text
https://raw.githubusercontent.com/swt5549087/flclash-overrides/main/override.js
```

在 FlClash 的覆写脚本编辑器中选择“从 URL 导入”，填写上述地址，保存后绑定到需要使用的订阅。
这是 JavaScript 覆写脚本，不是可直接添加到“配置订阅”的 YAML 地址。

## 后续更新

只维护 `main` 分支下的 `override.js`。提交修改后，固定地址不变，其他设备可重新从同一 URL 导入并保存。
FlClash 0.8.98 的脚本 URL 导入为一次性下载，不会自动更新已导入的本地脚本。
GitHub Raw 可能短暂缓存旧内容；刚发布后若仍显示旧版，可稍后重试。

## 当前设置

- 香港、新加坡（狮城）、美国：自动测速，间隔 300 秒。
- 台湾、日本、韩国、其他节点：手动选择。
- “自动选择”沿用原名称，但类型为手动选择，避免额外测速。
- 漏网之鱼默认 DIRECT；实际选择仍以各设备保存的状态为准。
- Notion 主要域名和 `5dm.ink` 及其子域名：国外媒体。
- 保留原来的公共规则源和 Home Depot、Chrome 商店等自定义分流。

修改网站规则时编辑 `override.js` 中的 `config["rules"]`。规则按顺序匹配，优先规则放在前面。
