# Dracula theme for Claude Code

A [Dracula](https://draculatheme.com) custom theme for the [Claude Code](https://claude.com/product/claude-code) CLI.

## Install

1. Copy `dracula.json` into your Claude Code themes directory:

   ```bash
   mkdir -p ~/.claude/themes
   curl -fsSL https://raw.githubusercontent.com/atkrv/dracula-claude-code/main/dracula.json \
     -o ~/.claude/themes/dracula.json
   ```

2. In Claude Code, run `/theme` and pick **Dracula**.

Claude Code watches `~/.claude/themes/` and reloads on change — no restart needed. Requires Claude Code v2.1.118 or later. See the [custom themes documentation](https://code.claude.com/docs/en/terminal-config#create-a-custom-theme) for how Claude Code theming works.

## A note on colors

The theme uses `base: dark-ansi`. Claude Code renders body text, markdown accents, and code syntax through your **terminal's ANSI palette**, while theme tokens control the UI chrome (input borders, mode indicators, diff backgrounds, spinners, rainbow). For the full Dracula look, pair it with a Dracula-colored terminal — for example one of the [Dracula terminal themes](https://draculatheme.com/) (iTerm2, Alacritty, Ghostty, …).

## License

[MIT](LICENSE)
