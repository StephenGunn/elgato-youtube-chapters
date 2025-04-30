# Elgato Timestamps to YouTube Chapters Converter

A utility application that converts Elgato Stream Deck timestamp files into properly formatted YouTube chapter markers.

## Technology Stack

- **Framework**: SvelteKit
- **UI Library**: Svelte 5 with runes
- **Hosting**: Cloudflare Pages
- **Language**: TypeScript

## Features

- Drag and drop or file selection for timestamp files
- Automatic conversion of Elgato timestamp format to YouTube chapter format
- Timestamp offset adjustment
- First chapter automatic formatting to 00:00
- Client-side processing (no server uploads)

## Development Setup

### Prerequisites

- Node.js (v18+)
- npm or pnpm

### Installation

1. Clone the repository

   ```bash
   git clone https://github.com/StephenGunn/elgato-youtube-chapters.git
   cd elgato-youtube-chapters
   ```

2. Install dependencies

   ```bash
   npm install
   # or
   pnpm install
   ```

3. Start the development server

   ```bash
   npm run dev
   # or
   pnpm dev
   ```

4. Open your browser and navigate to `http://localhost:5173`

## Building for Production

```bash
npm run build
# or
pnpm build
```

## Deployment

This application is configured for deployment to Cloudflare Pages:

1. Create a new Cloudflare Pages project
2. Connect your GitHub repository
3. Configure the build settings:
   - Build command: `npm run build` or `pnpm build`
   - Build output directory: `.svelte-kit/cloudflare`
   - Environment variables: Add any required environment variables

## License

[MIT](LICENSE)
