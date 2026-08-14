# Sawatari Shizuku Codex Pets and Windows Skin

An unofficial, non-commercial Codex Desktop customization project inspired by Sawatari Shizuku from *Bishoujo Mangekyou -Wasurenagusa to Eien no Shoujo-*. This repository provides three animated v2 pets and hosts the companion forget-me-not Windows skin release.

## Downloads

- [Pets v1.0.0](https://github.com/suakitsu/shizuku-codex-pet/releases/tag/v1.0.0): `shizuku-codex-pets-v1.0.0.zip`
- [Windows skin v1.0.0](https://github.com/suakitsu/shizuku-codex-pet/releases/tag/skin-v1.0.0): `Shizuku-Codex-Skin-Windows-v1.0.0.zip`

Download the named ZIP from the relevant release, not GitHub's automatic Source code archive. The pets and skin work independently.

## Pets

| Folder | Edition |
| --- | --- |
| `shizuku` | Full-body expressive |
| `shizuku-pixel` | Pixel |
| `shizuku-q` | Super-deformed Q style |

All three pets include the standard Codex v2 animations and sixteen clockwise look directions.

### Install the pets

Extract `shizuku-codex-pets-v1.0.0.zip`, then copy the `shizuku`, `shizuku-pixel`, and `shizuku-q` folders into:

```text
%USERPROFILE%\.codex\pets\
```

If `CODEX_HOME` is set, use `%CODEX_HOME%\pets\` instead. Keep `pet.json` and `spritesheet.webp` together inside each pet folder. Reopen the pet or restart Codex Desktop after installing.

## Windows skin

The skin is based on [Fei-Away/Codex-Dream-Skin](https://github.com/Fei-Away/Codex-Dream-Skin). It adds Shizuku hero artwork, a forget-me-not palette, signature, flower mark, and polaroid while preserving native Codex interactions and transparent pet windows.

### Requirements

- Windows 10/11
- Official Microsoft Store Codex desktop app
- Node.js 22 or newer
- Close Codex before installation

### Install the skin

1. Extract `Shizuku-Codex-Skin-Windows-v1.0.0.zip` completely.
2. Double-click `Install Shizuku Codex Skin.cmd`.
3. Approve the Codex restart when prompted.
4. Use the desktop `Shizuku Codex Skin` shortcut afterward.

The installer backs up the relevant appearance configuration. It does not modify API keys, Base URLs, accounts, chats, projects, or pet files. To restore the official appearance, double-click `Restore Shizuku Codex Skin.cmd` or use the desktop `Shizuku Codex Skin - Restore` shortcut.

## Notice and licenses

This is an unofficial, non-commercial fan project. It is not affiliated with or endorsed by OpenAI, Codex, ωstar, the original creators, or other rights holders. Sawatari Shizuku, the title, character design, setting, trademarks, and all underlying franchise rights belong to their respective owners and are not licensed by this repository.

No official reference images, game-extracted assets, official logos, commercial game files, generation logs, prompts, or private working records are included in the repository. See [ASSET_LICENSE.md](ASSET_LICENSE.md) for the pet visual asset terms and exclusions. Character artwork in the skin is governed by the `ASSET_LICENSE.md` inside its ZIP. See [LICENSE](LICENSE) for the documentation license.

中文说明：[README.md](README.md)
