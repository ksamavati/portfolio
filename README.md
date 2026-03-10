# Kayvon Samavati — Portfolio

A personal portfolio website built with Gulp, Bootstrap, and jQuery. It showcases projects, skills, resume, and contact information across multiple pages, and is deployed to Netlify.

## Live Site

Hosted on Netlify — auto-deploys from the `theme/` build directory on every push.

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Build | Gulp 4 |
| CSS | SCSS → Autoprefixer → CSS |
| Frontend | Bootstrap 3, jQuery 2, Slick, Isotope |
| HTML | `gulp-file-include` partials |
| Linting | JSHint |
| Dev Server | Browser-sync (live reload) |
| Deploy | Netlify / GitHub Pages |

## Project Structure

```
portfolio/
├── source/          # Editable source files
│   ├── *.html       # Page templates
│   ├── partials/    # Shared HTML includes (header, footer, nav)
│   ├── js/          # JavaScript source
│   ├── scss/        # SCSS stylesheets
│   ├── images/      # Images and assets
│   └── plugins/     # Third-party libraries
├── theme/           # Compiled build output (do not edit directly)
├── gulpfile.js      # Gulp task definitions
├── netlify.toml     # Netlify build and header config
└── package.json     # Dependencies and scripts
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v12 or later recommended)
- npm

### Install dependencies

```bash
npm install
```

### Start development server

```bash
npm run dev
```

This compiles SCSS, processes HTML partials, lints JS, and starts a Browser-sync server at `http://localhost:3000` with live reload on every file change.

### Build for production

```bash
npm run build
```

Compiled, processed assets are written to the `theme/` directory.

### Deploy to GitHub Pages

```bash
npm run deploy
```

Runs the production build and pushes the output to the `gh-pages` branch.

## Pages

| Page | Description |
|------|-------------|
| Home | Hexagon navigation hub |
| Welcome | Extended biography and introduction |
| About | Skills, specializations, and work status |
| Works | Project portfolio with category filtering (JavaScript, Java, Photoshop, Unity) |
| Services | Services offered |
| Resume | CV / résumé |
| Testimonials | Client testimonials carousel |
| Contact | Contact form and contact information |

## Configuration

- **Build output directory:** `theme/`
- **Dev server port:** `3000` (Browser-sync default)
- **Netlify publish directory:** `theme` (see `netlify.toml`)
- **JavaScript lint rules:** `.jshintrc`
- **Editor settings:** `.editorconfig`

## License

This project is based on the [Phantom Bootstrap Portfolio Template](https://themefisher.com/) by ThemeFisher, licensed under the [MIT License](https://opensource.org/licenses/MIT).
