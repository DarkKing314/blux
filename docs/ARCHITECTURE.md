# 🛰️ BLUX Architecture Overview

BLUX is a constellation of modular, open-source AI tools—each part designed to be independent, extensible, and privacy-first.

---

## BLUX Ecosystem Map

- [**BLUX** (Umbrella Project)](https://github.com/Justadudeinspace/blux)
    - [**BLUX-cA** (Coding Agent)](https://github.com/Justadudeinspace/blux-ca): Orchestrates engines, acts as the "hive mind"
    - [**BLUX-Quantum** (Modular AI CLI)](https://github.com/Justadudeinspace/blux-quantum): Command-line interface and plugin platform
    - [**BLUX-Lite** (Terminal/Android)](https://github.com/Justadudeinspace/blux-lite): Lightweight AI agent for terminals and Android
    - [**Liberation Framework** (User Memory System)](https://github.com/Justadudeinspace/liberation-framework): User-defined, persistent local memory

---

## Core Design Principles

- **Modular:** Each component is plug-and-play; use them together or independently
- **Local-First:** All user data and memory is stored locally by default
- **Privacy-First:** No data is sent to the cloud without your explicit consent
- **Extensible:** Easily add plugins, AI models, and custom agents
- **Interoperable:** All projects can communicate or run standalone

---

## How Components Work Together

- **BLUX-cA** acts as the main orchestrator, routing prompts to available AI engines and plugins.
- **BLUX-Quantum** provides a unified CLI to control BLUX-cA and other agents.
- **BLUX-Lite** delivers similar functionality for Android and lightweight terminals.
- **Liberation Framework** manages persistent, user-controlled memory for all BLUX tools.
- **Plugins and models** extend BLUX with new engines, tools, and capabilities.

---

## Extending BLUX

- Add new AI models (see [models](../models/README.md))
- Build plugins for new tasks or agent types (see [plugins](plugins.md))
- Compose pipelines and custom workflows with CLI or API access

---

> _BLUX: Building a modular, ethical AI ecosystem for the space age._
