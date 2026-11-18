# Money River

**See where your money is going, from this paycheck to the day you retire.**

[moneyriver.app](https://moneyriver.app) · Free · About 10 minutes · No sign-up · Your numbers never leave your device

![Money River](og-image.png)

## What it is

Money River is a personal finance planner for people in the US. You answer six short steps about your money, and the site turns your answers into a river:

- Your paycheck flows in.
- Bills, spending and interest drain off.
- What you invest keeps growing until you retire.

Most budgeting tools stop at "here's where your money went last month". Money River connects today's paycheck to the long-term outcome, then tells you what to do next, in order, with your own numbers.

## Features

- **Six guided steps:** Today, Paycheck, Bills, Spending, Investing, Your river. The river updates live as you type.
- **Take-home pay estimate:**
  - Federal tax brackets, Social Security and Medicare.
  - State tax for all 50 states plus DC.
  - City and county taxes (NYC, Maryland, Indiana, Pennsylvania and more).
  - California disability insurance (SDI).
- **Debt payoff:** shows what each debt costs you a month and when you'll be debt-free.
- **Retirement plans:** choose to keep investing until you retire, Coast FIRE or FIRE. A "Your number" check shows whether the plan gets there.
- **Your next 3 moves:** a prioritized checklist (emergency fund, employer match, high-interest debt, Roth IRA, 401(k) and more).
- **Downloads:** a two-page plan PDF, a net worth image, and an editable Word version.
- **Plain-English explainers** for every term, from APR to compound growth.

## Privacy by design

Money in someone's own numbers is sensitive, so the site is built so it can't collect them:

- All calculations run in the browser. There is no server, no database, no accounts, and no analytics or cookies.
- Answers live only in the current browser tab and are cleared when it closes, unless the person opts in to "Remember my answers on this device".
- A Content Security Policy blocks the page from sending data to any server.
- Fonts and libraries are self-hosted, so no third party sees visits either.

## Accuracy

- **Federal tax and contribution limits:** 2026 IRS figures, which switch to 2027 automatically on January 1, 2027.
  - Sources: Rev. Proc. 2025-32 and 2026-35, the IRS retirement-limit notices, and the SSA wage base.
- **State and local rates:** 2026 rates from state tax agencies and the Tax Foundation.
- **Projections:** use real (inflation-adjusted) returns and the 4% rule. The assumptions are editable.
- **Checking:** every headline number was verified against independent hand calculations.

## Accessibility

Tested against WCAG 2.1 AA with axe-core, with 0 violations across every step in light mode, dark mode and on phones. The site also supports:

- Full keyboard use.
- Screen reader labels and live announcements.
- 200% zoom and 320px-wide screens.
- Reduced motion.

## How it's built

- One HTML file of plain HTML, CSS and JavaScript, with no framework and no build step.
- The river is drawn as live SVG with its own label-placement logic.
- [jsPDF](https://github.com/parallax/jsPDF) makes the PDF and [docx](https://github.com/dolanmiu/docx) makes the Word file.
- Typefaces: Young Serif and Figtree.
- Hosted on GitHub Pages.

| File | What it is |
|---|---|
| `index.html` | The whole app |
| `privacy.html` | Privacy page |
| `fonts/`, `lib/` | Self-hosted fonts and the PDF and Word libraries |
| `favicon.svg`, `og-image.png` | Tab icon and link-preview image |
| `CNAME`, `robots.txt`, `sitemap.xml` | Domain and search engine settings |

To run it locally, download the repository and open `index.html` in a browser.

## Roadmap

- Partner links for investing and banking accounts, with clear disclosure.
- Cookie-free visit counts.
- A "How we calculate" page.
- A yearly refresh of tax figures each November.

## Disclaimer

Money River is for learning and planning, not financial or tax advice.

---

Designed and built by Jonathan Jeon, with Claude as an AI pair-programmer. © 2026 Jonathan Jeon. All rights reserved.
