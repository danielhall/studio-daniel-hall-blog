# Daniel Hall - Personal Blog Sanity Studio

Content management system for [danieljh.uk](https://danieljh.uk) - the personal website and blog of **Daniel Hall**, Solutions Architect. This Sanity Studio provides a streamlined interface for managing blog content and portfolio information.

**Author:** **Daniel Hall**, Solutions Architect  
**Website:** [https://danieljh.uk](https://danieljh.uk)

## About

This Sanity Studio powers the content management for my personal website, providing:

- Blog post creation and editing with rich text support
- Social media link management
- Media asset organisation
- Real-time preview and collaboration
- Version control and draft management

## Content Types

### Blog Posts (`postType`)
The primary content type for technical articles and insights:
- **Title** (required) - The post headline
- **Slug** (auto-generated) - URL-friendly identifier
- **Publication Date** - Defaults to creation date
- **Featured Image** (optional) - Hero image for the post
- **Body Content** - Rich text with code blocks, images, and formatting
- **Meta Description** - SEO optimisation
- **Tags** - Content categorisation

### Social Links (`socialType`)
Management of professional social media profiles:
- Platform name and URL
- Display preferences
- Icon configuration

## Getting Started

### Prerequisites

- Node.js 22.18.0 or higher
- pnpm (recommended) or npm
- Sanity account with project access

### Installation

1. Clone the repository:
```bash
git clone https://github.com/danielhall/studio-daniel-hall-blog.git
cd studio-daniel-hall-blog
```

2. Install dependencies:
```bash
pnpm install
```

3. Set up environment variables:
```bash
cp .env.example .env
```
Configure your Sanity project credentials:
- `SANITY_STUDIO_PROJECT_ID` - Your Sanity project ID
- `SANITY_STUDIO_DATASET` - Dataset name (usually "production")
- `SANITY_STUDIO_HOST` - Studio host configuration

4. Start the development server:
```bash
pnpm dev
```

The studio will be available at [http://localhost:3333](http://localhost:3333).

## Environment Variables

Required environment variables (see `.env.example`):

- `SANITY_STUDIO_PROJECT_ID` - Find this in your Sanity project settings
- `SANITY_STUDIO_DATASET` - Usually 'production' or 'development'
- `SANITY_STUDIO_HOST` - Custom domain or local host for your Sanity Studio

## Project Structure

```
├── schemaTypes/          # Content type definitions
│   ├── index.ts         # Schema type exports
│   ├── postType.ts      # Blog post schema
│   └── socialType.ts    # Social media schema
├── static/              # Static studio assets
├── .env                 # Environment variables (git-ignored)
├── sanity.cli.ts        # CLI configuration
└── sanity.config.ts     # Studio configuration
```

## Scripts

- `pnpm dev` - Start development studio
- `pnpm build` - Build studio for production  
- `pnpm deploy` - Deploy studio to Sanity hosting

## Technologies

- [Sanity.io](https://www.sanity.io/) - Headless CMS platform
- TypeScript - Type-safe schema definitions
- Modern studio UI with real-time collaboration

## Author

**Daniel Hall**  
Solutions Architect  
[https://danieljh.uk](https://danieljh.uk)

## Licence

Copyright © 2025 Daniel Hall. All rights reserved.

This project is provided for portfolio demonstration purposes. See [LICENSE](./LICENSE) for full terms and conditions.