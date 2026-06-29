# project.md Specification

project.md is an AI-native project management format.

It defines how a project should be structured so that humans and AI agents can continue working on it across conversations, devices, and tools.

## Goals

project.md is designed to help AI agents:

- understand the current state of a project
- continue from previous conversations
- update project knowledge after discussions
- preserve important decisions and reasoning
- avoid losing context when chats or tools change

## Non-Goals

project.md is not:

- a note-taking app
- a task manager
- a replacement for GitHub Issues
- a source code structure
- a private business database

## Core Files

A project using project.md should start with two files:

- `PROJECT.md`
- `HISTORY.md`

Additional files may be added only when the project requires them.

Examples:

- `ROADMAP.md`
- `BUSINESS.md`
- `SPECIFICATION.md`
- `RESEARCH.md`
- `QUESTIONS.md`

## PROJECT.md

`PROJECT.md` represents the current state of the project.

It should answer:

- What is this project?
- Why does it exist?
- What is the current focus?
- What has been decided?
- What is still unclear?
- What should happen next?

## HISTORY.md

`HISTORY.md` records important changes over time.

It should preserve:

- decisions
- direction changes
- reasoning
- major milestones
- rejected ideas when useful

## AI Behavior

When an AI agent works with a project.md repository, it should:

1. Read `PROJECT.md` first.
2. Read `HISTORY.md` when previous reasoning is needed.
3. Update `PROJECT.md` after meaningful project conversations.
4. Append important changes to `HISTORY.md`.
5. Avoid creating new files unless the project clearly needs them.
6. Keep the current state concise and useful.
7. Preserve private project details only inside the private project repository.

## Public and Private Separation

The `project.md` specification can be public.

Actual projects may be public or private.

Private business ideas, strategy, roadmaps, and source code should not be stored in the public specification repository.
