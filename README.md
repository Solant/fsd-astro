# Astro Starter Kit: Basics

```sh
pnpm create astro@latest -- --template basics
```

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

This project follows [Feature-Sliced Design](https://fsd.how/) methodology. Inside your project, you'll see the following folders and files:

```text
/
├── public/
│   ├── favicon.ico
│   └── favicon.svg
├── src/
│   ├── _pages/                    # FSD pages layer (page implementations)
│   │   └── home/
│   │       ├── ui/                # UI components for the home page
│   │       │   ├── assets/        # Page-specific assets
│   │       │   ├── HomePage.astro
│   │       │   └── Welcome.astro
│   │       └── index.ts           # Public API export
│   ├── pages/                     # Astro routing (thin entry points)
│   │   ├── 404.astro
│   │   ├── 500.astro
│   │   └── home.astro
│   └── shared/                    # FSD shared layer (reusable code)
│       └── layout/
│           ├── Layout.astro
│           └── index.ts
├── astro.config.mjs
├── package.json
├── tsconfig.json
└── pnpm-lock.yaml
```

### Feature-Sliced Design Layers

- **`pages/`** - Astro's file-based routing. These are thin entry points that import from `_pages/`.
- **`_pages/`** - FSD pages layer containing page-specific components and logic, organized by feature.
- **`shared/`** - FSD shared layer with reusable components, utilities, and configurations used across the entire application.

To learn more about the folder structure of an Astro project, refer to [our guide on project structure](https://docs.astro.build/en/basics/project-structure/). To learn more about FSD, visit [fsd.how](https://fsd.how/).

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `pnpm install`             | Installs dependencies                            |
| `pnpm dev`             | Starts local dev server at `localhost:4321`      |
| `pnpm build`           | Build your production site to `./dist/`          |
| `pnpm preview`         | Preview your build locally, before deploying     |
| `pnpm astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `pnpm astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
