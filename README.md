# Global Energy Intelligence — Interactive Analytics Portfolio

## What this project does
An interactive browser dashboard for exploring historical oil, natural-gas and coal production/consumption records. It includes:
- Dataset, country and year filters with reset.
- KPI cards that respond to filters.
- Historical trend, country ranking and record-coverage charts.
- Automatically generated insights: change between first and last available annual averages, highest annual-average year, and top country in the latest selected year.
- Searchable historical data preview and CSV export for the current dataset/country/year filters.
- Responsive dark-theme layout for desktop and mobile.
- Data validation and duplicate country-year handling in the supplied cleaned files.

## Run locally
1. Extract this ZIP into a folder.
2. Open the folder in VS Code.
3. Install/enable **Live Server**.
4. Right-click `index.html` → **Open with Live Server**.
5. Keep all six CSV files in the same folder as `index.html`.

Do not double-click `index.html` if the browser blocks local CSV fetching.

## Publish online (recommended: GitHub Pages)
1. Sign in or create an account at https://github.com/.
2. Click **New repository**. Name it `global-energy-intelligence-dashboard`.
3. Choose **Public**, then create the repository.
4. In the repository, click **Add file → Upload files**.
5. Upload `index.html` and all six CSV files from this folder. You may also upload this README and the quality report.
6. Click **Commit changes**.
7. Open the repository's **Settings → Pages**.
8. Under **Build and deployment**, choose **Deploy from a branch**.
9. Select branch `main` and folder `/(root)`, then click **Save**.
10. Wait a few minutes. The live URL will look like:
   `https://YOUR-GITHUB-USERNAME.github.io/global-energy-intelligence-dashboard/`
11. Open the live URL in an incognito/private window to verify it works before sharing. The URL is only an example until GitHub Pages has deployed your repository.

Important: upload the six CSVs beside `index.html`; otherwise the charts will not load. This project uses Chart.js and Three.js from public CDNs, so the page needs internet access.

## LinkedIn sharing
- Add the deployed GitHub Pages URL to the project link on LinkedIn; do not use `http://127.0.0.1:5500/...`, because that address only works on your computer.
- Also add the GitHub repository URL so viewers can inspect the source and datasets.
- Record a short 30–60 second screen recording showing dataset selection, filters, charts, insights, search and CSV export.
- Use a clear project title such as **Global Energy Intelligence Dashboard | Interactive Historical Energy Analytics**.
- Describe this as a portfolio/learning project and state the data period accurately.

## Methodology and limitations
- The dashboard calculates annual averages from the country-level records available in the selected dataset. It does not calculate global total energy consumption or production.
- The "period change" insight compares the first and last available annual averages in the currently filtered records. It is descriptive, not causal.
- Dataset coverage varies by country and year, so changing country coverage can affect the annual average.
- Oil, gas and coal datasets use different source units; do not compare their raw numeric values directly across energy types.
- The globe is a decorative animation, not a geographic map, and its dots are not actual country locations.
- The supplied CSVs do not carry enough source metadata in the files to confidently identify the original publisher. Before public release, identify and cite the original source and verify all unit definitions. Do not claim the data is live.
- This project is an interactive analytics portfolio project, not a production-grade market data service.

## Included files
- `index.html` — dashboard application.
- Six CSV datasets — required by the app.
- `data_quality_report.csv` — row counts and cleaning checks from the supplied dataset preparation.
