---
_build:
  publishResources: false
  render: never
  list: never

name: "Enable Node.js wasi module"
enable_flag: "enable_nodejs_wasi_module"
disable_flag: "disable_nodejs_wasi_module"
---

Enables the Node.js non-functional stub `wasi` module. It is required to use this flag with `nodejs_compat` (or `nodejs_compat_v2`).