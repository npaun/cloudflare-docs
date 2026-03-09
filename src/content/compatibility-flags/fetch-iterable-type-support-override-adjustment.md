---
_build:
  publishResources: false
  render: never
  list: never

name: "Fetch Iterable Type Support Override Adjustment"
sort_date: "2026-01-15"
enable_flag: "fetch_iterable_type_support_override_adjustment"
disable_flag: "no_fetch_iterable_type_support_override_adjustment"
---

Further adapts the fetch iterable type support to adjust for toString/toPrimitive overrides on sync iterable objects. Specifically, if an object passed as the body of a fetch Request or Response is sync iterable but has a custom toString or toPrimitive method, we will skip treating it as a sync iterable and instead allow it to fall through to being handled as a stringified object.
