# The Jar Co. — Small-Batch Sauce Brand Site (Demo)

A warm, playful brand site for a sauce company, modeled on the sauce-jar concept reel: rust-orange hero, cream panels, chunky sticker-style cards with hard shadows, "What's Inside" and "Why the Jar Matters" story sections, a working shop and recipe content that sells the jars.

**Live structure:** `index.html` (everything — CSS + JS embedded) + `images/` (11 real food photos). No build step, no dependencies. Open `index.html` or deploy the folder to any static host.

## Features

- **Hero** — oversized display type with an outlined word, arched photo, a rotating "Small Batch • Big Flavor" sticker badge (SVG), floating review chip and dashed feature tags.
- **What's Inside** — dark story panel with animated ingredient proportion bars that fill on scroll (72% tomatoes down to 3% smoked chili).
- **Why the Jar Matters** — cream section with a tilted, hard-shadow photo and three benefit cards (flavor stays true, sealed at peak, return-and-refill program).
- **Shop with working basket** — 4 products with honest heat ratings (dot meter), badges and prices. Slide-in basket: quantities, remove, free-shipping threshold progress ($35), shipping math, validated checkout (name + email) and an order confirmation with order number.
- **Recipes** — 4 recipe cards tagged with time, difficulty and which jar they use — content marketing that moves product.
- **Newsletter** — "10% off your first order" banner in the style of the original concept, with email validation and an instant success state revealing the JAR10 code.
- Marquee strip, scroll reveals, fully responsive, mobile nav.

## Make it yours (buyer customization)

- **Products:** the `PRODUCTS` array at the top of the `<script>` drives the whole shop — name, price, heat (1–4), photo, badge and description. The basket reads from the same array.
- **Recipes:** edit the `RECIPES` array the same way.
- **Photos:** replace files in `images/` keeping filenames, or update the `img` paths in the data arrays.
- **Palette:** rust/cream/pink/yellow live as CSS variables in `:root` (`--rust`, `--cream`, `--pink`, `--yellow`) — change four values to re-brand.
- **Prices & shipping:** the free-shipping threshold ($35) and flat rate ($4.95) are in `renderCart()` in the "CART" script section.

## Tech

Vanilla HTML/CSS/JavaScript in one file. Fonts: Bricolage Grotesque + Archivo (Google Fonts). Photos: Unsplash (free to use). Checkout and newsletter are front-end demos — connect them to Shopify/Mailchimp/etc. to sell and send for real.
