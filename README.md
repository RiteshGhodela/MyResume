# Ritesh Ghodela Portfolio

A dark, animated creator-style portfolio landing page built with React, TypeScript, Tailwind CSS, Framer Motion, and Lucide React.

## Tech Stack

- React 18
- TypeScript
- Vite
- Tailwind CSS
- Framer Motion
- Lucide React

## Sections

- Hero
- Marquee showcase
- About
- Services
- Projects
- Contact

## Project Links Used

The project cards use live links from the resume:

- Horloge: https://oc-clock.vercel.app/
- SolowebHQ: https://solowebhq.vercel.app/
- Personal Portfolio: https://riteshportfoliox3h.vercel.app/
- Creative Developer Portfolio: https://creativedesign-puce.vercel.app/
- Designjoy: https://designjoy-xi.vercel.app/

## Getting Started

Install dependencies:

```bash
npm install
```

Run the development server:

```bash
npm run dev
```

Open:

```txt
http://127.0.0.1:5173/
```

## Build

```bash
npm run build
```

The production output is generated in:

```txt
dist/
```

## Preview Production Build

```bash
npm run preview
```

## Windows npm Workaround

If `npm run build` fails with an error like:

```txt
Cannot find module 'C:\Users\rites\AppData\Roaming\npm\node_modules\npm\bin\npm-cli.js'
```

run npm through the installed Node.js npm CLI directly:

```powershell
& "C:\Program Files\nodejs\node.exe" "C:\Program Files\nodejs\node_modules\npm\bin\npm-cli.js" run build
```

Development server workaround:

```powershell
& "C:\Program Files\nodejs\node.exe" "C:\Program Files\nodejs\node_modules\npm\bin\npm-cli.js" run dev -- --host 127.0.0.1 --port 5173
```

Production preview workaround:

```powershell
& "C:\Program Files\nodejs\node.exe" "C:\Program Files\nodejs\node_modules\npm\bin\npm-cli.js" run preview -- --host 127.0.0.1 --port 4173
```

## Deploying

### Vercel or Netlify

Upload or connect the full project repository. Use:

```txt
Build command: npm run build
Output directory: dist
```

### GitHub Pages

For GitHub Pages, upload the contents of `dist`, not the `dist` folder itself.

Correct published structure:

```txt
index.html
assets/
project-shots/
```

If assets do not load on GitHub Pages, set the Vite base path in `vite.config.ts`:

```ts
import { defineConfig } from "vite";
import react from "@vitejs/plugin-react";

export default defineConfig({
  plugins: [react()],
  base: "./",
});
```

Then rebuild and upload the new `dist` contents.

## Contact

- Email: riteshghodela52@gmail.com
- Phone: +91-8770204001
- LinkedIn: https://www.linkedin.com/in/riteshghodela/
- GitHub: https://github.com/RiteshGhodela
