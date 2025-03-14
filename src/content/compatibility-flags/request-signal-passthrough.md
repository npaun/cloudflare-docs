---
_build: 
  publishResources: false
  render: never
  list: never

name: "Request.signal is passed through to subrequests"
sort_date: "2025-03-14"
enable_date: "2025-04-14"
enable_flag: "request_signal_passthrough"
disable_flag: "no_request_signal_passthrough"
---

When this flag is enabled, the `signal` property of the incoming request to a Worker follows Web-standard behaviour, and will be passed through when the request is cloned, or a new request is created from it. As a result, if the incoming request is canceled by the client, all outgoing subrequests will also be canceled, unless the `signal` property is explicitly modified or cleared.

Because support for Request.signal was recently added to Cloudflare Workers, this behaviour will not apply to existing Workers, and can also be disabled by setting `no_request_signal_passthrough`.
