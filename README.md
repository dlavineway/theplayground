# Lavineway Portfolio

This project is an online portfolio that shows my work, thinking, and technical range. It runs on PHP and includes a small CMS so I can update content without touching code.

## Domains

- Primary site: https://lavineway.com
- Playground site: https://theplayground.ws (for demos, utilities, and experiments)

## What’s Inside

Your portfolio has three parts:

### 1. Main Site
- About page
- Case studies
- Technical library
- Contact form
- Search and tagging
- Markdown support for all content

### 2. Admin Panel
- Create and edit pages
- Manage case studies
- Upload images
- Draft mode
- Simple auth

### 3. Playground
- The playground hosts small tools and experiments. Examples:
- JSON formatter
- JWT helper
- Log parser
- Markdown-to-folder converter
- Any other demos you want to expose publicly

## Tech Stack
- PHP 8.x
- Slim or Laravel (decide based on how heavy you want the stack)
- Tailwind CSS
- Alpine.js
- SQLite or MySQL
- Composer for dependencies

## Local Setup
- Clone the repo.
- Copy `.env.example` to `.env`.
- Set DB path or credentials.
- Run composer install.
- Start the local server:
```bash
php -S localhost:8080 -t public
```

## Deployment
The sites run on your shared hosting provider. Deployments are simple:

- Push to main.
- GitHub Actions builds and pushes files via SFTP to each domain.
- A small deploy script clears cache and updates the database if needed.

## Content Structure
```bash
/content
  /about
  /case-studies
  /library
  /playground
/public
/resources
/routes
/views
```
- Markdown lives in /content.
- Templates live in /views.
- Playground tools live under /public/tools.

## Roadmap
- Add dark/light mode
- Add version history for pages
- Add RSS feed
- Add API endpoint for pushing new articles from GitHub
- Add diagram support (Mermaid)