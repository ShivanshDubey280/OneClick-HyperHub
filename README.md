# OneClick HyperHub UI Demo

Standalone frontend-only product concept for OneClick HyperHub. It has its own dependencies and uses mock data/state only; it does not require the OneClick_UI application or backend.

## Requirements

- Node.js 20.19+ or 22.12+
- npm

## Install and run

```powershell
npm install
npm run dev
```

Open the local URL printed by Vite (usually `http://127.0.0.1:5174`).

## Build and preview

```powershell
npm run build
npm run preview
```

## Folder Structure

- `src/components/AppShell` - top header, sidebar, and application layout.
- `src/components/Hero` - dashboard hero with subtle cloud platform visual.
- `src/components/CapabilityAccordion` - expandable capability sections.
- `src/components/Cards` - tool, agent, and capability cards.
- `src/components/AgentChat` - mock AI assistant drawer and chat messages.
- `src/components/SearchBar` - reusable search input.
- `src/data` - static mock capabilities, tools, and agents.
- `src/pages` - home dashboard page.
- `src/styles` - global demo styles and small visual details.

## Mocked

- Tool detail launch behavior is a frontend-only modal.
- Agent cards open a chat drawer with static suggested prompts.
- Chat messages are stored in React state.
- Assistant responses are predefined and delayed to simulate thinking.
- Sidebar navigation only changes active UI state.

## Future Backend Integration

A production version would need authenticated user/session data, live capability configuration, tool launch APIs, real assessment workflows, persisted chat sessions, file upload handling, and an LLM or agent orchestration backend.
