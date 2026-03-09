---
_build:
  publishResources: false
  render: never
  list: never

name: "Remove Nodejs Compat Eol V23"
sort_date: "2025-09-01"
enable_flag: "remove_nodejs_compat_eol_v23"
disable_flag: "add_nodejs_compat_eol_v23"
---

Removes APIs that reached end-of-life in Node.js 23.x. This will default enable when the removeNodejsCompatEOLv24 flag is enabled after 2025-09-01. Went EOL on 2025-06-01
