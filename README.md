# Globomantics plugins

The plugin marketplace the Globomantics Shipping team uses to share GitHub Copilot plugins with each other.

| Plugin | What it adds |
| --- | --- |
| `provider-catalog` | The `lookup-spec` skill, which looks up a delivery provider's integration spec in the provider catalog |

The plugin doesn't connect to the provider catalog by itself. Everyone adds the provider catalog's MCP server with their own access token.

## Add the marketplace

In the GitHub Copilot app, open **Customize**, then **Plugins**, and use the settings icon next to the marketplace dropdown to add this repository. Then pick the marketplace in the dropdown and install `provider-catalog`.

From the Copilot CLI:

```
copilot plugin marketplace add <owner>/<this-repository>
```

## Layout

```
.github/plugin/marketplace.json            lists the plugins in this marketplace
plugins/provider-catalog/plugin.json       the plugin's manifest
plugins/provider-catalog/skills/lookup-spec/SKILL.md
```

## Disclaimer

This demo uses fictional names and people. No affiliation with or endorsement by any real company.
