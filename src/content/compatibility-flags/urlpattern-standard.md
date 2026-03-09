---
_build:
  publishResources: false
  render: never
  list: never

name: "Urlpattern Standard"
sort_date: "2025-05-01"
enable_flag: "urlpattern_standard"
disable_flag: "urlpattern_original"
---

The original URLPattern implementation is not compliant with the WHATWG URLPattern Standard, leading to a number of issues reported by users. Unfortunately, making it spec compliant is a breaking change. This flag controls the availability of the new spec-compliant URLPattern implementation.
