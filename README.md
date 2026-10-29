# Aadarsh Singh — Portfolio

The personal portfolio of Aadarsh Singh, built with Next.js. It presents selected
projects, GitHub activity, articles, experience, and a responsive visual
interface.

## Highlights

- Featured project showcases with responsive screenshots and technology badges
- GitHub-powered recent project listing
- Article and case-study pages backed by local content
- Responsive layout with dark, light, and themed color systems
- SEO metadata, sitemap, robots configuration, and web app manifest

## Tech stack

- Next.js 16 and React 19
- JavaScript and JSX
- Sass modules
- Framer Motion and React Intersection Observer
- Jest and Testing Library
- Font Awesome and Devicon

## Getting started

### Requirements

- Node.js 20 or newer
- npm

### Install and run

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the site.

## Available scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the local development server |
| `npm run build` | Create a production build |
| `npm run start` | Serve the production build |
| `npm run lint` | Run the Next.js linter |
| `npm test -- --watch=false` | Run the Jest suite once |

## Updating content

Most portfolio content lives in [`src/content`](./src/content):

- [`src/content/projects/featured.json`](./src/content/projects/featured.json)
  controls the featured project cards and screenshots.
- [`src/content/_settings.json`](./src/content/_settings.json) controls the
  GitHub username and repository metadata.
- [`src/content/footer.json`](./src/content/footer.json) controls social links.
- Page-specific JSON files under `src/content/index`, `articles`, and
  `case-studies` control the corresponding sections.

Place project screenshots and other static assets in [`public/img`](./public/img)
and reference them with a path beginning with `/img`.

## Project structure

```text
src/
  app/          Next.js routes and metadata
  components/   Reusable UI components
  content/     Editable portfolio content
  styles/       Sass modules and design tokens
public/         Static images, fonts, and web app assets
tests/          Unit tests
```

## Deployment

Build the project with `npm run build` and serve it with `npm run start`.
The application is also suitable for deployment on Vercel or another platform
that supports Next.js.

## License

This project is distributed under the MIT License. See
[`LICENSE.md`](./LICENSE.md) for details.
