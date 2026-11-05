# MINNEØATS website: Coral Rose

Homepage concept for MINNEØATS (Direction A, Coral Rose palette). It's a static site: one `index.html` plus the images in `assets/`. There is no build step.

## Run it locally

Pick one of these from the repo folder, then open http://localhost:3000.

```bash
# Node (no install needed)
npx serve -l 3000 .

# or Python 3
python3 -m http.server 3000
```

Open the page through the local server rather than double-clicking `index.html`, so every image and font loads the same way it will in production.

## What's live and what's a placeholder

- **Live checkout:** The "Add to bag" buttons use the store's real Shopify cart links (`minneoats.myshopify.com`), so clicking one starts a real checkout.
- **Proposals:** The subscription (Subscribe & save 10%), the newsletter signup and some copy are proposals. They show a mockup message instead of submitting.
- **Placeholder photos:** Images labeled "Placeholder · shoot: …" are stock stand-ins for the next photo shoot. The "Shot list" button is hidden from visitors. Add `?shots` to the address (for example `http://localhost:3000/?shots`) to show it.

## Files

- `index.html`: the whole site. Pages (Home, Shop, Our story, Events, Wholesale, Donation request) switch by the `#/page` part of the address.
- `site.css`: all shared styles, used by both pages.
- The Minne Club (`#/club`): the hosting box, activities, how it works and The Minne Club, with an example teaser video that uses filler photos. Prices are proposals and ordering is not live.
- `assets/`: images and the logo.

## Growth master plan: status

Every idea on that page is a proposal. Not approved: ending catering, sharing recipes, restricting purchases, brunch kit prices, ambassador counts. Blanks in dashed brackets, like `[to fill]`, are numbers and terms the team has not set. The projections tool starts empty on purpose.

## To confirm before this goes live

- **Shop count:** the site says "14 shelves", but the stockist list names 8 shops.
- **Reviews:** the reviews section is hidden. Add real customer reviews, then remove the `hidden` attribute on `#reviews` in `index.html`.
- **Health notes** for each ingredient and the **140 calories** per serving are marked as draft wording.
- **FAQ:** shipping, shelf life, allergen facility wording, and vegan or gluten-free claims are still bracketed.
- **Events, makers, wholesale terms and the donation policy** are empty templates.
- **Subscription and the 15% welcome offer:** the forms are demos and send nothing. Subscriptions are not connected to Shopify yet.
- **Photos:** confirm every stock image is licensed for use. Two credit Wikimedia Commons (CC BY-SA) and need attribution.
- **Instagram and Facebook** links in the footer point to `instagram.com/minneoats` and `facebook.com/minneoats`. Confirm they are the real pages.
- **Recipes:** Allie and Maria are not releasing recipes. The "Ways to bowl" cards now show only the idea and a "full recipe is for Minne Club members" message. The ingredient lists and steps were removed from the page code. Which recipes members get, and when, is still to be decided.

## Version 2 (combined prototype + master plan)

`site-v2.html` is a separate, noindex page that does not change `index.html`. It uses `site-v2.css`, `site-v2-extra.css` and `site-v2-pages.js`, and it reads images from `assets/`. Open it with `python3 -m http.server 3000` and visit `/site-v2.html`.

What it is: the structure and content of the Spacefast prototype (home, shop, product pages, subscribe and save with a portal preview, our story, catering with a 3-step inquiry, events, find our granola, wholesale, FAQ, contact), rebuilt in the packaging colors with our own layout, plus the master plan as real pages: The Minne Trio (`#/trio`), The Minne Morning Box (`#/box`), The Minne Club (`#/club`) and Gifts.

Also included: a welcome pop-up (15% off the first order) that opens on load once per browser session, an ingredient bowl you hover to see why each ingredient is in the granola, signature and specialty bowl cards, a bundle builder and "Every which way" ideas on the Shop page, "Plan your morning" tools (bowl-name builder, invitation writer, gathering list) on the Club and Morning Box pages, a Donation requests page, and a Follow along area.

Rules kept: no earnings or commissions are shown, full recipes stay members-only, and the cart, forms, pop-up and subscription portal are demos that save nothing and send nothing.

Placeholders left in brackets for Allie and Maria: shipping time and cost, Trio bag sizes, Box portions, gift box prices, catering PDF, policy text, subscription prices, pickup at events, a T-shirt photo, and the Minne Club card's member name and date. The brand story video is an embed of https://vimeo.com/804339516; change the video number in the `player.vimeo.com` address in `site-v2.html` to swap it.

Before launch: confirm licenses for the stock photos (for example the vanilla and pink salt photos), replace the stand-in Instagram tiles with real posts, and rebuild in the platform Allie and Maria choose.
