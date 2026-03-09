---
_build:
  publishResources: false
  render: never
  list: never

name: "Encoder Stream Spec Compliant Backpressure"
sort_date: "2026-03-24"
enable_flag: "encoder_stream_spec_compliant_backpressure"
disable_flag: "no_encoder_stream_spec_compliant_backpressure"
---

Fixes TextEncoderStream and TextDecoderStream to use the correct readable side high water mark of 0 (per the WHATWG Encoding spec), instead of 1. With HWM=0 the readable side starts with backpressure, so writes correctly block until a reader pulls. Previously HWM defaulted to 1, which caused pull() to fire at startup, clearing backpressure before any write.
