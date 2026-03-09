---
_build:
  publishResources: false
  render: never
  list: never

name: "Handle Cross Request Promise Resolution"
sort_date: "2024-10-14"
enable_flag: "handle_cross_request_promise_resolution"
disable_flag: "no_handle_cross_request_promise_resolution"
---

Historically, it has been possible to resolve a promise from an incorrect request IoContext. This leads to issues with promise continuations being scheduled to run in the wrong IoContext leading to errors and difficult to diagnose bugs. With this compatibility flag we arrange to have such promise continuations scheduled to run in the correct IoContext if it is still alive, or dropped on the floor with a warning if the correct IoContext is not still alive.
