# Autonomous Commerce AI Prompt Pack — Simple Store (Day 1)

Production-ready, static HTML commerce storefront with Stripe paywall.

**The only things you need to do:**
1. Add your Stripe variables in `index.html`
2. Push to GitHub
3. Connect the repo to Vercel (or Netlify) and deploy

Everything else is complete.

## Setup (5 minutes)

1. **Stripe Client-Only Checkout** (no backend required)
   - Log in to [Stripe Dashboard](https://dashboard.stripe.com)
   - Go to Settings → Checkout → enable “Client-only Checkout”
   - Create a Product (e.g. “Autonomous Commerce AI Prompt Pack”) and a one-time Price
   - Copy the **Price ID** (`price_...`)
   - Copy your **Publishable key** (`pk_test_...` or `pk_live_...`) from Developers → API keys
   - **Never** put the secret key in this frontend code

2. **Edit `index.html`**
   - Open the file
   - Find the `CONFIG` object near the bottom of the `<script>`
   - Replace:
     - `pk_test_YOUR_PUBLISHABLE_KEY`
     - `price_YOUR_PRICE_ID`
     - Adjust `priceDisplay` if needed (e.g. `"$29"`)

3. **Success page download**
   - Edit `success.html`
   - Replace the example download link with your real file URL (Google Drive, S3, Dropbox, Gumroad, etc.)

4. **Deploy**
   - Push the folder to a new GitHub repository
   - Import the repo in Vercel (or Netlify)
   - Deploy (static site — no build step)
   - In Stripe Dashboard → Checkout settings, add your Vercel domain to the allowed domains

## Files
- `index.html` — Landing page + checkout button
- `success.html` — Post-purchase download page
- `hero.jpg` / `product.jpg` — Generated visuals (add these images to the repo root for full visuals)
- This README

## Features
- Fully static, no server required
- Modern dark theme matching AI commerce aesthetic
- One-time payment via Stripe Checkout
- Mobile responsive
- Easy to understand and operate
- Reasonable paywall (free landing, paid instant access)

Agents can later update copy, pricing, or product via the same simple structure.

## Next modules
This is Day 1 of the Autonomous AI Commerce Platform. Future daily modules will add more agent layers, additional stores, and deeper automation while remaining simple to deploy.
