# 安装指南

<a href="https://ko-fi.com/kylincore"><img src="https://img.shields.io/badge/Ko--fi-Support-FF6433?style=for-the-badge&logo=kofi&logoColor=white" alt="在 Ko-fi 上支持 Kylin Core"></a>

如果您觉得这个项目对您有所帮助，请考虑支持它的持续开发。感谢您的支持！

## 环境要求

- 已破解的 PS5，需具备可用的 ELF 加载器
- 已安装 [PS5 Payload Manager (PLDMGR)](https://github.com/itsPLK/ps5-payload-manager)

## 所需文件

| 文件 | 说明 |
|---|---|
| `kylin-core.elf` | Payload 二进制，通过 PLDMGR 加载 |
| `IV0000-KYLN00003_00-KYLINCORELAUNCHR_GAME_SECTION.pkg` | 系统应用安装包 — 安装后 Launcher 显示在 **游戏** 分类下 |
| `IV0000-KYLN00003_00-KYLINCORELAUNCHR_MEDIA_SECTION.pkg` | 系统应用安装包 — 安装后 Launcher 显示在 **媒体** 分类下 |

> [!NOTE]
> 根据你希望 Launcher 出现在主屏幕的哪个位置，选择**其中一个** PKG 安装即可。

## 安装步骤

1. 将 `kylin-core.elf` 和你选择的 `.pkg` 文件复制到 U 盘根目录

2. 将 U 盘插入 PS5

3. 打开 **PS5 Payload Manager (PLDMGR)**，加载 `kylin-core.elf`

4. 进入 **设置 → 调试设置**，安装 `.pkg` 文件

5. 从主屏幕启动 **Kylin Core**

> [!IMPORTANT]
> 启动应用前必须先通过 PLDMGR 加载 `kylin-core.elf`，否则 UI 无法正常显示。

## 金手指文件

将金手指文件（`.shn`、`.mc4`、`.json`）放入：

```
/data/kylin/cheats
```

- 仅支持扁平目录，不支持子文件夹
- 工具会自动检测当前运行的游戏并匹配可用金手指

## 卸载

1. 从主屏幕删除应用（Options → 删除）
2. 如不再需要，删除 `/data/kylin/cheats` 目录
