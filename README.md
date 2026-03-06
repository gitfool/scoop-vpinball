# Scoop Bucket for Virtual Pinball Tools

[![Tests](https://github.com/gitfool/scoop-vpinball/actions/workflows/ci.yml/badge.svg)](https://github.com/gitfool/scoop-vpinball/actions/workflows/ci.yml) [![Excavator](https://github.com/gitfool/scoop-vpinball/actions/workflows/excavator.yml/badge.svg)](https://github.com/gitfool/scoop-vpinball/actions/workflows/excavator.yml)

## How do I install these tools?

* Install [scoop](https://scoop.sh) ([FAQ](https://github.com/ScoopInstaller/Scoop/wiki/FAQ)) using a non-elevated [PowerShell](https://github.com/PowerShell/PowerShell):
```pwsh
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

* Add this scoop [bucket](https://github.com/ScoopInstaller/Scoop/wiki/Buckets):
```pwsh
scoop bucket add vpinball https://github.com/gitfool/scoop-vpinball
```

* Install tools from this bucket:

| Name | Description | Command |
| --- | --- | --- |
| [vpinball](https://github.com/vpinball/vpinball) | Visual Pinball BGFX<sup>1</sup> | `scoop install vpinball` |
| [vpinball-nightly](https://nightly.link/vpinball/vpinball/workflows/vpinball/master?preview) | Visual Pinball BGFX<sup>1</sup> nightly<sup>2</sup> | `scoop install vpinball-nightly` |
| [vpxtool](https://github.com/francisdb/vpxtool) | Terminal based frontend and utilities for Visual Pinball | `scoop install vpxtool` |

<sup>1</sup> [BGFX](https://github.com/dekay/vpinball-wiki/wiki/About-Visual-Pinball#bgfx) x64 release only

<sup>2</sup> Requires GitHub login

## How do I update these tools?

* Update scoop and tools
```powershell
scoop update && scoop update --all && scoop cleanup --all --cache
```
