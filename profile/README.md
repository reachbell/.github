<h1 align="center">
  <a href="https://reachbell.com">
    <img src="https://reachbell.com/favicon.svg" alt="ReachBell" width="72" />
  </a>
  <br />
  ReachBell
</h1>

<p align="center">
  <b>Push, email, WhatsApp, SMS &amp; automations &mdash; one dashboard, one API key, one bill.</b>
</p>

<p align="center">
  <a href="https://reachbell.com"><img src="https://img.shields.io/badge/website-reachbell.com-6366f1?style=flat-square" alt="Website" /></a>
  <a href="https://docs.reachbell.com"><img src="https://img.shields.io/badge/docs-docs.reachbell.com-0ea5e9?style=flat-square" alt="Docs" /></a>
  <a href="https://app.reachbell.com"><img src="https://img.shields.io/badge/dashboard-app.reachbell.com-10b981?style=flat-square" alt="Dashboard" /></a>
  <a href="https://www.npmjs.com/package/@reachbell/sdk"><img src="https://img.shields.io/npm/v/@reachbell/sdk?style=flat-square&label=%40reachbell%2Fsdk&color=f59e0b" alt="npm" /></a>
  <a href="https://status.reachbell.com"><img src="https://img.shields.io/badge/status-live-22c55e?style=flat-square" alt="Status" /></a>
</p>

<p align="center">
  <a href="https://reachbell.com/pricing">Pricing</a> &middot;
  <a href="https://reachbell.com/compare/onesignal-alternative">Compare</a> &middot;
  <a href="https://reachbell.com/templates">Templates</a> &middot;
  <a href="https://reachbell.com/migrate/from-onesignal">Migrate</a> &middot;
  <a href="https://reachbell.com/changelog">Changelog</a>
</p>

---

## What is ReachBell?

ReachBell is a **multi-channel customer engagement platform** for product teams who'd rather ship one integration than juggle three vendors.

- **Web push** &mdash; Chrome, Firefox, Safari, Edge (VAPID)
- **Mobile push** &mdash; Android via FCM, iOS via APNs
- **Email** &mdash; campaigns + transactional on AWS SES
- **WhatsApp &amp; SMS** &mdash; Gupshup, MSG91, or Twilio (BYOK)
- **Automations** &mdash; cross-channel workflows with engagement-aware fallback

Built in &#127470;&#127475; India. Priced in &#x20B9; INR. GST invoices, UPI payments, IST-hours support.

---

## Why teams pick ReachBell

- **&#x20B9; INR-first pricing &mdash; no FX markup.** Pay by UPI, cards, or net banking via Cashfree. GST invoice on every charge. Global teams can pay USD via Stripe.
- **Every channel, one dashboard.** Push + email + WhatsApp + SMS + automations behind a single API key. One segment definition flows everywhere.
- **Real automations on standard plans &mdash; not enterprise-gated.** Welcome series, cart recovery, win-back, smart fallback (push -&gt; email -&gt; WhatsApp). Included on Growth.
- **DPDP- and GDPR-ready out of the box.** Hosted preference center, RFC 8058 one-click unsubscribe, consent records, 90-day audit log.
- **Zero subscriber loss when you migrate.** Import existing VAPID keys; your OneSignal / PushEngage / Webpushr subscribers keep working silently.
- **Honest, exportable.** Your audience stays yours &mdash; documented REST API, OpenAPI spec at `/docs`, CSV export, and per-project VAPID keys.

---

## Get started

```bash
# 1. Sign up at https://app.reachbell.com/register and create a project.
# 2. Install the SDK on your site:
npm install @reachbell/sdk

# 3. Three lines:
```

```js
import { ReachBell } from '@reachbell/sdk';
ReachBell.init({ apiKey: 'rb_live_...' });
await ReachBell.prompt();
```

Then drop `reachbell-sw.js` into your site root and you're sending push.

Detailed integration guides for [React](https://reachbell.com/integrations/react),
[Next.js](https://reachbell.com/integrations/nextjs),
[Vue](https://reachbell.com/integrations/vue),
[WordPress](https://reachbell.com/integrations/wordpress),
[Shopify](https://reachbell.com/integrations/shopify), and
[plain HTML/JS](https://reachbell.com/integrations/html-javascript).

---

## Open-source repos

| Repo | Description | npm / Marketplace |
|---|---|---|
| [`reachbell/sdk`](https://github.com/reachbell/sdk) | Browser SDK (TypeScript, Rollup, CSP-safe widgets) | [`@reachbell/sdk`](https://www.npmjs.com/package/@reachbell/sdk) |
| [`reachbell/react`](https://github.com/reachbell/react) | React bindings &mdash; `<ReachBellProvider>` + hooks | [`@reachbell/react`](https://www.npmjs.com/package/@reachbell/react) |
| [`reachbell/vue`](https://github.com/reachbell/vue) | Vue 3 plugin + composable | [`@reachbell/vue`](https://www.npmjs.com/package/@reachbell/vue) |
| [`reachbell/nextjs`](https://github.com/reachbell/nextjs) | Next.js Script wrapper + server helpers | [`@reachbell/nextjs`](https://www.npmjs.com/package/@reachbell/nextjs) |
| [`reachbell/wordpress-plugin`](https://github.com/reachbell/wordpress-plugin) | WordPress plugin (auto-enqueue + auto-notify on publish) | WordPress.org |
| [`reachbell/community`](https://github.com/reachbell/community/discussions) | Discussions, feature requests, Q&amp;A, showcase | &mdash; |

> The dashboard and backend live in private repos. Issues for the SDKs and plugins are welcome here on GitHub.

---

## Pricing

| Plan | INR / mo | USD / mo | Push subs | Push sends | Emails | Projects |
|---|--:|--:|--:|--:|--:|--:|
| Free | &#x20B9;0 | &#36;0 | 1,000 | 10,000 | 500 | 1 |
| Starter | &#x20B9;999 | &#36;19 | 10,000 | 100,000 | 5,000 | 3 |
| Growth | &#x20B9;2,999 | &#36;59 | 50,000 | 500,000 | 25,000 | unlimited |
| Business | &#x20B9;7,999 | &#36;149 | 200,000 | unlimited | 100,000 | unlimited |

WhatsApp + SMS are BYOK &mdash; pay your provider (Gupshup / MSG91 / Twilio) directly. We don't markup per-message cost. Full details: [reachbell.com/pricing](https://reachbell.com/pricing).

---

## Who's behind ReachBell

Built and operated by **[DotSpheres Technologies Pvt Ltd](https://reachbell.com/about)** &mdash; a small engineering team in Pune, India.

We answer our own support tickets. Decisions about pricing, roadmap, and privacy get made by the people writing the code, not a board.

---

## Get in touch

- **Sales** &mdash; sales@reachbell.com
- **Support** &mdash; support@reachbell.com
- **Security disclosures** &mdash; security@reachbell.com
- **Status** &mdash; [status.reachbell.com](https://status.reachbell.com)
- **Changelog** &mdash; [reachbell.com/changelog](https://reachbell.com/changelog)

<p align="center"><sub>&copy; DotSpheres Technologies Pvt Ltd &middot; Made with care in Pune.</sub></p>
