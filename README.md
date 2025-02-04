# AstroNvim Mason Registry

A community driven package registry for <a href="https://github.com/williamboman/mason.nvim"><code>mason.nvim</code></a>

Refer to [CONTRIBUTING.md](./CONTRIBUTING.md) for contribution guidelines.

Compiled registry contents are available via [releases](https://github.com/mason-org/mason-registry/releases).

## Usage

To use this registry you simply need to add the string `"github:AstroNvim/mason-registry"` to the `registries` list of
the `mason.nvim` configuration that is passed to the `require("mason").setup()` function.

**Lazy.nvim**

```lua
return {
    "williamboman/mason.nvim",
    opts = {
        registries = {
            -- default Mason registry has highest priority
            "github:mason-org/mason-registry",
            -- Add the AstroNvim mason registry
            "github:AstroNvim/mason-registry",
        },
    },
}
```
