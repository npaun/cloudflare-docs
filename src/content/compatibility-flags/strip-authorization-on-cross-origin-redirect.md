---
_build:
  publishResources: false
  render: never
  list: never

name: "Strip Authorization On Cross Origin Redirect"
sort_date: "2025-09-01"
enable_flag: "strip_authorization_on_cross_origin_redirect"
disable_flag: "retain_authorization_on_cross_origin_redirect"
---

This flag specifies that when automatic redirects are enabled, and a redirect points to a URL at a different origin, if the original request contained an Authorization header, that header is removed before following the redirect. This behavior is required by the current version of the Fetch API specification.  This requirement was added to the Fetch spec in 2022, well after Cloudflare Workers originally implemented it. Hence, Workers did not originally implement this requirement. This requirement is backwards-incompatible, and so the new behavior is guarded by a compatibility flag.  Note that the old behavior was not inherently insecure, and indeed could be desirable in many circumstances. For example, if an API that requires authorization wishes to change its hostname, it might wish to redirect to the new hostname while having the client send along their credentials. Under the new fetch behavior, such a redirect will break clients, and this has legitimately broken real use cases. However, it's true that the old behavior could be a "gotcha" leading to security problems when combined with other mistakes. Hence, the spec was changed, and Workers must follow the spec.
