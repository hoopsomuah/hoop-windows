bundle:
  name: hoop-windows
  version: 1.0.0
  description: Personal Windows development bundle with PowerShell

includes:
  - bundle: git+https://github.com/microsoft/amplifier-foundation@main
  - bundle: hoop-windows:behaviors/hoop-windows
---

# Hoop Windows Development Bundle

Personal development bundle optimized for Windows with PowerShell as the primary shell. Uses a thin bundle pattern with behavior-driven composition.

@hoop-windows:context/instructions.md

---

@foundation:context/shared/common-system-base.md
