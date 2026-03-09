---
_build:
  publishResources: false
  render: never
  list: never

name: "Fetch Iterable Type Support"
sort_date: "2026-02-19"
enable_flag: "fetch_iterable_type_support"
disable_flag: "no_fetch_iterable_type_support"
---

Enables passing sync and async iterables as the body of fetch Request or Response. Previously, sync iterables like Arrays would be accepted but stringified, and async iterables would be treated as regular objects and not iterated over at all. With this flag enabled, sync and async iterables will be properly iterated over and their values used as the body of the request or response. The actual compat flag enables the specific AsyncGeneratorIgnoringStrings type wrapper that allows this behavior and allows sync Generator and AsyncGenerator objects to be included in kj::OneOf declarations safely with strings and other types. When enabled, strings are ignored but Arrays will be treated as iterables and not stringified as before. Also see fetchIterableTypeSupportOverrideAdjustment.
