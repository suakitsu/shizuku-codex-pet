# 沢渡雫 Codex 桌宠与 Windows 皮肤

<p align="center">
  <strong>中文</strong> · <a href="./README.en.md">English</a>
</p>

<p align="center">
  三套 Codex Desktop v2 动画桌宠 + 一套 Windows 勿忘草主题<br>
  可独立安装 · 原生交互 · 透明桌宠兼容 · 外观可完整恢复
</p>

> 非官方、非商业同人项目。本项目与 OpenAI、Codex、ωstar 及角色权利人没有隶属、赞助或官方合作关系。

## 这个仓库提供什么

| 内容 | 包含 | 平台 | 存放位置 |
| --- | --- | --- | --- |
| Codex v2 桌宠 | 全身表现版、像素版、Q 版 | 支持 Codex Desktop v2 桌宠的环境 | `pets/` 源文件 + `v1.0.0` Release |
| Shizuku Windows 皮肤 | 主视觉、勿忘草配色、签名、花朵标识和右下角相框 | Windows 10/11 | `skin-v1.0.0` Release 独立安装包 |

仓库主分支保存三套桌宠源文件和项目文档。Windows 皮肤的安装脚本、主题文件、测试和素材声明封装在独立 Release ZIP 中。桌宠和皮肤互不依赖，可以只安装其中一项。

## 下载

| 项目 | 版本 | 下载内容 |
| --- | --- | --- |
| [三套桌宠](https://github.com/suakitsu/shizuku-codex-pet/releases/tag/v1.0.0) | v1.0.0 | `shizuku-codex-pets-v1.0.0.zip` 及其 `.sha256` |
| [Windows 皮肤](https://github.com/suakitsu/shizuku-codex-pet/releases/tag/skin-v1.0.0) | v1.0.0 | `Shizuku-Codex-Skin-Windows-v1.0.0.zip` 及其 `.sha256` |

请下载表格中命名明确的 ZIP，不要下载 GitHub 自动生成的 Source code 压缩包。

## 安装桌宠

三套桌宠均使用 Codex Desktop v2 精灵格式，包含标准动作和顺时针十六向注视：

| 文件夹 | 显示名称 | 风格 |
| --- | --- | --- |
| `shizuku` | Shizuku | 全身表现版 |
| `shizuku-pixel` | Shizuku · Pixel | 全身像素版 |
| `shizuku-q` | Shizuku · Q | Q 版 |

1. 下载并解压 `shizuku-codex-pets-v1.0.0.zip`。
2. 将需要的宠物文件夹复制到 `%USERPROFILE%\.codex\pets\`。
3. 如果设置了 `CODEX_HOME`，改用 `%CODEX_HOME%\pets\`。
4. 重新打开桌宠；如果 Codex Desktop 已经运行但没有刷新，请重启 Codex。

正确的目录结构如下。不要拆散同一文件夹内的 `pet.json` 和 `spritesheet.webp`。

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

## 安装 Windows 皮肤

皮肤基于 [Fei-Away/Codex-Dream-Skin](https://github.com/Fei-Away/Codex-Dream-Skin)，用于 Microsoft Store 官方 Codex 桌面应用。它统一侧栏、标题栏、卡片、输入框、菜单、编辑器和终端配色，同时保持原生控件可交互，并避免给 `/avatar-overlay` 桌宠窗口添加不透明主题背景。

### 系统要求

- Windows 10/11
- Microsoft Store 官方 Codex 桌面应用
- Node.js 22 或更新版本
- 安装前关闭 Codex

### 安装与恢复

1. 下载并完整解压 `Shizuku-Codex-Skin-Windows-v1.0.0.zip`。
2. 双击 `Install Shizuku Codex Skin.cmd`。
3. 按提示允许 Codex 重启。
4. 后续通过桌面的 `Shizuku Codex Skin` 快捷方式启动。

安装脚本会先备份相关外观配置。需要恢复官方外观时，双击 `Restore Shizuku Codex Skin.cmd`，或使用桌面的 `Shizuku Codex Skin - Restore` 快捷方式。

### 安全范围

- CDP 仅绑定本机回环地址 `127.0.0.1`。
- 不修改 WindowsApps、`app.asar`、官方安装包或代码签名。
- 不修改 API Key、Base URL、账号、对话、项目或桌宠文件。
- 皮肤运行期间不要同时运行来源不明的本机程序。

## 校验下载文件

每个 Release 都提供对应的 `.sha256` 文件。在 PowerShell 中运行：

```powershell
Get-FileHash -Algorithm SHA256 .\Shizuku-Codex-Skin-Windows-v1.0.0.zip
Get-Content .\Shizuku-Codex-Skin-Windows-v1.0.0.zip.sha256
```

两处哈希值应完全一致。桌宠压缩包可以使用相同方法校验。

## 仓库结构

```text
.
├── pets/                 # 三套 Codex v2 桌宠源文件
├── ASSET_LICENSE.md      # 桌宠视觉素材许可与第三方权利排除
├── LICENSE               # 仓库代码和文档许可
├── README.md             # 中文说明
└── README.en.md          # English documentation
```

## 声明与许可

沢渡雫、作品名称、角色设计、设定、商标及其他原作权利归各自权利方所有，本仓库不主张这些权利，也不对其进行授权。

仓库不包含官方参考图、游戏提取素材、官方标志、商业游戏文件、生成日志、提示词或私人制作记录。桌宠视觉素材的许可范围及第三方权利排除见 [ASSET_LICENSE.md](ASSET_LICENSE.md)；皮肤角色素材受其 ZIP 内的 `ASSET_LICENSE.md` 约束；仓库代码和文档许可见 [LICENSE](LICENSE)。
