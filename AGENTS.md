# Guidance for Coding Agents

## Project and Scope

This guidance applies to the entire repository. The project contains the static
**VoteEasy** website at <https://voteeasy.aiki-it.de>, not the VoteEasy web
application itself. The website is built with Hugo and the Beautiful Hugo theme.

## Project Structure

- `site/`: Hugo project; run Hugo commands from this directory.
- `site/hugo.toml`: Website configuration, navigation and theme import.
- `site/content/_index.md`: Home page.
- `site/content/page/`: Content pages and demo documentation.
- `site/content/post/`: Blog posts.
- `site/static/`: Images, videos, PDFs and other files served without modification.
- `site/layouts/_partials/`: Local customisations to the head and footer.
- `site/go.mod` and `site/go.sum`: Hugo module dependencies.
- `site/themes/beautifulhugo/`: An additional Git submodule containing the theme.
  The active theme import uses the Hugo module in `site/hugo.toml`.
- `site/public/`: Generated output; do not edit manually or commit.
- `README.md`: Installation, development and theme guidance.
- `run.sh`: Starts the local development server with Git information enabled.
- `updateTheme.sh`: Updates the theme module.
- `copyUpstream.sh.example`: Template for building and uploading to the hosting provider.

## Development and Validation

A recent Hugo Extended release and Go are required. The Go version must meet or
exceed the requirement in `site/go.mod`.

From the repository root:

```sh
# Development server with Git information
./run.sh

# Production build for validation
(cd site && hugo --gc --minify --enableGitInfo)
```

Alternatively, start the development server with `cd site && hugo serve`.
Validate the production build after changes to content, configuration or templates.
For visible changes, also inspect the affected pages in a browser, particularly
navigation, images, shortcodes and mobile presentation. Mention any checks not
performed or missing prerequisites in the final report.

There is no dedicated automated test suite in this repository. The Cypress tests
mentioned in a blog post belong to a separate repository for the web application.

## Change Conventions

- Keep changes small and limited to the requested task; do not overwrite existing
  changes made by others.
- Write website content mainly in German and preserve the style of the relevant
  page. The configured default language is currently `en`; do not change it
  incidentally.
- Markdown pages use YAML front matter between `---` lines. Preserve existing
  metadata and Hugo shortcodes; use suitable neighbouring pages as templates for
  new pages.
- Preserve existing URLs, filenames and menu links wherever possible. When
  changing them, also check internal links and `site/hugo.toml`.
- Place static files under `site/static/`. For example,
  `site/static/img/demo/abstimmung.png` is referenced as `/img/demo/abstimmung.png`.
- Follow `site/.editorconfig`: spaces rather than tabs, LF line endings, a final
  newline, UTF-8 for Markdown/JavaScript and four-space indentation for TOML.
- Prefer local layouts for theme customisations rather than modifying the theme
  submodule.
- Do not commit generated files, local IDE files, credentials or `.DS_Store`.
- Do not introduce additional external resources or tracking services unless
  requested; the configuration favours self-hosted resources.

## Dependencies and Deployment

Only update the theme when this is part of the requested task:

```sh
./updateTheme.sh
(cd site && hugo mod tidy)
```

Review changes to `site/go.mod` and `site/go.sum`, then build the website. Do not
inadvertently mix module and submodule updates.

Do not upload or deploy without an explicit request. `copyUpstream.sh.example`
includes a step that deletes generated output and an `scp` upload; it is not a
local validation routine. A customised `copyUpstream.sh` is deliberately excluded
from Git.
