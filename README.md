# Badvel ISP Autonomous NOC Monitoring Engine

Single-file React dashboard (no build step) for the Badvel ISP network, backed by Google Sheets through an Apps Script web app.

- `index.html` - the dashboard
- `apps-script/Code.gs` - paste into Extensions > Apps Script in the spreadsheet, then deploy as a Web app
- `.github/workflows/pages.yml` - deploys `index.html` to GitHub Pages on every push to `main`

## Connect to Google Sheets
1. Spreadsheet > Extensions > Apps Script > replace Code.gs with `apps-script/Code.gs`.
2. Deploy > New deployment > Web app. Execute as: Me. Who has access: Anyone.
3. Open the deployed dashboard > Settings > paste the `/exec` URL > Save and sync now.

The dashboard runs on built-in mock data until a URL is saved.
