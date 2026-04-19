# Repository Guidelines

## Project Structure & Module Organization
This repository is a Hexo theme. Template markup lives in `layout/`, with shared partials in `layout/_partial/` and page templates such as `index.ejs`, `post.ejs`, `search.ejs`, and `about.ejs`. Static assets are in `source/`, including CSS in `source/css/main.css`, client scripts in `source/js/`, and vendor libraries in `source/lib/`. Theme options are defined in `_config.yml`. Keep new assets close to the feature they support.

## Build, Test, and Development Commands
There is no local build system in this theme repo itself. Typical development happens from the parent Hexo site:

- `hexo clean` removes generated output and cached data.
- `hexo generate` rebuilds the site with this theme.
- `hexo server` starts a local preview server.

If you edit only CSS or EJS, refresh the Hexo preview after each change.

## Coding Style & Naming Conventions
Use 4-space indentation in YAML, EJS, CSS, and JavaScript to match `.prettierrc.yaml`. The configured style is `singleQuote: true`, `semi: false`, and `trailingComma: es5`. Keep file names descriptive and aligned with their role: `layout/friends.ejs`, `source/js/main.js`, `source/css/main.css`. Prefer small, focused changes over broad template rewrites.

## Testing Guidelines
There is no automated test suite in this repository. Validate changes by running the parent Hexo site locally and checking the affected pages in the browser. Verify at least the home page, post pages, TOC behavior, search, tags/categories, and any page touched by the change. For layout fixes, test both desktop and mobile widths.

## Commit & Pull Request Guidelines
Recent commits use short, imperative summaries, often in Chinese, and describe the visible change directly. Follow the same pattern: keep the subject brief and specific, for example `修复 search 页面刷新问题`. Pull requests should explain what changed, why it changed, and which page(s) are affected. Include screenshots or a short screen recording for UI updates.

## Security & Configuration Tips
Avoid committing real API keys or private repository data in `_config.yml`. The file currently contains third-party integration settings, so verify any changes before pushing.
