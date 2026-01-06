---
_build:
  publishResources: false
  render: never
  list: never

name: "Remove Node.js Compat EOL features - v22"
enable_flag: "remove_nodejs_compat_eol_v22"
disable_flag: "add_nodejs_compat_eol_v22"
---

Removes APIs that reached end-of-life in Node.js 22.x. When using the `removeNodejsCompatEOL` flag, this will default enable on/after 2027-04-30.