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

```
# TODO
```

* Update scoop and tools
```powershell
scoop update && scoop update --all && scoop cleanup --all --cache
```

## How do I contribute new tools?

To make a new manifest contribution, please read the [Contributing
Guide](https://github.com/ScoopInstaller/.github/blob/main/.github/CONTRIBUTING.md)
and [App Manifests](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests)
wiki page.
