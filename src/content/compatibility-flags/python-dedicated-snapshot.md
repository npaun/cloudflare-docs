---
_build:
  publishResources: false
  render: never
  list: never

name: "Python Dedicated Snapshot"
sort_date: "2025-10-16"
enable_flag: "python_dedicated_snapshot"
disable_flag: "disable_python_dedicated_snapshot"
---

Enables the generation of dedicated snapshots on Python Worker upload. The snapshot will be stored inside the resulting WorkerBundle of the Worker. The snapshot will be taken after the top-level execution of the Worker.
