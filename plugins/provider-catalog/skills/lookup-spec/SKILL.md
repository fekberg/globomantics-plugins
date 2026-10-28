---
name: lookup-spec
description: Look up a delivery provider's integration spec in the provider catalog. Use this when someone asks to look up, read or check a provider's spec, or which API versions a provider has.
---

# Look up an integration spec

The provider catalog is the partnerships team's internal service. It holds every delivery provider's integration spec, version by version, and offers them through the provider-catalog MCP server.

1. If the provider catalog's find_provider and get_spec tools aren't available, say that the provider catalog isn't connected and stop. Don't answer from memory or from the repository.
2. If no provider is named, ask which one.
3. Call find_provider with the provider's name to get its id and the versions that exist.
4. If no version was given, use the current version and say which one you used. If the version asked for doesn't exist, list the versions that do.
5. Call get_spec with the provider id and the version.
6. Answer with:
   - the provider, the version, and whether that version is current or retired
   - a table of services: code, name, transit days
   - a table of tracking codes: code, description, and whether it's final

Copy every code exactly as the spec spells it. When you answer a question about a spec, say which part of the spec the answer comes from.
