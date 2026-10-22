# loopdesk

A local control desk for AI agents: an MCP server your coding agents (Claude Code, Codex, …) connect to, and a web UI in
your browser where you steer them.

> **Status: planning.** Version 0.0.1 holds the name; nothing is usable yet.

## The idea

With capable agents, the limit is no longer how fast code gets written but how fast a human can understand and steer
the work. loopdesk keeps the models busy and keeps the human's part small and quick:

- **Tasks with a finish line.** Agents queue tasks, each with a well-defined goal that says when it is done; the
  result (code, text, images, …) waits for you to accept or reject.
- **Feedback before execution.** Tasks that need your input are put in front of you before they run — as multiple
  choice, a text box, or a button that asks the agent for clarification (shift-click to add your own question).
- **Recorded assumptions.** Every assumption an agent makes is written down, with what depends on it, so a wrong one
  is cheap to find and fix.
- **Work for subagents.** Approved tasks are split into units subagents can take on their own.
- **Search.** A local vector index over tasks, assumptions and decisions.

Runs locally: `pip install loopdesk`, start the server, open it in your browser.

## License

MIT
