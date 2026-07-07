# MAXFMS

Project by- Ithish Jonnes

## Run Locally

**Prerequisites:** Node.js

1. Install dependencies:

   ```bash
   npm install
   ```

2. Create a `.env.local` or `.env` file and add any required variables.
   - Do not commit `.env`, `.env.local`, or any files containing secrets to GitHub.
   - No frontend API key is required when using Netlify Forms.

3. Run the app:

   ```bash
   npm run dev
   ```

## Netlify Forms Setup

1. When you deploy to Netlify, the `contact` form is automatically processed as long as the form markup includes `data-netlify="true"` and a `form-name` field. No frontend API key is required.

2. Netlify deploy settings:

   - Build command: `npm run build`
   - Publish directory: `dist`

3. Netlify Forms will collect submissions in the Netlify dashboard. If you want email notifications, configure them in your Netlify site settings.

## What to Upload to GitHub

Upload the source and configuration files only. Do not upload generated or local files containing secrets.

- `package.json`, `package-lock.json` / `pnpm-lock.yaml`, `tsconfig.json`, `vite.config.ts`
- `.gitignore`, `.env.example`, `README.md`
- `src/` folder and any project assets needed for the app
- `server.ts`, `contact-submissions.json` should not be uploaded if it contains user data
- `node_modules/`, `dist/`, and `.env*` should never be committed

## Production / Vercel

 - No frontend API key is required for Netlify Forms.
- Do not commit your real API key into source control.
