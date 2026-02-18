---
title: Biome
description: "Configure Biome language support in Zed, including language servers, formatting, and debugging."
---

# Biome

[Biome](https://biomejs.dev/) support in Zed is provided by the community-maintained [Biome extension](https://github.com/biomejs/biome-zed).
Report issues to: [https://github.com/biomejs/biome-zed/issues](https://github.com/biomejs/biome-zed/issues)

- Language Server: [biomejs/biome](https://github.com/biomejs/biome)

## Supported Languages

The Biome extension includes support for the following languages:

- JavaScript
- TypeScript
- JSX
- TSX
- JSON
- JSONC
- Vue.js
- Astro
- Svelte
- CSS

## Configuration

Create `biome.json` in the root directory of the workspace with this settings:

```json [settings]
{
  "$schema": "https://biomejs.dev/schemas/1.8.3/schema.json"
}
```

For a full list of configuration options, see [Biome Configuration](https://biomejs.dev/reference/configuration/) documentation.

### Features

See the [Biome Zed Extension Reference](https://biomejs.dev/reference/zed/) for a complete list of editing features and configuration options.
