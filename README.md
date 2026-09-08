# Kajal Enterprises Product Catalog

Static GitHub Pages catalog with:
- `/catalog` — product catalog
- `/catalog/k101`, `/k102`, etc. — individual product pages

## Products
K101, K102, K106, K111, K111F, K113, K122, K131, K132, K201, K202, K203, K213, K301, K302

## Deploy
Upload all files to the repository used for `kajalenterprises.github.io` and enable GitHub Pages.

The site uses client-side routing, so `/catalog` and product URLs work as GitHub Pages paths. If GitHub Pages serves the root `index.html`, the included `404.html` redirects deep links back through the SPA.

## Add product images
Put images in `assets/products/` using the product code, e.g. `k101.jpg`. If no image exists, the product page shows a clean placeholder.


### Deep-link fix
The included `404.html` preserves direct product URLs such as `/catalog/k101` and restores them through `/catalog`, so clicking or opening a product URL on GitHub Pages renders the correct product page instead of an error.
