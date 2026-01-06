---
_build:
  publishResources: false
  render: never
  list: never

name: "Strip Bom In Read All Text"
sort_date: "2026-01-13"
enable_flag: "strip_bom_in_read_all_text"
disable_flag: "do_not_strip_bom_in_read_all_text"
---

Instructs the `readAllText` method in streams to strip the leading UTF8 BOM if present.