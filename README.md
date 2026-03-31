# 💬 Real-Time Messaging App

Live chat application with a professional interface built with HTML, CSS, and JavaScript. Simulates the complete experience of a messaging platform including conversations, automatic replies, file attachments, and status indicators.

## Features

- **Contact list** with online/away/offline status and unread message badges
- **Real-time messages** — Send messages and receive automatic simulated replies
- **Typing indicator** — Animated dots while the contact is "typing"
- **Read receipts** — Double check ✓✓ on sent messages
- **File attachments** — Simulates sending .zip, .pdf, .sql files with name and size
- **Image sharing** — Screenshot upload simulation
- **Code snippets** — Button to insert code blocks in the chat
- **Team channels** — Channel section (#general, #projects, #design)
- **Info panel** — Contact stats, recent files, and online members
- **Contact search** — Real-time filter in the contact list
- **Responsive design** — Collapsible side panels on mobile

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML5, CSS3, JavaScript ES6+ |
| Layout | CSS Grid, Flexbox, sticky positioning |
| Typography | Inter + JetBrains Mono |
| Animations | CSS keyframes (typing dots, pulse) |

> **Production stack:** Node.js · Socket.io · Express · MySQL · JWT Auth

## Getting Started

```bash
# Clone the repository
git clone https://github.com/Xasve/livechat-demo.git

# Open in browser (no server required)
open index.html
```

Or visit the **[Live Demo →](https://xasve.github.io/livechat-demo)**

## Project Structure

```
livechat-demo/
└── index.html      # Full app (HTML + CSS + JS)
```

## Production Architecture

```
Browser (Client)
    │
    ├── Socket.io client  ──→  Node.js + Express server
    │                              │
    │                              ├── Socket.io (real-time events)
    │                              ├── REST API (history, users)
    │                              └── MySQL (messages, rooms, users)
    │
    └── JWT Token  ──→  Auth middleware
```

## What You'll See in the Demo

- Left panel with 6 contacts and their online statuses
- Central chat with conversation history
- Automatic replies when you send messages
- "Typing..." animation before each reply
- Right panel with contact info and online members list

## Author

**Ethan Barboza** — Full Stack Developer · Freelance
📧 ethan.barboza10@gmail.com
🌐 [xasve.github.io](https://xasve.github.io)
