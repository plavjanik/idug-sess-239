# SESS-239 — SQL Injection on SterAIds: Is Your Db2 Ready for AI-Assisted Attackers?

**IDUG EMEA 2026 · Porto · Wednesday, September 30, 2:00–3:00 pm · Room E · Platform: Db2 for z/OS**

Petr Plavjaník, Broadcom

Interactive companion demos and slides for the session. Everything here is
self-contained, open-source, and uses only synthetic data.

## ▶ Demos

**Start here: [the demo launcher](https://plavjanik.github.io/idug-sess-239/)** — all seven
demos in talk order, with keyboard shortcuts and recommended zoom levels.

| Demo | What it shows |
|---|---|
| [SQL injection anatomy](https://plavjanik.github.io/idug-sess-239/sql-injection-anatomy.html) | The classic mechanism, animated, in 7 languages (COBOL, PL/I, HLASM, REXX, Java, Python, TypeScript) — vulnerable vs. fixed |
| [The ORDER BY oracle](https://plavjanik.github.io/idug-sess-239/order-by-oracle.html) | Every value is a parameter, yet an 18-question binary search steals a salary through the sort order alone |
| [The lethal trifecta](https://plavjanik.github.io/idug-sess-239/lethal-trifecta.html) | Private data × untrusted content × exfiltration channel — arm the legs and watch how far the attack gets |
| [MCP in 90 seconds](https://plavjanik.github.io/idug-sess-239/mcp-in-90-seconds.html) | A self-running tour of the Model Context Protocol with real JSON-RPC frame shapes |
| [Demo A: schema discovery](https://plavjanik.github.io/idug-sess-239/demo-a-schema-discovery.html) | Replay of a real capture: an AI agent learns a Db2 database's structure by itself |
| [Demo B: the data bites back](https://plavjanik.github.io/idug-sess-239/demo-b-data-bites-back.html) | A planted prompt injection vs. six protections — with honest labels for what is simulated and what mirrors the real capture |
| [Same query, three identities](https://plavjanik.github.io/idug-sess-239/same-query-three-identities.html) | The SQL never changes; trusted contexts, roles, row permissions, and column masks decide what Db2 returns |

The demos run in any modern browser with no server and no build — clone and
double-click, or use the GitHub Pages links above. On a projector, use the zoom
level recommended per demo on the launcher page. Every page also has a ☀/☾
dark↔light theme toggle and an A/A/A text-size control (top right) — both
settings persist across pages.

## Slides

[SESS-239-SQL-Injection-on-SterAIds.pdf](https://plavjanik.github.io/idug-sess-239/slides/SESS-239-SQL-Injection-on-SterAIds.pdf)

## The stack shown in the session

- [Zowe MCP](https://github.com/zowe/zowe-mcp) (`@zowe/mcp-server`, EPL-2.0) — MCP server for z/OS
- [`@zowe/db2-for-zowe-cli`](https://www.npmjs.com/package/@zowe/db2-for-zowe-cli) — the Db2 plug-in the MCP Db2 tools are modeled after
- Db2 13 for z/OS native controls: trusted contexts, roles, row permissions, column masks, audit

Demo captures were made against a lab subsystem with synthetic data only.

## License

Code and content: [MIT](LICENSE).
Bundled IBM Plex fonts: [SIL Open Font License 1.1](fonts/LICENSE-IBM-Plex.txt) (© IBM Corp.).
