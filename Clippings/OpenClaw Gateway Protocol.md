# OpenClaw Gateway Protocol
#dev #agents #protocols

https://docs.openclaw.ai/gateway/protocol

Unified control and transport layer for agent systems. WebSocket + JSON protocol providing a single connection point for all client types (CLI, web, desktop, mobile) to communicate with agents.

Role-based model: **Operators** (control plane - CLI, UI, automation) send commands; **Nodes** (capability hosts - mobile, embedded) execute tasks. Connections begin with cryptographic handshake declaring role, capabilities, and permissions.

Message types: requests, responses, and server-pushed events. Scopes control API access; capabilities/permissions gate what nodes can execute.
