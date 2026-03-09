---
_build:
  publishResources: false
  render: never
  list: never

name: "Containers Pid Namespace"
sort_date: "2026-04-01"
enable_flag: "containers_pid_namespace"
disable_flag: "no_containers_pid_namespace"
---

When enabled, containers attached to Durable Objects do NOT share the host PID namespace (they get their own isolated PID namespace). When disabled (the default), containers share the host PID namespace.
