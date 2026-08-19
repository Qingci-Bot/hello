# Hello 示例插件（独立仓库）

Hello World 示例插件，演示 Qingci-Bot 插件 SDK 能力。仓库根目录即插件源码，可作为新插件仓库的模板参考。

## 安装

**方式一：通过插件市场安装**

本插件已登记在 [Qingci-Bot 插件市场](https://github.com/Qingci-Bot/Plugin-Market)（`source` 指向本仓库）。Qingci-Bot WebUI「插件管理 → 插件市场」搜索 `hello` 一键安装。

**方式二：手动安装**

```bash
git clone https://github.com/Qingci-Bot/hello.git
# 将仓库内容放入 Qingci-Bot 实例的 plugins/hello/ 目录，重启机器人
```

安装后 Qingci-Bot 会自动读取 `requirements.txt` 安装依赖（`qingci-plugin-sdk>=1.0`）。

## 演示能力

| 命令 | 说明 |
|---|---|
| `/hello`（别名 `/hi`、`/你好`） | 打个招呼 |
| `/greet zh` / `/greet en` | 子指令示例 |
| `/weather <城市> <天数>` | 类型化参数示例 |

另演示：i18n 国际化、全局生命周期钩子（`on_startup`/`on_shutdown`/`on_bot_connect`/`on_metaevent`）、`@llm_tool` LLM 工具声明（`get_time` / `echo`）、插件数据目录 `self.data_dir`。

## 开发

插件模板见 [Plugins-SDK](https://github.com/Qingci-Bot/Plugins-SDK) 仓库 `plugins/_template/`；SDK API 文档见 [README](https://github.com/Qingci-Bot/Plugins-SDK)。

## 许可

GPL-3.0-or-later
