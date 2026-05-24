# RiskManager 4.2.1 Build Info

## Target

- Product: RiskManager Pro
- Version: 4.2.1
- ATAS target: 8.x
- Target framework: historical single-target release

## Original build

```powershell
dotnet build "RiskManager 4.0\src\RiskManager.csproj" -c Release
```

## Current output

```text
release-archive\正式版\8.x\RiskManager-4.2.1\RiskManager-4.2.1-ATAS-8.x.dll
```

## Migration note

This file was migrated from the historical product-version archive path:

```text
release-archive\正式版\4.2\RiskManager-4.2.1\
```

The original protected DLL content is preserved; only the archive path and DLL filename were normalized.
