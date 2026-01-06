---
_build:
  publishResources: false
  render: never
  list: never

name: "Enable Node.js trace_events module"
enable_flag: "enable_nodejs_trace_events_module"
disable_flag: "disable_nodejs_trace_events_module"
---

Enables the Node.js non-functional stub `trace_events` module. It is required to use this flag with `nodejs_compat` (or `nodejs_compat_v2`).