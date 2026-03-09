---
_build:
  publishResources: false
  render: never
  list: never

name: "Enable Nodejs Perf Hooks Module"
sort_date: "2026-03-17"
enable_flag: "enable_nodejs_perf_hooks_module"
disable_flag: "disable_nodejs_perf_hooks_module"
---

Enables the Node.js perf_hooks module. It is required to use this flag with nodejs_compat (or nodejs_compat_v2). This flag also implicitly enables the global Performance classes (PerformanceEntry, PerformanceMark, etc.).
