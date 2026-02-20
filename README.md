# Tailwind CSS Best Practices

Stop your AI agent from generating Tailwind CSS v3 code. 20+ rules for v4 syntax, CSS-first config,
modern utility patterns, and common anti-patterns agents produce.

## Install

### Cursor IDE

```
/add-plugin tailwind-best-practices
```

### Claude Code

```
/plugin install tailwind-best-practices
```

### Skills only (any agent)

```bash
npx skills add ofershap/tailwind-best-practices/tailwind-best-practices
```

Or copy `skills/` into your `.cursor/skills/` or `.claude/skills/` directory.

## What's Included

### Skills

- **tailwind-best-practices** - Stop your AI agent from generating Tailwind CSS v3 code. 20+ rules
  for v4 syntax, CSS-first config, modern utility patterns.

### Rules

- **best-practices** - Always-on rules that enforce current Tailwind CSS v4 patterns

### Commands

- `/audit` - Scan your codebase for Tailwind CSS anti-patterns

## Why This Plugin?

AI agents are trained on data that includes outdated Tailwind patterns. This plugin ensures your
agent uses Tailwind v4 best practices. Agents commonly get wrong:

1. **tailwind.config.js** - v4 uses CSS-first @theme; agents keep generating JavaScript config
2. **bg-opacity-50, text-opacity-25** - v4 uses inline opacity: bg-red-500/50, text-white/80
3. **@tailwind directives** - v4 uses @import "tailwindcss"; agents output the old three-line setup
4. **bg-gradient-to-r** - v4 prefers bg-linear-to-r and bg-linear-45 for gradients
5. **!important placement** - v4 puts ! at the end (flex!) not the start (!flex); agents use the old
   syntax
6. **CSS variables in arbitrary values** - v4 requires bg-(--var) not bg-[--var]; agents use square
   brackets
7. **Commas in grid/object arbitrary values** - v4 requires underscores:
   grid-cols-[max-content_auto]

## License

MIT
