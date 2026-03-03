# Agent async notifications
#ai #design #interfaces #agents

How agents communicate state changes to users asynchronously - outside of the chat stream.

## Observed pattern

Agents doing background work need to surface status without requiring the user to watch a chat window. Mobile OS primitives (Live Activities, Dynamic Island, push notifications, haptics) provide channels for this.

## Examples

- [[Chowder iOS]] - shows thinking steps and tool execution inline with haptic feedback
- [[ActivitySmith]] - infrastructure for pushing Live Activities from any backend
