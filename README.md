[README.md](https://github.com/user-attachments/files/31033761/README.md)
# Modern Login/Signup Component

A ready-made, dark-themed authentication card for React projects, with an animated WebGL dot-grid background and a Sign In ⇄ Sign Up toggle. Built to drop straight into a **React + shadcn/ui + Tailwind CSS + TypeScript** project.

![stack](https://img.shields.io/badge/React-TypeScript-blue) ![stack](https://img.shields.io/badge/shadcn%2Fui-Tailwind-black)

## Features

- 🌌 Animated WebGL dot-grid background, rendered with a custom GLSL shader via Three.js
- 🔁 Built-in Sign In / Sign Up toggle (local `useState`, no routing required)
- 🔐 Email field + Google / GitHub / Apple buttons (inline SVG icons, no image assets needed)
- 🎨 Dark theme, fully self-contained inline styles — works even without Tailwind configured
- 🧹 Clean WebGL teardown on unmount (no leaked renderers/contexts on route changes)

## Project structure

```
modern-login-signup/
├── SKILL.md                        # Claude Skill definition (see "Using this as a Claude Skill" below)
├── README.md                       # This file
└── assets/
    ├── modern-login-signup.tsx     # The component
    └── demo.tsx                    # Minimal usage example
```

## Requirements

- React + TypeScript
- A shadcn/ui-structured project (components under `components/ui/`) — run `npx shadcn@latest init` if you don't have one yet
- Tailwind CSS installed (the component doesn't use Tailwind classes itself, but lives in `components/ui/` alongside your other shadcn components by convention)
- No `three` npm package needed — Three.js is loaded at runtime from a CDN to avoid SSR/bundler issues (e.g. in Next.js App Router)

## Manual installation

1. Copy `assets/modern-login-signup.tsx` into `components/ui/modern-login-signup.tsx` in your project.
2. (Optional) Copy `assets/demo.tsx` anywhere you want a quick usage example, e.g. `app/demo/page.tsx`.
3. Import and render it:

```tsx
import Component from "@/components/ui/modern-login-signup";

export default function LoginPage() {
  return <Component />;
}
```

## Using this as a Claude Skill

This folder is also packaged as a [Claude Skill](https://docs.claude.com) (`modern-login-signup.skill`). Install it and Claude will automatically:

- Check whether your project has shadcn/Tailwind/TypeScript set up (and walk you through it if not)
- Copy the component into the right place following shadcn conventions
- Explain the CDN-based Three.js loading pattern so it doesn't get "fixed" into a broken `import`
- Ask the follow-up questions that matter before calling the integration done (see below)

## ⚠️ Before shipping this to production

The component is visual scaffolding, not a finished auth flow. Before you ship it:

- [ ] **Wire up the forms** — both `onSubmit` handlers currently just call `e.preventDefault()`. Connect them to your real auth provider, a mock, or a callback prop.
- [ ] **Replace the placeholder logo** — the avatar currently shows the initials `"JS"`.
- [ ] **Decide on placement** — the component renders full-viewport (`height: 100vh`); confirm whether it belongs on a dedicated `/login` route or inside a modal.

## License

Add the license that applies to your project here.
