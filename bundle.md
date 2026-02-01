---
bundle:
  name: hoop-windows
  version: 1.0.0
  description: Personal Windows development bundle with PowerShell

includes:
  - bundle: git+https://github.com/anokye-labs/amplifier-bundle-pwsh-dev@main
  - bundle: git+https://github.com/colombod/amplifier-bundle-deepwiki@main
  - bundle: git+https://github.com/colombod/amplifier-bundle-perplexity@main

providers:
  - module: provider-perplexity
    source: git+https://github.com/colombod/amplifier-module-provider-perplexity@main
    config:
      api_key: ${PERPLEXITY_API_KEY}
      default_model: sonar-pro
---

# Hoop Windows Development Bundle

Personal development bundle optimized for Windows with PowerShell as the primary shell.

---

@foundation:context/shared/common-system-base.md
