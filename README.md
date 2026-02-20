# Tailwind CSS Best Practices

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Skills](https://img.shields.io/badge/skills.sh-tailwind--best--practices-blue)](https://skills.sh/ofershap/tailwind-best-practices)

Stop your AI agent from generating Tailwind CSS v3 code. 12 rules for Tailwind v4 syntax, CSS-first
config with @theme, modern utility patterns, and the anti-patterns every agent produces.

> AI coding assistants (Cursor, Claude Code, Copilot, Codex) are trained on Tailwind v3 data. They
> generate `tailwind.config.js`, `@tailwind` directives, `bg-opacity-50`, and other patterns that
> don't exist in Tailwind CSS v4. This plugin fixes that.

## Install

### Cursor / Claude Code / Windsurf

```bash
npx skills add ofershap/tailwind-best-practices
```

Or copy `skills/` into your `.cursor/skills/` or `.claude/skills/` directory.

## What's Included

| Type    | Name                      | Description                                                                                  |
| ------- | ------------------------- | -------------------------------------------------------------------------------------------- |
| Skill   | `tailwind-best-practices` | 12 rules covering @import, @theme, opacity, gradients, container queries, @utility, and more |
| Rule    | `best-practices`          | Always-on behavioral rule that enforces v4 patterns on every file                            |
| Command | `/audit`                  | Scan your codebase for Tailwind v3 anti-patterns                                             |

## What Agents Get Wrong

AI agents consistently produce these outdated Tailwind patterns:

| What the agent writes                   | What v4 actually uses                     |
| --------------------------------------- | ----------------------------------------- |
| `tailwind.config.js` with JS objects    | CSS-first `@theme { }` in your stylesheet |
| `@tailwind base; @tailwind components;` | `@import "tailwindcss";`                  |
| `bg-opacity-50`, `text-opacity-25`      | `bg-red-500/50`, `text-white/80`          |
| `bg-gradient-to-r`                      | `bg-linear-to-r`, `bg-linear-45`          |
| `!flex`, `!bg-red-500`                  | `flex!`, `bg-red-500!`                    |
| `bg-[--brand-color]`                    | `bg-(--brand-color)`                      |
| `grid-cols-[max-content,auto]`          | `grid-cols-[max-content_auto]`            |

## Related Plugins

- [shadcn-best-practices](https://github.com/ofershap/shadcn-best-practices) - shadcn/ui component
  patterns, forms, theming
- [typescript-best-practices](https://github.com/ofershap/typescript-best-practices) - TypeScript
  5.x strict patterns
- [sveltekit-best-practices](https://github.com/ofershap/sveltekit-best-practices) - Svelte 5 runes
  and SvelteKit patterns

## Author

[![Made by ofershap](https://gitshow.dev/api/card/ofershap)](https://gitshow.dev/ofershap)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/ofershap)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat&logo=github&logoColor=white)](https://github.com/ofershap)

## License

MIT
