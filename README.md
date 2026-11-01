# Zambia Land Lots & Lot Number Lookup MCP

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Zambian land research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- ~297k state-cadastre lots and ~34k customary/village records from the Ministry of Lands' NSDI lot locator
- Lot lookup by lot key as the registry writes it (`LUS/2675`, `F/8178/34`) or coordinates
- Each lot's representative point and, for state lots, its bounding extent

Index records only: there are no parcel boundaries, owners, titles, areas or land use.

## Connect

```
https://bumiatlas.com/mcp/zambia
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/zambia](https://bumiatlas.com/mcp-docs/zambia).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `ZM_lot_search` | Find lots by lot key, or by `latitude, longitude` (lots whose extent holds the point first, then the nearest), with each lot's point and extent |

## Example prompts

- *"Which lots are near -15.4167, 28.2833?"*
- *"Where is lot LUS/2675?"*
- *"Find farm lot F/8178/34."*
- *"Is this point inside a state lot's extent?"*

## Data source

Lot index © Ministry of Lands and Natural Resources, Zambia, National Spatial Data Infrastructure (map.gov.zm). A copy of public data for research, not a legal record.
