# circle-chat
> Collaborative AI Editor — Real-Time Multi-User Workspace

A real-time collaborative text editor where multiple users can write and edit together simultaneously, with AI capabilities built directly into the editing experience.

## What is this?

circle-chat is a multiplayer document editor powered by WebSocket-based synchronization and CRDT (Conflict-free Replicated Data Type) algorithms to keep all users in sync without conflicts. Think Google Docs, but with an AI co-writer embedded inline — users can highlight text and instantly summarize, rewrite, or generate new content using OpenAI.

The backend is designed for scale: Redis handles pub/sub for real-time events, role-based access control manages document permissions, and version history lets users roll back to any previous state.

## Core Features

- [ ] Real-time multi-user editing with CRDT synchronization
- [ ] WebSocket connection management and presence indicators
- [ ] Inline AI tools — summarize, rewrite, generate
- [ ] Role-based access control (owner, editor, viewer)
- [ ] Version history and document restore
- [ ] Redis-backed event layer
- [ ] Dockerized deployment on AWS

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React, TypeScript, Tailwind CSS |
| Real-time | WebSockets, CRDT |
| Backend | Node.js, Express |
| AI | OpenAI API (GPT-4o) |
| Caching | Redis |
| Database | PostgreSQL |
| Infra | Docker, AWS |
