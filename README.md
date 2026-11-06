# Portfolio

Personal portfolio of Stefano D'Ambrosio, front-end developer based in Berlin.

**Live:** [stedamb.dev](https://www.stedamb.dev)

## Features

- Single-page portfolio with project showcase, smooth scrolling (Lenis) and carousels (Embla)
- Contact form validated with React Hook Form and Zod, delivered through a serverless endpoint using [Resend](https://resend.com)
- SEO essentials: sitemap, structured metadata, privacy and cookie policy pages
- Accessible UI components built on Radix primitives

## Tech stack

| Area      | Tooling                                  |
| --------- | ---------------------------------------- |
| Framework | Astro 7 with the Vercel adapter          |
| UI        | React 19 islands, Radix UI, Lucide icons |
| Styling   | Tailwind CSS 4                           |
| Forms     | React Hook Form, Zod                     |
| Email     | Resend                                   |
| Packages  | pnpm                                     |

## Getting started

Requires Node.js 22 or later and [pnpm](https://pnpm.io).

```bash
pnpm install
cp .env.example .env   # add your Resend key and recipient address
pnpm dev
```

The dev server runs at <http://localhost:4321>.

### Environment variables

| Name             | Purpose                                     |
| ---------------- | ------------------------------------------- |
| `RESEND_API_KEY` | Resend API key used by `/api/contact`       |
| `CONTACT_EMAIL`  | Address that receives contact form messages |

## Scripts

| Command        | Description                                          |
| -------------- | ---------------------------------------------------- |
| `pnpm dev`     | Start the dev server                                 |
| `pnpm build`   | Type-check with `astro check`, then build for Vercel |
| `pnpm preview` | Preview the production build                         |
| `pnpm format`  | Format the codebase with Prettier                    |

## Project structure

```text
src/
├── components/   # Layout, sections, blocks, SEO and UI components
├── data/         # Site config, projects and routes
├── pages/        # Home, policies, sitemap and the /api/contact endpoint
└── styles/       # Global styles and Tailwind theme
```

## License

Code is released under the [MIT License](LICENSE). Text, images and other content are © Stefano D'Ambrosio and are not covered by the license.
