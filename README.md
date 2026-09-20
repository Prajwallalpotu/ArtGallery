# Himanshi Kadu — The Weekend Artist

A responsive React gallery built with Vite, Tailwind CSS, custom editorial styling, and Lucide icons.

## Run locally

```sh
npm install
npm run dev
```

Open http://localhost:5173. Build for deployment with `npm run build`; the output is `dist/`. Run `npm run preview` to preview the production build.

## Update the collection

Edit `src/data/artworks.json`. Each painting has an `id`, `title`, `category`, `status` (`available` or `sold`), `image`, and `description`. Put optimized images in `public/artworks/` and use a path such as `/artworks/painting-1.webp`.

All 37 supplied paintings are included. **Titles, category assignments, descriptions, and sold/available statuses are demonstration content and must be confirmed by Himanshi before launch.** The artist introduction is draft copy. No prices, dimensions, or materials have been invented; visitors ask the artist directly for those details.

The Instagram destination is configured in `src/main.jsx`. Enquiry buttons open the artist's profile; they do not send messages automatically. The studio section uses the supplied photos and links to Instagram, rather than claiming to display a live feed or embedded reels.

The site has no database, checkout, or server dependency. Filters, search, pagination, artwork dialogs, mobile navigation, keyboard focus restoration, and reduced-motion preferences work client-side. Fonts are loaded from Google Fonts with system fallbacks. Original source images remain in `images/`; smaller WebP copies are in `public/`.

## Verification

- `npm run build` passes.
- The collection has 37 unique IDs and valid local image paths.
- Browser visual checks require a connected browser or computer-use permissions in the current environment.
