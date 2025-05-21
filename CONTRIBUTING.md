# Contributing to LOLBAS-Hardening-Community

We welcome your submissions! Whether it's a new rule, correction, or platform-specific consideration — your help strengthens the community.

## Submission Guidelines

- Submit PowerShell-based blocking rules under the `submissions/` directory
- Each submission must:
  - Be named clearly (e.g., `Block-cmstp.ps1`)
  - Include comments explaining:
    - Binary targeted
    - Why it’s safe to block
    - How it was tested

## Example Rule Comment Format

```powershell
<#
Target: cmstp.exe
Reason: LOLBAS binary used for execution and bypass
Safe to block? Yes - used only in rare enterprise VPN setups
Tested on: Windows 10 21H2, Windows 11 23H2
#>
```

## Validation Checklist (include in your Pull Request)

- [ ] Rule follows naming convention
- [ ] Binary is not critical for standard operation
- [ ] Works on latest Windows versions
- [ ] Peer-reviewed or approved by another community member

Thanks for contributing!
