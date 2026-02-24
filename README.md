# Hit Documentation

Official documentation for [Hit](https://hit.com), a peer-to-peer prediction market powered by Base.

**Live Documentation:** [docs.hit.com](https://docs.hit.com)

## About

This repository contains the complete documentation for Hit, covering:

- **Users Guide**: Trading, deposits, withdrawals, market types, and more
- **Developer Guide**: API reference and integration guides
- **FAQ**: Common questions about the platform

Built with [Mintlify](https://mintlify.com), our docs are written in MDX and configured through `docs.json`.

## Repository Structure

```
├── users/              # User-facing documentation
│   ├── signing-up.mdx
│   ├── trading.mdx
│   ├── market-types.mdx
│   └── ...
├── developers/         # Developer documentation
│   └── quickstart.mdx
├── images/            # Screenshots and assets
├── logo/              # Brand assets
├── docs.json          # Mintlify configuration
├── favicon.svg
└── index.mdx          # Documentation homepage
```

## Local Development

### Prerequisites

- Node.js 18+
- npm or pnpm

### Setup

1. Install the Mintlify CLI globally:

```bash
npm i -g mint
```

2. Clone this repository:

```bash
git clone https://github.com/hit/hit-docs.git
cd hit-docs
```

3. Start the development server:

```bash
mint dev
```

4. Open your browser to `http://localhost:3000`

### Troubleshooting

- **Dev environment not running**: Run `mint update` to ensure you have the latest CLI version
- **Page loads as 404**: Verify you're in a folder with a valid `docs.json` file

## Contributing

We welcome contributions to improve our documentation!

### Writing Guidelines

- Write in second person ("you")
- Keep content concise and scannable
- Include code examples where relevant
- Test all code snippets before submitting
- Use relative paths for internal links
- Add alt text to all images

### MDX Frontmatter

Every `.mdx` file requires frontmatter:

```mdx
---
title: Page Title
description: Brief description for SEO and navigation
---
```

### Making Changes

1. Create a new branch for your changes
2. Make your edits to the relevant `.mdx` files
3. Test locally with `mint dev`
4. Commit with clear, descriptive messages
5. Submit a pull request

### Navigation

To add or modify navigation, edit `docs.json`. The structure follows this pattern:

```json
{
  "navigation": {
    "tabs": [
      {
        "tab": "Tab Name",
        "groups": [
          {
            "group": "Group Name",
            "pages": ["path/to/page"]
          }
        ]
      }
    ]
  }
}
```

## Publishing

Changes merged to the `main` branch are automatically deployed to production via our [Mintlify GitHub app](https://dashboard.mintlify.com/settings/organization/github-app).

## Resources

- [Mintlify Documentation](https://mintlify.com/docs)
- [Mintlify Components](https://mintlify.com/docs/content/components)
- [Hit Website](https://hit.com)
- [Hit on X](https://x.com/Hit)

## Support

For questions about Hit itself, reach out:

- Twitter: [@Hit](https://x.com/Hit)
- Website: [hit.com](https://hit.com)

For documentation issues, please open an issue in this repository.
