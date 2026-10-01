# 安装指南

<a href="https://ko-fi.com/0xp0co"><img src="https://img.shields.io/badge/Ko--fi-Support-FF6433?style=for-the-badge&logo=kofi&logoColor=white" alt="在 Ko-fi 上支持 Kylin Core"></a>

如果您觉得这个项目对您有所帮助，请考虑支持它的持续开发。感谢您的支持！

## 环境要求

- 已破解的 PS5，需具备可用的 ELF 加载器
- 已安装 [PS5 Payload Manager (PLDMGR)](https://github.com/itsPLK/ps5-payload-manager)

## 所需文件

| 文件 | 说明 |
|---|---|
| `kylin-core.elf` | payload 本体，包含守护进程、金手指引擎与网页界面 |

## 安装步骤

1. 用 **PS5 Payload Manager (PLDMGR)** 加载 `kylin-core.elf`

2. 等待就绪通知。**Kylin Core** 入口就在主屏幕的**媒体**分类下

3. 从主屏幕启动 **Kylin Core**

> [!IMPORTANT]
> 启动应用前必须先通过 PLDMGR 加载 `kylin-core.elf`，否则 UI 无法正常显示。

如果主屏幕上始终没有出现入口，请检查 `/data/kylin/logs/kylin-core.log`。

## 金手指文件

将金手指文件（`.json`、`.shn`、`.mc4`、`.ShnExt`）放入：

```
/data/kylin/cheats
```

- 仅支持扁平目录，不支持子文件夹
- 工具会自动检测当前运行的游戏并匹配可用金手指
- `.ShnExt` 属于 Alpha，尚未完全支持；`.json`、`.shn`、`.mc4` 是完整支持的格式

## 卸载

1. 停止 payload（重启主机，或在界面里结束守护进程）
2. 从主屏幕删除 **Kylin Core** 入口（Options → 删除）
3. 如不再需要，删除 `/data/kylin` 目录
