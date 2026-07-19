# Waypoint — Vercel direct-key build

This build calls OpenRouteService directly from `index.html` using the embedded key supplied for testing.

## Deploy

1. Upload this folder to the Git repository connected to Vercel.
2. Commit and push.
3. Redeploy the project.

No `ORS_API_KEY` Vercel environment variable is required for this version.

## Important security note

The OpenRouteService key is visible in the deployed page source and browser developer tools. Anyone visiting a public deployment can copy it. For a private test deployment this may be acceptable, but for a public production site use the server-proxy version and rotate the exposed key afterward.
