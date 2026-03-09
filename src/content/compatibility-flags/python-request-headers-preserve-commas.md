---
_build:
  publishResources: false
  render: never
  list: never

name: "Python Request Headers Preserve Commas"
sort_date: "2026-02-17"
enable_flag: "python_request_headers_preserve_commas"
disable_flag: "disable_python_request_headers_preserve_commas"
---

Preserve commas in Python Request headers rather than treating them as separators, while still exposing multiple Set-Cookie headers as distinct values.
