---
_build:
  publishResources: false
  render: never
  list: never

name: "Text Decoder Replace Surrogates"
sort_date: "2026-02-24"
enable_flag: "text_decoder_replace_surrogates"
disable_flag: "disable_text_decoder_replace_surrogates"
---

When enabled, the UTF-16le TextDecoder will replace lone surrogates with U+FFFD (the Unicode replacement character) as required by the spec. Previously, lone surrogates were passed through unchanged, producing non-well-formed strings.
