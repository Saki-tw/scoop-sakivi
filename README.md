# Scoop-SakiStudio

[![Winget](https://img.shields.io/badge/winget-SakiStudio.SakiVI-blue?logo=windows)](https://github.com/microsoft/winget-pkgs/tree/master/manifests/s/SakiStudio/SakiVI)

> **Saki Studio's Scoop Bucket** — because sometimes the main repository isn't ready for what's coming.

Custom [Scoop](https://scoop.sh) bucket for Saki Studio's Windows tools.

## Why a personal bucket?

This bucket exists because [ScoopInstaller/Main rejected Vi](https://github.com/ScoopInstaller/Main/pull/7643)
for not being "famous enough" — despite all automated checks passing ✅.

Meanwhile, [Microsoft Winget accepted it](https://github.com/microsoft/winget-pkgs/pull/339486) on first submission.

<details>
<summary>Scoop maintainer's exact words / 原文</summary>

> I suggest maintaining this in your [personal bucket](https://github.com/ScoopInstaller/Scoop/wiki/Buckets#creating-your-own-bucket) instead. Please feel free to reopen this PR once it fully meets the criteria.
>
> — [z-Fng](https://github.com/z-Fng), ScoopInstaller/Main [#7643](https://github.com/ScoopInstaller/Main/pull/7643)

</details>

Since then, the bucket has grown beyond Vi to host all Saki Studio tools for Windows.

---

## Available Packages

| Package | Description | Version |
|---------|-------------|---------|
| `saki-vi` | Vi — the original Vi, not Vim. Trilingual (繁中 / 日本語 / EN) | 1.0.0 |
| `sakiclip-hub` | SakiClip Hub — 跨裝置文字推送中繼站 | 2.0.0 |
| `sakiclip-client` | SakiClip Client — 跨裝置文字推送用戶端 | 2.0.0 |
| `sakiagentssh-daemon` | SakiAgentSSH Daemon — Agent-native gRPC execution daemon | 0.2.0 |
| `sakiagentssh-client` | SakiAgentSSH Client — Agent-native gRPC execution CLI | 0.2.0 |

---

## Install

### Vi — Scoop

```powershell
scoop bucket add sakistudio https://github.com/Saki-tw/Scoop-SakiStudio
scoop install saki-vi
vi file.txt   # ready to go
```

### Vi — Winget（Recommended）

```powershell
winget install SakiStudio.SakiVI
vi file.txt
```

### SakiClip

```powershell
scoop bucket add sakistudio https://github.com/Saki-tw/Scoop-SakiStudio
scoop install sakiclip-hub
scoop install sakiclip-client
```

### SakiAgentSSH

```powershell
scoop bucket add sakistudio https://github.com/Saki-tw/Scoop-SakiStudio
scoop install sakiagentssh-daemon
scoop install sakiagentssh-client
```

---

## Migration from scoop-sakivi

```powershell
scoop bucket rm sakivi
scoop bucket add sakistudio https://github.com/Saki-tw/Scoop-SakiStudio
```

GitHub auto-redirects from the old URL, but updating your local bucket is recommended.

---

## About

- **Vi**: Bill Joy's vi, recompiled for Windows. 178 KB. That's it.
- **SakiClip**: Cross-device text push & file relay. Hub runs the server, Client connects to it.
- **SakiAgentSSH**: Agent-native cross-machine execution over gRPC/HTTP2.

---

**Saki Studio** · [saki-studio.com.tw](http://saki-studio.com.tw) · [GitHub](https://github.com/saki-tw)
