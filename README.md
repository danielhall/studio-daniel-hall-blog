# Daniel Hall Portfolio - Sanity Studio

This is the Sanity Studio configuration for [danieljh.uk](https://danieljh.uk), Daniel Hall's portfolio website. The studio provides a content management interface for managing blog posts and other website content.

## Content Structure

### Blog Posts (`postType`)
The main content type is `post`, which includes:
- Title (required)
- URL-friendly slug (auto-generated from title)
- Publication date (defaults to creation date)
- Featured image (optional)
- Body content (rich text with block content)

## Getting Started

1. Clone the repository
2. Copy `.env.example` to `.env` and fill in your Sanity project credentials
3. Install dependencies:
```bash
npm install
```
4. Start the development server:
```bash
npm run dev
```

## Environment Variables

The following environment variables are required:

- `SANITY_STUDIO_PROJECT_ID`: Your Sanity project ID
- `SANITY_STUDIO_DATASET`: Your dataset name (usually "production")
- `SANITY_STUDIO_HOST`: The studio host name

## Technologies

- [Sanity.io](https://www.sanity.io/) - Headless CMS
- TypeScript - For type-safe schema definitions
- Modern studio UI with real-time collaboration

## Project Structure

```
├── schemaTypes/       # Content type definitions
│   ├── index.ts      # Schema type exports
│   └── postType.ts   # Blog post schema
├── .env              # Environment variables (git-ignored)
├── sanity.cli.ts     # CLI configuration
└── sanity.config.ts  # Studio configuration
```

## License

Copyright © 2025 Daniel Hall. All rights reserved.