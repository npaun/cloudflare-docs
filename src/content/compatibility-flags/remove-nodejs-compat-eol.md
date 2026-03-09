---
_build:
  publishResources: false
  render: never
  list: never

name: "Remove Nodejs Compat Eol"
sort_date: "2025-09-01"
enable_flag: "remove_nodejs_compat_eol"
disable_flag: "add_nodejs_compat_eol"
---

Removes the Node.js compatibility layer for EOL versions of Node.js. When the flag is enabled, APIs that have reached End-of-Life in Node.js will be removed for workers. When disabled, the APIs are present (but might still be non-functional stubs) This flag is intended to be a roll-up flag. That is, as additional APIs reach EOL, new compat flags will be added for those that will have `impliedByAfterDate(name = "removeNodeJsCompatEOL", ...` annotations.
