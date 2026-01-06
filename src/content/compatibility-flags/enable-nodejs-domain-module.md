---
_build:
  publishResources: false
  render: never
  list: never

name: "Enable Node.js domain module"
enable_flag: "enable_nodejs_domain_module"
disable_flag: "disable_nodejs_domain_module"
---

Enables the Node.js non-functional stub `domain` module. It is required to use this flag with `nodejs_compat` (or `nodejs_compat_v2`).