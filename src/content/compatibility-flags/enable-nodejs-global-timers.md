---
_build:
  publishResources: false
  render: never
  list: never

name: "Enable Nodejs Global Timers"
sort_date: "2026-02-10"
enable_flag: "enable_nodejs_global_timers"
disable_flag: "no_nodejs_global_timers"
---

When enabled, setTimeout, setInterval, clearTimeout, and clearInterval are available on globalThis as Node.js-compatible versions from node:timers. setTimeout and setInterval return Timeout objects with methods like refresh(), ref(), unref(), and hasRef(). This flag requires nodejs_compat or nodejs_compat_v2 to be enabled.
