# Hoop Windows Bundle

Thin Amplifier bundle optimized for Windows development with PowerShell. It follows the recommended pattern from the [Amplifier bundle guide](https://github.com/microsoft/amplifier-foundation/blob/main/docs/BUNDLE_GUIDE.md): a minimal root bundle that includes foundation and its own behavior.

## What's Included

- **Root bundle** (`bundle.md`): Thin entry point that includes foundation and this repo's behavior.
- **Behavior** (`behaviors/hoop-windows.yaml`): Composes PowerShell dev tooling, Deepwiki, and Perplexity provider configuration.
- **Context** (`context/instructions.md`): Single source of instructions for the bundle.

## Usage

1. Ensure you have the Amplifier CLI available.
2. Set required secrets:
   ```bash
   export PERPLEXITY_API_KEY=your_key_here
   ```
3. Load the bundle:
   ```bash
   amplifier session start --bundle git+https://github.com/hoopsomuah/hoop-windows@main
   ```

The bundle pulls:
- Foundation defaults
- PowerShell development behavior
- Deepwiki behavior
- Perplexity provider (defaults to `sonar-pro`)

## Conventions

- Keep the root bundle thin—add new capabilities via behaviors.
- Place reusable capabilities in `behaviors/`.
- Put shared instructions in `context/` and reference them from both the bundle and behaviors.
