# Scoop Bucket for Virtual Pinball

[![License](https://img.shields.io/github/license/gitfool/scoop-vpinball?color=blue&label=License&logo=github)](LICENSE)
[![Tests](https://img.shields.io/github/actions/workflow/status/gitfool/scoop-vpinball/ci.yml?branch=main&label=Tests&logo=github)](https://github.com/gitfool/scoop-vpinball/actions/workflows/ci.yml)
[![Excavator](https://img.shields.io/github/actions/workflow/status/gitfool/scoop-vpinball/excavator.yml?branch=main&label=Excavator&logo=github)](https://github.com/gitfool/scoop-vpinball/actions/workflows/excavator.yml)

## How do I install apps?

* Install [scoop](https://scoop.sh) ([FAQ](https://github.com/ScoopInstaller/Scoop/wiki/FAQ)) using a non-elevated [PowerShell](https://github.com/PowerShell/PowerShell):
```pwsh
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

* Add scoop [bucket](https://github.com/ScoopInstaller/Scoop/wiki/Buckets):
```pwsh
scoop bucket add vpinball https://github.com/gitfool/scoop-vpinball
```

* Install apps via scoop [cli](https://github.com/ScoopInstaller/Scoop/wiki/Commands):

| Name | Description | Command | Version |
| --- | --- | --- | --- |
| [vpinball](https://github.com/vpinball/vpinball) | Visual Pinball BGFX<sup>1</sup> | `scoop install vpinball` | [![Version](https://img.shields.io/scoop/v/vpinball?bucket=https%3A%2F%2Fgithub.com%2Fgitfool%2Fscoop-vpinball&label=&logo=scoop)](bucket/vpinball.json) |
| [vpinball-nightly](https://nightly.link/vpinball/vpinball/workflows/vpinball/master?preview) | Visual Pinball BGFX<sup>1</sup> nightly<sup>2</sup> | `scoop install vpinball-nightly` | [![Version](https://img.shields.io/scoop/v/vpinball-nightly?bucket=https%3A%2F%2Fgithub.com%2Fgitfool%2Fscoop-vpinball&label=&logo=scoop)](bucket/vpinball-nightly.json) |
| [vpxtool](https://github.com/francisdb/vpxtool) | Terminal based frontend and utilities for Visual Pinball | `scoop install vpxtool` | [![Version](https://img.shields.io/scoop/v/vpxtool?bucket=https%3A%2F%2Fgithub.com%2Fgitfool%2Fscoop-vpinball&label=&logo=scoop)](bucket/vpxtool.json) |

<sup>1</sup> [BGFX](https://github.com/dekay/vpinball-wiki/wiki/About-Visual-Pinball#bgfx) x64 release only

<sup>2</sup> Requires GitHub login

## How do I update apps?

* Update scoop and apps
```powershell
scoop update && scoop update --all && scoop cleanup --all --cache
```
