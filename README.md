# GL Consulting — Website v2

Corporate, executive-style, bilingual website for GL Consulting. Built with plain HTML, CSS and JavaScript for free static hosting with GitHub Pages.

## Files
- `index.html` — page structure and content
- `styles.css` — responsive visual design
- `script.js` — Portuguese/English language switch, mobile navigation and contact form
- `config.js` — contact details

## Before publishing
1. Open `config.js`.
2. Replace `SEU_EMAIL@DOMINIO.COM` with the official GL Consulting contact email.
3. Replace `55DDDNUMERO` with the WhatsApp number using country code + area code + number, digits only. Example format: `5542999999999`.
4. If a contact method is not ready, leave its placeholder; the corresponding link will remain hidden.

## Update the existing GitHub Pages repository
1. Extract this ZIP.
2. Open the existing `gl-consulting-site` repository.
3. Choose **Add file → Upload files**.
4. Upload the four website files (`index.html`, `styles.css`, `script.js`, `config.js`) and this `README.md`.
5. Commit directly to `main`, replacing the existing files when GitHub asks.
6. GitHub Pages will publish the update automatically.

Keep all five files in the repository root (not inside a nested folder).

## Contact form limitation
The form uses `mailto:` and opens the visitor's email application. It does not store submissions on a server. A hosted form service or backend would be needed for submissions without an email application.

## Domain / HTTPS
This website package does not change DNS or GitHub Pages domain settings. Keep the existing custom domain configuration. HTTPS certificate provisioning is separate from editing the website files.
