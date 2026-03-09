---
_build:
  publishResources: false
  render: never
  list: never

name: "Unhandled Rejection After Microtask Checkpoint"
sort_date: "2026-03-03"
enable_flag: "unhandled_rejection_after_microtask_checkpoint"
disable_flag: "no_unhandled_rejection_after_microtask_checkpoint"
---

When enabled, unhandledrejection processing is deferred until the microtask checkpoint completes, avoiding misfires on multi-tick promise chains.
