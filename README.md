My projects are meant to fit together like the pieces of a jigsaw puzzle: some big, some small, each useful on its own. This is the current set, and how the pieces connect.

- <img src="https://pihme.github.io/fregoli/favicon.svg" width="18" height="18" alt=""> **[Fregoli](https://pihme.github.io/fregoli/)** · [repository](https://github.com/pihme/fregoli)  
  A web application an agent can rewrite while it is running: capabilities are Cordis plugins mounted and unmounted in a live Node process.
- <img src="https://pihme.github.io/hermetarium/favicon.svg" width="18" height="18" alt=""> **[Hermetarium](https://pihme.github.io/hermetarium/)** · [repository](https://github.com/pihme/hermetarium)  
  The world an agent wakes up in: an OCI image it may use freely as root, behind a wall with Squid as the only, logged way out.
- <img src="https://pihme.github.io/grok-budget-mcp/favicon.svg" width="18" height="18" alt=""> **[grok-budget-mcp](https://pihme.github.io/grok-budget-mcp/)** · [repository](https://github.com/pihme/grok-budget-mcp)  
  A small local MCP server that tells a Grok Build agent how much of its weekly usage pool is left, the same figure as /usage. Read-only, unofficial endpoint.
- <img src="https://pihme.github.io/claude-budget-mcp/favicon.svg" width="18" height="18" alt=""> **[claude-budget-mcp](https://pihme.github.io/claude-budget-mcp/)** · [repository](https://github.com/pihme/claude-budget-mcp)  
  A small local MCP server that tells a Claude Code agent how much of its 5-hour and weekly usage limits is left, the same figures as /usage. Read-only, unofficial endpoint.
- <img src="https://pihme.github.io/git-warden/favicon.svg" width="18" height="18" alt=""> **[Git Warden](https://pihme.github.io/git-warden/)** · [repository](https://github.com/pihme/git-warden)  
  Guard posts between AI agents and their Git remote: a Push Guard that checks every push with deterministic rules, and a Backup Guard that keeps an append-only backup of every branch and tag.

**How they fit:** Fregoli can live inside Hermetarium. Fregoli's docs recommend Hermetarium as an optional habitat, and Hermetarium names Fregoli as one possible inhabitant. grok-budget-mcp could tell agents inside a Hermetarium habitat, or a watching agent next to its supervisor, how much Grok budget is left; both are possible uses, not built yet. claude-budget-mcp is grok-budget-mcp's sister for Claude Code: the same read-only gauge, with 5-hour and weekly windows instead of one weekly pool. Git Warden's Push Guard could stand on Hermetarium's wall and keep the Git write credential out of the habitat; its spec names Hermetarium as one possible wall, and nothing is built together yet.

Each project's website has a Jigsaw page with the same picture from that project's point of view, for example [Fregoli’s](https://pihme.github.io/fregoli/jigsaw/).
