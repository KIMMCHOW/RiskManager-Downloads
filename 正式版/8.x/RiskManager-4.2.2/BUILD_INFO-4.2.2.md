# RiskManager 4.2.2 Build Info

## Target

- Product: RiskManager Pro
- Version: 4.2.2
- ATAS target: 8.x
- Target framework: net10.0-windows

## Build command

```powershell
powershell.exe -ExecutionPolicy Bypass -File .\scripts\build-atas-versions.ps1 -Version 4.2.2 -Protect
```

## Output

```text
release-archive\正式版\8.x\RiskManager-4.2.2\RiskManager-4.2.2.dll
```

## Protection

- Tool: Eziriz .NET Reactor
- Script: `scripts\protect-release.ps1`
- Formal release file name does not include `protected`.
