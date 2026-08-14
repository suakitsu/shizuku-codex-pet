# Sawatari Shizuku Codex Pets and Windows Skin

<p align="center">
  <a href="./README.md">中文</a> · <strong>English</strong>
</p>

<p align="center">
  Three animated Codex Desktop v2 pets + a forget-me-not Windows theme<br>
  Independent installs · Native interactions · Transparent pet support · Complete appearance restore
</p>

> Unofficial, non-commercial fan project. This project is not affiliated with, sponsored by, or endorsed by OpenAI, Codex, ωstar, or the character rights holders.

## What this repository provides

| Component | Included | Platform | Location |
| --- | --- | --- | --- |
| Codex v2 pets | Full-body expressive, pixel, and Q-style editions | Environments that support Codex Desktop v2 pets | Source files in `pets/` + the `v1.0.0` release |
| Shizuku Windows skin | Hero artwork, forget-me-not palette, signature, flower mark, and bottom-right polaroid | Windows 10/11 | Standalone installer in the `skin-v1.0.0` release |

The default branch contains the three pet source folders and project documentation. The Windows skin's installer, theme files, tests, and asset notice are packaged in a standalone release ZIP. The pets and skin do not depend on each other, so either component can be installed by itself.

## Downloads

| Component | Version | Files |
| --- | --- | --- |
| [Three pets](https://github.com/suakitsu/shizuku-codex-pet/releases/tag/v1.0.0) | v1.0.0 | `shizuku-codex-pets-v1.0.0.zip` and its `.sha256` file |
| [Windows skin](https://github.com/suakitsu/shizuku-codex-pet/releases/tag/skin-v1.0.0) | v1.0.0 | `Shizuku-Codex-Skin-Windows-v1.0.0.zip` and its `.sha256` file |

Download the named ZIP in the table, not GitHub's automatically generated Source code archive.

## Install the pets

All three pets use the Codex Desktop v2 sprite format and include the standard animations plus sixteen clockwise look directions:

| Folder | Display name | Style |
| --- | --- | --- |
| `shizuku` | Shizuku | Full-body expressive |
| `shizuku-pixel` | Shizuku · Pixel | Full-body pixel art |
| `shizuku-q` | Shizuku · Q | Super-deformed Q style |

1. Download and extract `shizuku-codex-pets-v1.0.0.zip`.
2. Copy the pet folders you want into `%USERPROFILE%\.codex\pets\`.
3. If `CODEX_HOME` is set, use `%CODEX_HOME%\pets\` instead.
4. Reopen the pet. If Codex Desktop was already running and does not refresh, restart Codex.

The directory should look like this. Keep each `pet.json` and `spritesheet.webp` together in the same folder.

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

## Install the Windows skin

The skin is based on [Fei-Away/Codex-Dream-Skin](https://github.com/Fei-Away/Codex-Dream-Skin) and targets the official Microsoft Store Codex desktop app. It coordinates the sidebar, title bar, cards, composer, menus, editor, and terminal while keeping native controls interactive and preventing an opaque theme background from appearing behind `/avatar-overlay` pet windows.

### Requirements

- Windows 10/11
- Official Microsoft Store Codex desktop app
- Node.js 22 or newer
- Close Codex before installation

### Install and restore

1. Download and fully extract `Shizuku-Codex-Skin-Windows-v1.0.0.zip`.
2. Double-click `Install Shizuku Codex Skin.cmd`.
3. Approve the Codex restart when prompted.
4. Use the desktop `Shizuku Codex Skin` shortcut afterward.

The installer backs up the relevant appearance configuration first. To restore the official appearance, double-click `Restore Shizuku Codex Skin.cmd` or use the desktop `Shizuku Codex Skin - Restore` shortcut.

### Safety scope

- CDP binds only to the local loopback address `127.0.0.1`.
- The installer does not modify WindowsApps, `app.asar`, the official package, or its code signature.
- It does not modify API keys, Base URLs, accounts, chats, projects, or pet files.
- Avoid running untrusted local software while the skin is active.

## Verify a download

Each release includes a matching `.sha256` file. Run the following in PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 .\Shizuku-Codex-Skin-Windows-v1.0.0.zip
Get-Content .\Shizuku-Codex-Skin-Windows-v1.0.0.zip.sha256
```

The two hashes must match exactly. Use the same process for the pets archive.

## Repository layout

```text
.
├── pets/                 # Source files for the three Codex v2 pets
├── ASSET_LICENSE.md      # Pet artwork terms and third-party rights exclusions
├── LICENSE               # Repository code and documentation license
├── README.md             # Chinese documentation
└── README.en.md          # English documentation
```

## Notice and licenses

Sawatari Shizuku, the title, character design, setting, trademarks, and all underlying franchise rights belong to their respective rights holders. This repository does not claim or license those rights.

The repository does not contain official reference images, game-extracted assets, official logos, commercial game files, generation logs, prompts, or private working records. See [ASSET_LICENSE.md](ASSET_LICENSE.md) for the pet artwork terms and third-party rights exclusions. Character artwork in the skin is governed by the `ASSET_LICENSE.md` inside its ZIP. See [LICENSE](LICENSE) for the repository code and documentation license.
