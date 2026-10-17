# Receptron

**We build the tools we need for working with AI agents, and we open-source them.**

Everything here is written in TypeScript and runs on your own machine. Pick the one that matches
what you are trying to do.

## Run several coding agents at once

**[MulmoTerminal](https://github.com/receptron/mulmoterminal)** — a browser terminal grid for
parallel coding agents. Claude Code, Codex and six more CLIs side by side, each cell a real pty,
with the one that needs you marked in colour. Sessions survive a reload (tmux), work isolates in
git worktrees, and a push reaches your phone when a turn finishes.

![MulmoTerminal — a grid of live Claude Code sessions, each colour-coded by state, updating in real time](https://raw.githubusercontent.com/receptron/mulmoterminal/main/docs/guide/images/hero.gif)

```sh
npx mulmoterminal@latest
```

[Guide](https://www.mulmoterminal.com) · [日本語ガイド](https://zenn.dev/singularity/articles/mulmoterminal-guide-ja)

## Keep an assistant on your own computer

**[MulmoClaude](https://github.com/receptron/mulmoclaude)** — chat with Claude Code where the
answer can be a wiki page, a spreadsheet, a chart, a form or a 3D scene instead of more text.
Memories, data and apps stay as plain files in your workspace, readable without us.

```sh
npx mulmoclaude@latest
```

## Turn a written script into video, audio or slides

**[MulmoCast](https://github.com/receptron/mulmocast-cli)** — write a script, get a narrated
video, a podcast episode or a deck. Voice cloning, AI-generated music, lip sync, and image and
video models from several providers.

```sh
npx mulmocast
```

Also as a desktop app: **[mulmocast-app](https://github.com/receptron/mulmocast-app)**.

## Keep talking while the answer draws itself

**[MulmoChat](https://github.com/receptron/MulmoChat)** — in active development again. A research
prototype for chat that is not a text stream: you keep speaking, and images materialise, maps
become explorable and games turn playable on the canvas beside the conversation. Each kind of
answer is a plugin on the GUI Chat Protocol — the same protocol MulmoClaude and MulmoTerminal
speak — so teaching it something new is a package rather than a fork.

Run it from source, with your own API keys:

```sh
git clone https://github.com/receptron/MulmoChat.git
```

[The idea](https://github.com/receptron/MulmoChat/blob/main/docs/LLM_OS.md) ·
[Architecture](https://github.com/receptron/MulmoChat/blob/main/docs/WHITEPAPER.md) ·
[Writing a plugin](https://github.com/receptron/MulmoChat/blob/main/docs/TOOLPLUGIN.md)

## Build on the engines

**[GraphAI](https://github.com/receptron/graphai)** — describe an agentic workflow as a
declarative dataflow graph in YAML or JSON, and run it. Nodes run as soon as their inputs are
ready, so concurrency is a property of the graph rather than something you write.
[graphai.info](https://graphai.info)

**[@receptron/laya](https://github.com/receptron/laya)** — run Laya, an open-source System-1
decision model, from Node.js via ONNX Runtime. Typed questions in, calibrated probabilities out,
in one forward pass. No Python at runtime.

**[SlashGPT](https://github.com/receptron/SlashGPT)** — our earlier LLM-agent experiment, from
before the category had a name, and the ground the rest of this work was built on. A new agent is
a manifest file, and `/name` switches between them.

## Who we are

[Satoshi Nakajima](https://github.com/snakajima), architect of Windows 95 at Microsoft, and
[Isamu Arimoto](https://github.com/isamu), his long-time development partner. We have built
together since 2015, across four unrelated domains, and the core has been open source every time.

More at the [Singularity Society](https://singularitysociety.org).

MulmoTerminal, MulmoClaude, MulmoChat, GraphAI, SlashGPT and @receptron/laya are MIT.
MulmoCast is AGPL-3.0.
