---
_build:
  publishResources: false
  render: never
  list: never

name: "Python Workflows Implicit Dependencies"
sort_date: "2026-02-25"
enable_flag: "python_workflows_implicit_dependencies"
disable_flag: "no_python_workflows_implicit_dependencies"
---

replaces depends param on steps to an implicit approach with step callables passed as params these steps are called internally and act as dependencies
