## Hey, I'm Henry 👨‍💻

I build full-stack systems—backend APIs, mobile apps, frontend experiences—whatever's needed to ship a product that people actually use. Right now I'm writing Spring Boot backends for two different products, React for a live edtech platform, and React Native for my own finance app. I've shipped to production across fintech, agritech, and edtech, mostly owning things end-to-end.

Based in Nigeria, working remotely. I care about systems that don't break, code that's maintainable six months later, and products that feel good to use.

## 🛠️ Stack I use

**Backend** — Java, Spring Boot, Spring Security, PostgreSQL, Flyway, JWT, OAuth2  
**Mobile** — React Native, Expo, Expo Router, NativeWind, Zustand, TanStack Query  
**Frontend** — React, Next.js, Tailwind CSS  
**Tools** — Docker, Git, GitLab CI, EAS, Firebase, PostHog

## 🏗️ Things I've built

### Rubi — Personal finance that actually makes sense
A cross-platform finance app I'm building because most personal finance tools either treat you like a spreadsheet expert or hide everything behind "smart" automation that makes no sense. Rubi's somewhere in between—detailed when you need it, invisible when you don't.

Designed and shipped the complete backend: 75+ REST endpoints covering accounts, multi-currency transactions, budgets, savings goals, recurring payments, reports, and a daily check-in streak system. Multi-currency was the interesting challenge—automatic exchange rate caching with direct, inverse, and USD-bridged lookup paths, balance integrity enforcement on every transaction, structured conflict errors when currencies don't align.

The React Native client's built with Expo Router, Zustand for state, TanStack Query for server sync. Flash-free auth hydration (no login screen flicker on cold start), native Google OAuth with PKCE, Skia aurora card backgrounds, Reanimated streak animations. OTA updates via Expo Updates, PostHog analytics, tier-based feature limits (Free/Pro).

Auth's stateless JWT with dual token delivery—HTTP-only cookie for web, response body for native—so the same backend serves both without platform-specific hacks. Google OAuth implementation has provider separation to prevent account takeover (the "sign in with Google" flow that lets attackers link their Google account to your email if you signed up with a password first—most apps get this wrong).

`Java` · `Spring Boot` · `PostgreSQL` · `React Native` · `Expo` · `TypeScript`

---

### Divyd — [Live on the App Store](https://apps.apple.com/ng/app/divyd/id6755341606) · 5.0★
Bill splitting and P2P payments. Built the entire mobile app from scratch—auth (email/PIN/Google OAuth), multi-step onboarding, bill creation (equal/custom/recurring splits), in-app wallet, friends & groups, KYC flows, push notifications.

The hard parts weren't the features, they were the edge cases: session management with idle timeout and background/foreground token revalidation, making sure users don't restore a stale session after force-quitting the app. OTA updates with route-aware safeguards so updates never interrupt an active payment or split flow (imagine pushing an update while someone's mid-transaction—disaster).

PostHog analytics with session replay, Bugsnag for crashes, FCM for push. Deployed to production via EAS with environment-separated build profiles.

`React Native` · `Expo` · `TypeScript` · `Firebase` · `PostHog` · `EAS`

---

### Aviarai — AgriTech poultry management platform
I own several core modules here with full responsibility for data correctness, business logic, and production reliability. Built the inventory management module for egg and feed stock—dispatch workflows, operational tracking, user-facing views. Designed the task management system with automated notifications and task generation tied to vaccination schedules and dependent modules. Implemented egg production KPI calculations with regional benchmarking across farms to surface actionable insights.

The interesting part's been integrating AI-driven features and making sure the Smart Feed logic and eligibility checks produce accurate outputs that the rest of the product can trust. When you're dealing with farm operations, incorrect data isn't just a bug—it's someone's livelihood.

`Spring Boot` · `PostgreSQL` · `REST APIs`

---

### AceBuddy — [Live EdTech platform](https://acebuddy.so)
I built and maintain AI-powered features using Server-Sent Events (SSE) for real-time UI updates and interactive learning experiences. Own the marketplace module end-to-end—reliability, usability, features that support user retention. Improved onboarding flows to reduce friction and increase activation rates.

Originally a short-term contract that got extended because delivery speed and code quality turned out to matter.

`React` · `Next.js` · `Tailwind CSS` · `SSE`


## 📫 Let's talk

I'm open to remote opportunities where I can own something meaningful—backend systems, mobile apps, full-stack work, whatever needs building. If you're working on something interesting and need someone who ships, reach out.

**Email:** devthenry@gmail.com  
**LinkedIn:** [henry-taiwo](https://linkedin.com/in/henry-taiwo-b60198313/)  
**GitHub:** You're already here
