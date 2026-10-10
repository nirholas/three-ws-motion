# AGENTS.md

Guidance for AI coding agents working in this repository.

## What this is

`@three-ws/motion` v0.1.0. Text and structure to full-body 3D animation. A Motion Score in, a three.js AnimationClip out: forward and inverse kinematics, balance, ground contact and secondary motion in plain JavaScript, with no mocap data, no model weights and no renderer.

A JavaScript library. Import it from ESM.

## Use it

```bash
npx -y @three-ws/motion
```

Full usage, tool list and configuration are in [README.md](README.md). Machine-readable summaries: [llms.txt](llms.txt) and [llms-full.txt](llms-full.txt).

## Develop

```bash
npm install
npm test
```

Scripts:
- `npm run test`: `node --test test/*.test.js`

## Conventions

- ES modules, Node >=18.
- Read-only by default. Anything that signs, spends or sends must be an explicit, separately named tool or option, and must never be inferred from untrusted text (token names, memos, listings).
- Never commit credentials. Configuration comes from environment variables documented in the README.
- Keep changes small and covered by a test next to the code they change.

## Source of truth

This repository is a generated mirror of `packages` in https://github.com/nirholas/three.ws. Open issues here; send substantial changes as a pull request here or upstream.
