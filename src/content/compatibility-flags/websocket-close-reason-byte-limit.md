---
_build:
  publishResources: false
  render: never
  list: never

name: "Websocket Close Reason Byte Limit"
sort_date: "2026-03-03"
enable_flag: "websocket_close_reason_byte_limit"
disable_flag: "no_websocket_close_reason_byte_limit"
---

When enabled, WebSocket close() throws a SyntaxError DOMException if the reason string exceeds 123 bytes when UTF-8 encoded, as required by the WHATWG WebSocket spec and RFC 6455 Section 5.5. Previously, workerd allowed arbitrarily long close reasons without validation.
