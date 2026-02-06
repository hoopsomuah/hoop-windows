# Hoop Windows Development Instructions

This bundle is designed for Windows-based development with PowerShell as the primary shell. It composes capabilities for local development, deep knowledge retrieval, and Perplexity search.

## Capabilities

- **PowerShell Development**: Inherits PowerShell-first tooling from the pwsh dev bundle.
- **Deep Knowledge Retrieval**: Deepwiki integration for exploring and summarizing knowledge bases.
- **Perplexity Search**: Perplexity provider configured for concise, high-quality search responses (requires `PERPLEXITY_API_KEY`).

## Usage Notes

- Ensure the `PERPLEXITY_API_KEY` environment variable is set before running sessions.
- Prefer Windows Terminal with PowerShell for the best experience.
- Keep this bundle thin—additional capabilities should be added via behaviors rather than modifying the root bundle.

## Included Behaviors

- `hoop-windows:behaviors/hoop-windows` — composes the upstream behaviors and provider configuration for Perplexity.
