---
_build:
  publishResources: false
  render: never
  list: never

name: "Enable Fast Jsg Struct"
sort_date: "2025-12-03"
enable_flag: "enable_fast_jsg_struct"
disable_flag: "disable_fast_jsg_struct"
---

Enables the fast `jsg::Struct` optimization. With this enabled, `JSG_STRUCTS` will use a more efficient creation pattern that reduces construction time. However, optional fields will be explicitly set to `undefined` rather than being omitted, which is an observable behavior change.