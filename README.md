# Torpedo Box — Presets CDN

Public preset list for [Torpedo Box](https://github.com/your-org/torpedo-box) VPN client.

## Format

```json
{
  "version": 1,
  "presets": [
    {
      "id":      "unique-id",
      "name":    "Display Name",
      "hint":    "short · domain · hint",
      "color":   "#RRGGBB",
      "letter":  "ab",
      "policy":  "proxy | direct",
      "domains": ["example.com", "cdn.example.com"]
    }
  ]
}
```

| Field     | Type                 | Description                              |
|-----------|----------------------|------------------------------------------|
| `id`      | string               | Unique stable identifier                 |
| `name`    | string               | Shown in UI                              |
| `hint`    | string               | Monospace subtitle (key domains)         |
| `color`   | hex string           | Icon accent color                        |
| `letter`  | string (1–3 chars)   | Icon label                               |
| `policy`  | `"proxy"` / `"direct"` | Route through VPN or bypass it         |
| `domains` | string[]             | Domain suffixes added as one rule        |

## Contributing

PRs welcome — add new presets or expand domain lists.
