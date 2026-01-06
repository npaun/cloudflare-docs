---
_build:
  publishResources: false
  render: never
  list: never

name: "Python Workers force new vendor path"
sort_date: "2025-08-11"
enable_flag: "python_workers_force_new_vendor_path"
---

Disables adding `/session/metadata/vendor` to the Python Worker's `sys.path`. So Workers using this flag will have to place their vendored modules in a `python_modules` directory.