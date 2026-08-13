Mimoon Dance Challenge — optimized mobile web package

Included:
- index.html
- assets/hero.[hash].webp
- assets/poster.[hash].webp
- assets/dance.[hash].mp4

Mobile/performance optimizations:
1. Hero JPG converted to lightweight WebP and resized for mobile-retina use.
2. Poster converted to lightweight WebP.
3. Video converted to a true 16:9 landscape MP4 (640×360) and compressed with H.264 + faststart.
4. Video source is injected only after the user taps Play, so the MP4 is not downloaded on initial page load.
5. Asset filenames contain content hashes, which reduces stale-cache problems after updates.
6. No external fonts, JS frameworks, icon libraries, or third-party assets.
7. Safe-area support and mobile text-size stabilization included.
8. WhatsApp links use noopener/noreferrer when opening a new tab.

Deployment:
Upload index.html and the assets folder together. Do not rename individual asset files unless you also update index.html.
