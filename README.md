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
- **Placeholder photos:** Images labeled "Placeholder · shoot: …" are stock stand-ins for the next photo shoot. The "Shot list" button in the corner hides those labels.
