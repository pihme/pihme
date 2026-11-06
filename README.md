My projects are meant to fit together like the pieces of a jigsaw puzzle: some big, some small, each useful on its own. This is the current set, and how the pieces connect.

- <img src="https://pihme.github.io/fregoli/favicon.svg" width="18" height="18" alt=""> **[Fregoli](https://pihme.github.io/fregoli/)** · [repository](https://github.com/pihme/fregoli)  
  A web application an agent can rewrite while it is running: capabilities are Cordis plugins mounted and unmounted in a live Node process.
- <img src="https://pihme.github.io/hermetarium/favicon.svg" width="18" height="18" alt=""> **[Hermetarium](https://pihme.github.io/hermetarium/)** · [repository](https://github.com/pihme/hermetarium)  
  The world an agent wakes up in: an OCI image it may use freely as root, behind a wall with Squid as the only, logged way out.
- <img src="https://pihme.github.io/git-warden/favicon.svg" width="18" height="18" alt=""> **[Git Warden](https://pihme.github.io/git-warden/)** · [repository](https://github.com/pihme/git-warden)  
  Guard posts between AI agents and their Git remote: a Push Guard that checks every push with deterministic rules, and a Backup Guard that keeps an append-only backup of every branch and tag.
- <img src="https://pihme.github.io/grok-budget-mcp/favicon.svg" width="18" height="18" alt=""> **[grok-budget-mcp](https://pihme.github.io/grok-budget-mcp/)** · [repository](https://github.com/pihme/grok-budget-mcp)  
  A small local MCP server that tells a Grok Build agent how much of its weekly usage pool is left, the same figure as /usage. Read-only, unofficial endpoint.
- <img src="https://pihme.github.io/claude-budget-mcp/favicon.svg" width="18" height="18" alt=""> **[claude-budget-mcp](https://pihme.github.io/claude-budget-mcp/)** · [repository](https://github.com/pihme/claude-budget-mcp)  
  A small local MCP server that tells a Claude Code agent how much of its 5-hour and weekly usage limits is left, the same figures as /usage. Read-only, unofficial endpoint.
- <img src="https://media.githubusercontent.com/media/pihme/helferlein/main/docs/mascot.png" height="18" alt=""> **[Helferlein](https://pihme.github.io/helferlein/)** · [repository](https://github.com/pihme/helferlein)  
  An animated Three.js 3D avatar that a web page can summon: it floats in, shows when it is waiting or working, and gets a random new look on every applied change.

**How they fit:** Fregoli can live inside Hermetarium. Fregoli's docs recommend Hermetarium as an optional habitat, and Hermetarium names Fregoli as one possible inhabitant. grok-budget-mcp could tell agents inside a Hermetarium habitat, or a watching agent next to its supervisor, how much Grok budget is left; both are possible uses, not built yet. claude-budget-mcp is grok-budget-mcp's sister for Claude Code: the same read-only gauge, with 5-hour and weekly windows instead of one weekly pool. Git Warden's Push Guard could stand on Hermetarium's wall and keep the Git write credential out of the habitat; its spec names Hermetarium as one possible wall, and nothing is built together yet. Fregoli could use grok-budget-mcp to check its Grok agent's budget, stop when it runs out, or warn the user; a possible use, not built yet. claude-budget-mcp could serve Fregoli the same way if its agent were Claude Code; today Fregoli runs Grok, so this is a possible use only. Helferlein is not part of the puzzle yet: it could become the face of Fregoli's agent, which is planned but not built.

Each project's website has a Jigsaw page with the same picture from that project's point of view, for example [Fregoli’s](https://pihme.github.io/fregoli/jigsaw/).

A second, smaller puzzle stands on its own, apart from the set above: two pieces that belong together.

- <img src="https://pihme.github.io/ragite/favicon.svg" width="18" height="18" alt=""> **[RAGite](https://pihme.github.io/ragite/)** · [repository](https://github.com/pihme/ragite)  
  Embeddable, CPU-friendly retrieval (RAG) as a SQLite extension.
- <img src="https://pihme.github.io/ragite-demo/favicon.svg" width="18" height="18" alt=""> **[RAGite demo](https://pihme.github.io/ragite-demo/)** · [repository](https://github.com/pihme/ragite-demo)  
  Search the SQLite docs and Wikipedia in your browser with RAGite and Datasette, offline and in one SQLite file.

**How they fit:** RAGite demo is a small Datasette app built on RAGite: it loads the released extension and uses only RAGite's public interface. Both websites have a Jigsaw page for this pair, for example [RAGite’s](https://pihme.github.io/ragite/jigsaw/).

Apart from the puzzles above, two more projects share a mark of their own.

- <img src="https://pihme.github.io/freigeist/assets/freigeist-mark.svg" width="18" height="18" alt=""> **[Freigeist](https://pihme.github.io/freigeist/)** · [repository](https://github.com/pihme/freigeist)  
  A blog about steering AI in uncharted waters.
- <img src="https://pihme.github.io/my-data-my-tools-my-rules/assets/logo-mark.svg" width="18" height="18" alt=""> **[My Data, My Tools, My Rules](https://pihme.github.io/my-data-my-tools-my-rules/)** · [repository](https://github.com/pihme/my-data-my-tools-my-rules)  
  A wiki-style directory of open-source projects for digital self-determination.

**How they fit:** Freigeist's site points readers to My Data, My Tools, My Rules; the two share a mark. The directory is a companion for the blog. Nothing else is built together yet.
