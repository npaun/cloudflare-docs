---
_build:
  publishResources: false
  render: never
  list: never

name: "Enable Node.js cluster module"
enable_flag: "enable_nodejs_cluster_module"
disable_flag: "disable_nodejs_cluster_module"
---

Enables the Node.js non-functional stub `cluster` module. It is required to use this flag with `nodejs_compat` (or `nodejs_compat_v2`).