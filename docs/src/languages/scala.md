---
title: Scala
description: "Configure Scala language support in Zed, including language servers, formatting, and debugging."
---

# Scala

Scala language support in Zed is provided by the community-maintained [Scala extension](https://github.com/scalameta/metals-zed).
Report issues to: [https://github.com/scalameta/metals-zed/issues](https://github.com/scalameta/metals-zed/issues)

- Tree-sitter: [tree-sitter/tree-sitter-scala](https://github.com/tree-sitter/tree-sitter-scala)
- Language Server: [scalameta/metals](https://github.com/scalameta/metals)

## Setup

Install Scala with `cs setup` (Coursier):

```sh
# macOS with Homebrew
brew install coursier/formulas/coursier && cs setup
```

For other operating systems, see Scala [installation documentation](https://www.scala-lang.org/download/).

### REPL (Almond) Setup Instructions

```sh
# macOS with Homebrew
# Eclipse foundation official OpenJDK binaries
brew install --cask temurin

brew install coursier/formulas/coursier && cs setup

coursier launch --use-bootstrap almond -- --install
```

For more installation guide, visit [almond installation documentation](https://almond.sh/docs/quick-start-install).

## Configuration

Behavior of the Metals language server can be controlled with:

- `.scalafix.conf` file - See [Scalafix Configuration](https://scalacenter.github.io/scalafix/docs/users/configuration.html)
- `.scalafmt.conf` file - See [Scalafmt Configuration](https://scalameta.org/scalafmt/docs/configuration.html)

You can place these files in the root of your project or specifying their location in the Metals configuration. See [Metals User Configuration](https://scalameta.org/metals/docs/editors/user-configuration) for more.

<!--
TBD: Provide LSP configuration example for metals in Zed settings.json. metals.{javaHome,excludedPackages,customProjectRoot} etc.
-->
