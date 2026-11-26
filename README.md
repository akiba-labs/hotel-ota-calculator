# Hotel OTA Commission Calculator

Free calculator for small hotels: enter rooms, average rate, occupancy, OTA share, and commission to see the yearly cost of Booking.com / Expedia / Agoda commissions and what shifting some bookings to direct would save.

- Full app and API (Vercel): https://hotel-ota-calculator.vercel.app
- Calculator (GitHub Pages): https://akiba-labs.github.io/hotel-ota-calculator/

Educational estimate only. Not financial or accounting advice. Not affiliated with any OTA. No tracking.

```bash
npm install
npm test
npm run dev
npm run build
npm run build:pages
```

`npm run build` is the Vercel app (calculator, JSON API, share pages). `npm run build:pages` writes a static `out/` for GitHub Pages and checks that internal links and assets resolve under `/hotel-ota-calculator`. Server routes stay in the repo; the Pages script only moves them aside for that build.

GitHub settings: **Settings → Pages → Build and deployment → Source: GitHub Actions**. Pushes to `main` deploy with `.github/workflows/pages.yml`. The copy-paste steps for the other tool repos are at the top of `scripts/build-pages.mjs`.
