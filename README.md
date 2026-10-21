# LASC Record Book Publisher — browser edition

A self-contained static website for GitHub Pages. No Python, Windows executable or server required.

## Publish on GitHub Pages

1. Create a new GitHub repository (for example `lasc-record-book-publisher`).
2. Upload `index.html` and `.nojekyll` to the repository root.
3. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
4. Once published, use the GitHub Pages URL shown in Settings → Pages. It normally has the form `https://YOUR-USERNAME.github.io/lasc-record-book-publisher/`.
5. Share that URL with the designated club publisher. The CSV remains in the browser and is not uploaded to GitHub.

## Operator instructions

1. In Airtable, download the current club records CSV (all records held in one table).
2. Open the publisher website, select the CSV and click **Validate records**.
3. Correct any reported duplicates or invalid data in Airtable, then export again.
4. Click **Open print / Save as PDF**. Select **Save as PDF**, **A4 landscape**, **margins none**, **100% scale**, **background graphics on**, and **browser headers/footers off**.
5. Review the PDF before publishing.

## Reporting rules

- Only Status `Approved` or `Active` is included.
- Reports split SC/LC, Licensed/Unlicensed, Girls/Boys.
- Licensed ages 6 and 7 are excluded from the report.
- Events sorted by stroke then increasing distance.
- Duplicate category keys: Pool, Type, Gender, Age Group, Stroke, Distance.
- Validation errors block publication; raw record names and meet names are rendered as plain text (not HTML).
- No third-party JavaScript or CDN dependencies; you can also open `index.html` directly in Edge or Chrome.
- Printing is handled by the browser. Exact pagination and font rendering may vary slightly between browser versions. Test the first PDF in Edge before delegating.

## Privacy and access

A public GitHub Pages site is publicly accessible. The app contains **no swimmer data**, but anyone with the link can open the publisher. Only CSV files selected by an operator are processed, locally. Do **not** commit CSV exports or generated reports to the public repository.

## Maintenance

Replace `index.html` in the repository to deploy future changes. Keep a backup copy of the last tested version.
