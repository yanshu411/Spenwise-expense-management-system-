# SpendWise — Personal Expense Management System

A clean, responsive personal-finance tracker for recording everyday income and expenses. Built as a portfolio project with **HTML, CSS, and vanilla JavaScript**.

> **Edition in this repository:** a **static browser-based application**. The earlier Python Flask + SQLite version is a separate implementation. This version does **not** have a Python backend, accounts, or cloud database.

## Features

- Add income and expense transactions with a title, amount, category, and date.
- View **balance**, **total income**, and **total expenses** in an at-a-glance dashboard.
- Browse transactions in descending date order and delete individual entries.
- See a category-by-category expense visualization.
- **Export JSON backups** and **import them later**.
- Responsive UI for mobile and desktop browsers.
- Form input validation and safe DOM text rendering.

## Technology

| Layer | Technology |
| --- | --- |
| Frontend | HTML5, CSS3, JavaScript |
| Data storage | `localStorage` in the current browser profile |
| Hosting | Netlify, Cloudflare Pages, GitHub Pages, or any static web host |
| Build tools | None needed |

## Try the site locally

1. [Download the repository](https://github.com/yanshu411/Spenwise-expense-management-system-/archive/refs/heads/main.zip) and extract it, or clone it:

   ```bash
   git clone https://github.com/yanshu411/Spenwise-expense-management-system-.git
   ```

2. Double-click **`index.html`**. The dashboard opens in your browser.
3. Record an income transaction and an expense transaction, then refresh to see that they are saved in that browser.

**No Python, npm, Node.js, XAMPP, or SQL database is required for this static edition.**

## Deploy from GitHub to Netlify

1. Open [Netlify](https://app.netlify.com/) and choose **Add new project → Import an existing project → GitHub**.
2. Select **`yanshu411/Spenwise-expense-management-system-`**.
3. Set **Base directory** to repository root (leave it blank).
4. Leave **Build command** blank; set **Publish directory** to `.` (repository root).
5. Deploy. Netlify will serve the root **`index.html`** and create a public URL.

A root `netlify.toml` is provided with the same publish settings.

### Alternative: manual upload

Drag the root folder containing `index.html` onto [Netlify Drop](https://app.netlify.com/drop), or upload it to Cloudflare Pages as a static site.

## Important: how data is stored

SpendWise saves transaction records to **browser localStorage**, not to the GitHub repository or a server.

- **Each browser/device keeps separate records.** There is no synchronization between two phones or computers.
- Clearing site data, changing browsers, using Incognito, or uninstalling the browser could remove records.
- Anyone with access to the same browser profile may see the locally stored financial information.
- **Use Export Backup regularly** and store the downloaded JSON securely. Importing a backup **replaces** the current local records.
- This project is not suitable for sensitive or business-critical financial record keeping without an authenticated backend and secure backups.

Read [SECURITY.md](SECURITY.md) before sharing with others.

## Sample transactions

| Title | Type | Category | Amount |
| --- | --- | --- | ---: |
| Monthly allowance | Income | Salary | ₹10,000 |
| Groceries | Expense | Food | ₹1,500 |
| Metro | Expense | Transport | ₹500 |

Expected balance: **₹8,000**.

## Project structure

```text
.
├── index.html          # Complete static website and application logic
├── README.md           # Project documentation
├── SECURITY.md         # Data storage and privacy notes
├── netlify.toml        # Netlify Git deployment config
├── .gitignore          # Ignore sensitive/local files
├── LICENSE             # MIT license
└── SpendWise_Netlify.zip # Original uploaded archive (retained for reference)
```

## CV / LinkedIn

**SpendWise — Personal Expense Tracker:** Developed a responsive expense-management website using HTML, CSS and JavaScript. Implemented transaction tracking, income/expense dashboards, category analytics, local persistence, and JSON backup/import.

## Ideas for future development

- Optional user accounts and private cloud storage
- Monthly budgets and spending alerts
- Filters by date/category and richer charts
- Automated backups and sync across devices
- Accessibility and automated browser tests

## License

MIT — see [LICENSE](LICENSE).
