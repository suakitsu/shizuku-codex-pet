# 沢渡雫 Codex 桌宠与 Windows 皮肤

以《美少女万華鏡 -忘れな草と永遠の少女-》沢渡雫为灵感制作的非官方、非商业 Codex Desktop 定制项目。本仓库提供三套 v2 动画桌宠，并托管配套的 Windows 勿忘草主题发布包。

## 下载

- [桌宠 v1.0.0](https://github.com/suakitsu/shizuku-codex-pet/releases/tag/v1.0.0)：`shizuku-codex-pets-v1.0.0.zip`
- [Windows 皮肤 v1.0.0](https://github.com/suakitsu/shizuku-codex-pet/releases/tag/skin-v1.0.0)：`Shizuku-Codex-Skin-Windows-v1.0.0.zip`

请下载 Release 中命名明确的 ZIP，不要下载 GitHub 自动生成的 Source code 包。桌宠与皮肤可以独立使用。

## 桌宠

| 文件夹 | 版本 |
| --- | --- |
| `shizuku` | 全身表现版 |
| `shizuku-pixel` | 像素版 |
| `shizuku-q` | Q 版 |

三套均包含 Codex v2 标准动作与顺时针十六向注视。

### 安装桌宠

解压 `shizuku-codex-pets-v1.0.0.zip`，把其中三个宠物文件夹复制到：

```text
%USERPROFILE%\.codex\pets\
```

如果设置了 `CODEX_HOME`，请复制到 `%CODEX_HOME%\pets\`。正确结构为：

```text
.codex/pets/
├── shizuku/
│   ├── pet.json
│   └── spritesheet.webp
├── shizuku-pixel/
│   ├── pet.json
│   └── spritesheet.webp
└── shizuku-q/
    ├── pet.json
    └── spritesheet.webp
```

安装时不要拆散同一文件夹内的 `pet.json` 与 `spritesheet.webp`。如果 Codex Desktop 已经打开，请重新打开桌宠或重启 Codex。

## Windows 皮肤

皮肤基于 [Fei-Away/Codex-Dream-Skin](https://github.com/Fei-Away/Codex-Dream-Skin)，提供沢渡雫横向主视觉、勿忘草配色、签名、花朵标识和相框，同时保留 Codex 原生交互与透明桌宠窗口。

### 系统要求

- Windows 10/11
- Microsoft Store 官方 Codex 桌面应用
- Node.js 22 或更新版本
- 安装时先关闭 Codex

### 安装皮肤

1. 完整解压 `Shizuku-Codex-Skin-Windows-v1.0.0.zip`。
2. 双击 `Install Shizuku Codex Skin.cmd`。
3. 按提示允许 Codex 重启。
4. 后续使用桌面的 `Shizuku Codex Skin` 快捷方式启动。

安装脚本会先备份相关 Codex 外观配置；不会修改 API Key、Base URL、账号、对话、项目或宠物文件。需要恢复官方外观时，双击 `Restore Shizuku Codex Skin.cmd`，或使用桌面的 `Shizuku Codex Skin - Restore` 快捷方式。

## 声明与许可

这是非官方、非商业同人项目，与 OpenAI、Codex、ωstar、原作作者及其他权利方无隶属或授权关系。沢渡雫、作品名称、角色设计、设定、商标及其他原作权利归各自权利方所有，本仓库不主张这些权利，也不对其进行授权。

仓库不包含官方参考图、游戏提取素材、官方标志、商业游戏文件、生成日志、提示词或私人制作记录。桌宠视觉素材的许可范围及原作权利排除条款见 [ASSET_LICENSE.md](ASSET_LICENSE.md)；皮肤角色素材受其 ZIP 内的 `ASSET_LICENSE.md` 约束；文档许可见 [LICENSE](LICENSE)。

English: [README.en.md](README.en.md)
