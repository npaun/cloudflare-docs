---
_build:
  publishResources: false
  render: never
  list: never

name: "Internal Writable Stream Abort Clears Queue"
sort_date: "2024-09-02"
enable_flag: "internal_writable_stream_abort_clears_queue"
disable_flag: "internal_writable_stream_abort_does_not_clear_queue"
---

When using the original WritableStream implementation ("internal" streams), the abort() operation would be handled lazily, meaning that the queue of pending writes would not be cleared until the next time the queue was processed. This behavior leads to a situtation where the stream can hang if the consumer stops consuming. When set, this flag changes the behavior to clear the queue immediately upon abort.
