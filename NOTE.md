## What I picked
The **Bundle Builder** implementation and a **Global JS Foundation Fix**.

## Why it's the highest-impact thing here
1.  **Revenue Drive (AOV):** The Bundle Builder is the single most effective tool for increasing Average Order Value. By incentivizing customers to buy sets (3, 5, or 7+ items), we move from single-item sales to high-ticket transactions.
2.  **Conversion Integrity:** I discovered a systemic bug where `@theme/` imports were breaking all JavaScript functionality across the theme. Fixing this was mandatory to ensure a functional, high-converting experience.
3.  **Cross-Selling:** Using smart keyword detection (`stone`, `guard`, `roll`), I implemented an "Accessories" tab that automatically surfaces high-margin add-ons, further boosting AOV.

## What I did
- **Refactored 40+ JS Files:** Replaced unsupported `@theme/` aliases with browser-native relative paths, restoring site-wide functionality.
- **Implemented Tiered Discounts:** Added a high-value 20% tier (7 items) and ensured discount codes (`BUNDLE-10`, `BUNDLE-15`, `BUNDLE-20`) are passed to checkout.
- **Added Smart Accessory Detection:** Built logic to automatically populate an "Accessories" tab with relevant products to complete a user's set.
- **Premium UX Enhancements:** Added milestone "🎉 UNLOCKED" animations, progress trackers, and sticky summary bars with real-time savings calculations.

## What I'd do next
- **In-Bundle Upsell Popups:** Trigger a modal when a user is 1 item away from a higher discount tier.
- **Inventory Check integration:** Real-time checking to ensure items aren't oversold during the bundle building process.
- **Performance Optimization:** Move all non-critical JS to a single bundled asset to improve LCP.
