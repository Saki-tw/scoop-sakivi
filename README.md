# Scoop Bucket: SakiVI

[![Winget](https://img.shields.io/badge/winget-SakiStudio.SakiVI-blue?logo=windows)](https://github.com/microsoft/winget-pkgs/tree/master/manifests/s/SakiStudio/SakiVI)

Custom [Scoop](https://scoop.sh) bucket for [Vi-SakiWin64](https://github.com/Saki-tw/Vi-SakiWin64).

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

## Install — Scoop

```powershell
scoop bucket add sakivi https://github.com/Saki-tw/scoop-sakivi
scoop install saki-vi
vi file.txt   # ready to go
```

## Install — Winget（Recommended）

```powershell
winget install SakiStudio.SakiVI
vi file.txt
```

## About

Bill Joy's vi, recompiled for Windows. 178KB. That's it.

- **Author**: 咲ちゃん（Saki）/ Saki Studio — [saki-studio.com.tw](http://saki-studio.com.tw)
- **License**: GPL-2.0-only
