---
_build:
  publishResources: false
  render: never
  list: never

name: "Nodejs Compat V2"
sort_date: "2024-09-23"
enable_flag: "nodejs_compat_v2"
disable_flag: "no_nodejs_compat_v2"
---

Implies nodeJSCompat with the following additional modifications: * Node.js Compat built-ins may be imported/required with or without the node: prefix * Node.js Compat the globals Buffer and process are available everywhere
