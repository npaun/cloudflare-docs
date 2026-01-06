---
_build:
  publishResources: false
  render: never
  list: never

name: "Remove Node.js Compat EOL features - v24"
enable_flag: "remove_nodejs_compat_eol_v24"
disable_flag: "add_nodejs_compat_eol_v24"
---

Removes APIs that reached end-of-life in Node.js 24.x. When using the `removeNodejsCompatEOL` flag, this will default enable on/after 2028-04-30.