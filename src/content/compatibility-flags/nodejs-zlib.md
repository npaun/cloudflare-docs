---
_build:
  publishResources: false
  render: never
  list: never

name: "Node.js Zlib module"
enable_flag: "nodejs_zlib"
disable_flag: "no_nodejs_zlib"
---

Enables `node:zlib` implementation. Automatically enabled when `nodejs_compat` is set.