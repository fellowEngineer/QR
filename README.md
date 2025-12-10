# QR Generator

A Next.js app for generating QR codes with a focus on flexibility. The current UI is minimal while the core QR plumbing is being built out. Planned improvements include color controls, sizing, and downloads.

## Features

-   Instant QR rendering with React and `react-qr-code`
-   Next.js 16 app router setup (ready for client-side controls)
-   Clear roadmap for customization (colors, size, format export)

## Roadmap

-   Input source: URL, text, or any string payload
-   Style controls: foreground/background color, margin, rounding
-   Size controls: set width/height together (square) or with padding
-   Export: download as PNG, SVG, PDF; copy to clipboard
-   Accessibility: label input, ARIA for form controls

## Future Plans: Barcode Generator API Actor

-   Output formats: PNG, SVG, PDF for server-side and batch use
-   Barcode standards: UPC, EAN, Code 128, QR, Data Matrix
-   Appearance controls: colors, fonts, sizing to match branding
-   Batch processing: create multiple barcodes in one request
-   Cloud storage: deliver and archive generated assets automatically
-   QR error correction: improve readability and data integrity
-   Validation checks: confirm payload compatibility with the selected format

## Getting Started

1. Install dependencies

```bash
npm install
```

2. Run the dev server

```bash
npm run dev
```

3. Open http://localhost:3000 to view the app.

## Scripts

-   `npm run dev` – start Next.js in development
-   `npm run build` – production build
-   `npm start` – run the production server after build
-   `npm run lint` – lint with the Next.js config

## Tech Stack

-   Next.js 16
-   React 19
-   React QR Code (`react-qr-code`)
-   TypeScript
-   Tailwind CSS 4 (via `@tailwindcss/postcss`)

## Development Notes

-   Entry page is `app/page.tsx`
-   Global styles live in `app/globals.css`
-   Layout and metadata are defined in `app/layout.tsx`

## Contributing

Issues and PRs are welcome. Please run `npm run lint` before submitting changes.
