# ActiveLayer integrations

Integrations that connect developer tools and AI assistants to
[ActiveLayer](https://activelayer.com) spam protection.

## Cursor

The [ActiveLayer Cursor plugin](cursor/README.md) connects to the hosted
ActiveLayer MCP server through OAuth. Create projects, test submissions, review
detections, report incorrect verdicts, and track usage from your editor.

The plugin is packaged in `cursor/`. The root
`.cursor-plugin/marketplace.json` indexes it with `"source": "cursor"` so Cursor
can discover the plugin from this repository.

```text
.cursor-plugin/
  marketplace.json
cursor/
  .cursor-plugin/
    plugin.json
  assets/
    logo.svg
  mcp.json
  README.md
  LICENSE
README.md
LICENSE
```

See the [plugin README](cursor/README.md) for setup, available tools, local
testing, and publisher application copy. For local testing, copy the contents
of `cursor/` into `~/.cursor/plugins/local/activelayer/`.

After testing, submit this repository at
[Cursor Marketplace publishing](https://cursor.com/marketplace/publish).
Marketplace publication requires Cursor's review.

## License and support

The integration package is licensed under [MIT](LICENSE). Use of the hosted
ActiveLayer service is governed by its [terms](https://activelayer.com/terms/)
and plan limits. Contact [support@activelayer.com](mailto:support@activelayer.com).
