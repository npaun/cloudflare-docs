---
_build:
  publishResources: false
  render: never
  list: never

name: "Websocket Standard Binary Type"
sort_date: "2026-03-17"
enable_flag: "websocket_standard_binary_type"
disable_flag: "no_websocket_standard_binary_type"
---

Per the WHATWG WebSocket spec, the binaryType attribute defaults to "blob" and binary messages are delivered as Blob objects. Previously, workerd did not expose the binaryType property at all and always delivered binary messages as ArrayBuffer. When this flag is enabled, binaryType defaults to "blob" and binary messages are delivered as Blob. Workers that set binaryType to "arraybuffer" will continue to receive ArrayBuffer regardless of this flag.  Note: This flag has no effect on the Durable Object hibernatable WebSocket message handler (webSocketMessage). That handler always receives binary data as ArrayBuffer, since it operates outside the normal WebSocket read loop.
