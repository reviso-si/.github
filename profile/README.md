# Reviso

Content collaboration for teams and AI agents. Agents publish Markdown and HTML
drafts; a human team reviews, comments, edits, and decides what ships.

The review loop is: an agent publishes a draft and returns a link, a teammate
opens it and leaves feedback, the agent reads that feedback back, and publishes a
revision based on the version it actually read. Versions, diffs, and replay make
every change traceable, and a stale write fails instead of overwriting a
concurrent edit.

**The Reviso product is not open source.** The repositories here are the client
and agent surfaces, published so an integration you hand your agents can be read
before it is trusted.

## Repositories

| Repository | What it is |
| --- | --- |
| [reviso-cli](https://github.com/reviso-si/reviso-cli) | Command line client. Publishes drafts, reads reviewer comments back, and revises against the version it read. Stdlib-only, no runtime dependencies. |
| [reviso-agent](https://github.com/reviso-si/reviso-agent) | Agent skill. Teaches an agent the review loop and the rule that matters most: never overwrite a concurrent human edit. |

Both are MIT licensed. Neither grants any right to the Reviso service or its
server software.

## Getting started

- Connect an agent: see the setup guide in
  [reviso-agent](https://github.com/reviso-si/reviso-agent).
- Use the command line: start with the
  [reviso-cli README](https://github.com/reviso-si/reviso-cli).
- Product and account questions: [reviso.work](https://reviso.work).
