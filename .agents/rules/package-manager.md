# Package Manager Rules

**IMPORTANT: Use pnpm exclusively as the package manager**

- Always use `pnpm` commands (e.g., `pnpm install`, `pnpm add`, `pnpm remove`)
- Never mix package managers - do NOT use `npm`, `yarn`, or any other package
  manager
- If you encounter `package-lock.json` or `yarn.lock`, do not use them - only
  `pnpm-lock.yaml` is valid
- All scripts should use `pnpm run` instead of `npm run` or `yarn`
- When adding dependencies: `pnpm add <package>`
- When adding dev dependencies: `pnpm add -D <package>`
- When removing dependencies: `pnpm remove <package>`
