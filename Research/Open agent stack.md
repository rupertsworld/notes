# Open agent stack

Thinking about what's needed to create an open, viable agent stack — not a single product but a set of composable pieces. Some of this overlaps with Telepath's roadmap; the goal is to figure out where the product area fits.

## Key pieces

### Background agent execution
A way to execute a command with an agent in the background, track running commands, and see active background jobs/agents. Agents should also have a tool to dispatch background work themselves. They return a summary or report; full messages are posted for review.

If in a git repo, there should be an option to spin up a disposable worktree — replicate the repo elsewhere, do work, push a branch. Cleanup or retention TBD.

### Agent cron / scheduled jobs
A jobs directory with cron-like scheduling for background agents. Triggers could be:
- Time-based (actual cron schedule)
- File/folder change (watch-based) — though this is dicier, more experimental

### Relationship to Telepath
These are internal tools / experiments right now. The bet is that some will grow into products or open source packages and become part of the company OS. Even if they stay internal, they exercise the same muscles as future product areas Telepath might pursue — orchestration, agent infrastructure, developer tooling.

Worth experimenting with soon for personal workflows to validate the ideas.
