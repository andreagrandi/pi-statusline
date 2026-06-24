# @andreagrandi/pi-statusline

Claude-like statusline extension for the [Pi coding agent](https://pi.dev).

It replaces Pi's default crowded footer with a compact line focused on the information I want during everyday coding sessions:

```text
📁 …/Projects/book-corners │ 🌿 branch ✓ │ 🤖 gpt-5.5 🧠 xhigh │ ctx 11% │ 📊 57% (5h) / 50% (7d)
```

## Features

- Hides Pi's default token/cache/cost footer by default.
- Shows path, git branch, model, thinking level, compact context usage, and status chips.
- Defaults to emoji icons and below-editor placement.
- Keeps the configurable `/statusline` overlay, layout controls, icon sets, prompt stash, and fixed-editor options from the upstream extension.
- Consumes `notify:status` chips, including usage chips emitted by `@andreagrandi/pi-codex-usage` and `@andreagrandi/pi-kimi-code-usage`.

## Install

From GitHub:

```bash
pi install git:github.com/andreagrandi/pi-statusline
```

Reload Pi:

```text
/reload
```

## Useful commands

```text
/statusline
/statusline layout
/statusline icons emoji
/statusline placement below
/statusline off
/statusline on
```

## Configuration

Settings are stored in:

```text
~/.pi/agent/andreagrandi-pi-statusline/events.json
```

On first load, this fork migrates an existing Savagelands config from:

```text
~/.pi/agent/savagelands-net-pi-statusline/events.json
```

## Credits

This package is a fork/refactor of [`@savagelands-net/pi-statusline`](https://github.com/savagelands-net/pi-statusline), which is itself a fork of [`@wierdbytes/pi-statusline`](https://www.npmjs.com/package/@wierdbytes/pi-statusline).

Original credits from upstream also mention [`pi-powerline-footer`](https://github.com/nicobailon/pi-powerline-footer) and token-rate logic inspired by [`tok-rate-footer`](https://github.com/Cass67/tok-rate-footer).

Thank you to the original authors and maintainers. This fork keeps the MIT license.
