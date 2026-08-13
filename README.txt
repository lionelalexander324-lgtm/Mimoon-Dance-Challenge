Mimoon Dance Challenge — mobile web package

Files to upload to GitHub Pages / your static host:
- index.html
- assets/ (keep this folder and all files inside it)

Mobile/performance optimizations included:
1. The supplied banner was converted to a lightweight WebP asset while preserving the artwork.
2. The supplied dance video was re-encoded to mobile-friendly H.264/AAC with fast-start enabled.
3. The video is not downloaded on first page load. It starts loading only after the user taps Play.
4. No external fonts, frameworks, icon libraries, or tracking scripts are used.
5. Below-the-fold sections use content-visibility to reduce initial rendering work.
6. Asset filenames include content hashes. When an image/video changes, its filename changes too, which helps prevent stale mobile browser/CDN asset caches.
7. No Service Worker is used, avoiding a common source of stale-page cache problems.
8. HTML includes no-cache meta directives. Note: GitHub Pages/CDN may still briefly cache index.html at the server level after deployment, but versioned assets will refresh as soon as the new HTML is served.

Recommended deployment:
Upload index.html and the assets folder together at the site root.
