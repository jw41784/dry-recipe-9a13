# CLAUDE.md - Development Guide for eudex.io

## Commands
- Build: `npm run build` (astro build)
- Dev server: `npm run dev` (astro dev)
- Preview: `npm run preview` (astro build && wrangler dev)
- Type check: `tsc --noEmit`
- Deploy: `npm run deploy` (astro build && wrangler deploy)

## Site Information
- Site name: eudex.io
- Purpose: Distributed leadership training and assessment platform
- Primary color: #482532 (burgundy)
- Secondary color: #607D8B (blue-gray)
- Background color: #FFFAF0 (off-white)

## Code Style
- TypeScript with strict mode enabled
- Components: PascalCase (BaseHead.astro, HeaderLink.astro)
- Variables/functions: camelCase
- Constants: UPPER_SNAKE_CASE
- Content validation: Use Zod schemas in content.config.ts
- Imports: Group by external/internal/types
- Format with consistent spacing (2 space indentation)

## Project Structure
- Content collections in src/content/
- Page components in src/pages/
- Shared components in src/components/
- Layouts in src/layouts/
- Global styles in src/styles/
- Images in public/img/

## Key Pages
- Home: Landing page with service overview
- About: Information about the organization's approach
- Survey: Distributed team maturity assessment
- Resources: Future content library (coming soon)

## Typography
- Headings: Playfair Display (serif)
- Body text: Lato (sans-serif)
- Font sizes should be responsive using rem units

## UI/UX Guidelines
- Mobile-first, responsive design
- Interactive elements should have hover states
- Maintain consistent spacing throughout components
- Use subtle animations for interactions (transforms, transitions)
- Cards and containers should use subtle shadows for depth

## Error Handling
- Handle user-facing errors gracefully with helpful messages
- Use TypeScript types to prevent runtime errors
- Form validation should provide clear user feedback