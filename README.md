# Case-Senff

## Dashboard

The standalone dashboard is available in [`index.html`](index.html), with its workbook data in [`dashboard-data.js`](dashboard-data.js). It provides Adesões, Cancelamentos, and Comissões views with a navigation menu; data is processed in the browser and requires no build step.

GitHub Actions deploys the site to GitHub Pages when changes are pushed to `main` or when the workflow is run manually. In the repository settings, open **Pages** and set the publishing source to **GitHub Actions**. After the first successful deployment, the workflow will report the published URL.