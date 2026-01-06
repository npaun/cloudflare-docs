---
_build:
  publishResources: false
  render: never
  list: never

name: "Enable Node.js punycode module"
enable_flag: "enable_nodejs_punycode_module"
disable_flag: "disable_nodejs_punycode_module"
---

Enables the Node.js deprecated `punycode` module. It is required to use this flag with `nodejs_compat` (or `nodejs_compat_v2`).