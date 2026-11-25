# Performance optimization notes

- Existing WebP images were recompressed (quality 80, WebP method 6) and resized where their display size did not need the original dimensions.
- Images in the Work and About sections now use lazy loading and asynchronous decoding.
- The navbar logo now has explicit width and height attributes.
- Design, copy, routes, colors, layout, and animation styles were left unchanged.

Approximate public asset sizes:
- Before: 18.52 MiB
- After: 2.63 MiB
- Reduction: 15.89 MiB (about 86%)

Please run `npm install` and `npm run build` locally before deploying. A Lighthouse retest is recommended after deployment.
