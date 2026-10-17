# Arjun's Birthday Surprise

A premium 10-route React birthday experience for Arjun from Aryan. The routes are:

`/`, `/story`, `/roast`, `/gallery`, `/cake`, `/quiz`, `/letter`, `/wishes`, `/surprise`, and `/finale`.

## Run locally

1. Install current Node.js (it includes npm): https://nodejs.org/
2. In this folder, run:

   ```powershell
   npm install
   npm run dev
   ```

3. Open the local address Vite prints (normally `http://localhost:5173`).

To make a production build, run `npm run build`, then `npm run preview`.

## Make it personal

- Most visible copy can be clicked and edited in the browser for a quick preview. For permanent changes, edit `src/App.tsx`.
- Replace gallery images in `public/assets/photos/`; keep the filenames or update the `photos` list near the top of `src/App.tsx`.
- The supplied optional audio is `public/assets/birthday-track.m4a`. It never autoplayes; the gold music button starts it only after a click.
- Quiz progress uses this browser's local storage. Use **Replay quiz** to reset it.
- The story, roast, letter, quiz, and surprise intentionally use editable prompts instead of invented personal details.

## Deploy online

The simplest choice is Vercel:

1. Put this folder in a GitHub repository and push it.
2. At https://vercel.com/new, import that repository.
3. Leave the build command as `npm run build` and publish the deployment.
4. Vercel provides a shareable URL. Its Vite hosting supports the app's direct routes.

Netlify is also suitable: import the repository, use `npm run build` as the build command and `dist` as the publish directory. Add a SPA redirect rule if using a static host that does not already fall back to `index.html`.
