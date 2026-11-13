# Case-Senff

## Dashboard

The standalone dashboard is available in [`index.html`](index.html), with its processed data in [`dashboard-data.js`](dashboard-data.js). It provides contract, product, premium, status, cancellation, and daily-registration indicators; data is processed in the browser and requires no build step.

The current data snapshot contains 2,519 insurance contracts registered from November 1–12, 2026, with cancellation information through November 13. The dashboard data is a reduced version of the supplied workbook: it excludes names, CPF numbers, IP addresses, individual identifiers, and free-text cancellation reasons. Reasons and registration origins are grouped into broad categories.

Active and cancelled counts use the workbook status codes `A` and `C`. The cancellation rate is cancelled contracts divided by the filtered contract count; active monthly premium sums only active contracts; average monthly premium is the total premium divided by the filtered contract count.

GitHub Actions deploys the site to GitHub Pages when changes are pushed to `main` or when the workflow is run manually. In the repository settings, open **Pages** and set the publishing source to **GitHub Actions**. After the first successful deployment, the workflow will report the published URL.