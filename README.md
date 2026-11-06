# UWM-Sandbox — Genesys Cloud Web Messaging POC Demo Site

Static GitHub Pages site for the UWM-Sandbox Genesys Cloud POC.

## Files
- `index.html` — demo portal and Genesys snippet placeholder
- `css/styles.css` — responsive UWM-inspired styling
- `js/app.js` — demo tabs, navigation, and customer-journey activity

## Add Genesys Web Messaging
Open `index.html`, find `GENESYS CLOUD WEB MESSAGING DEPLOYMENT SNIPPET`, and paste the deployment snippet directly below that comment.

Use the snippet generated for the Messenger deployment in the **UWM-Sandbox** Genesys Cloud org. Do not commit secrets or OAuth client secrets to GitHub.

## Publish with GitHub Pages
1. Create a GitHub repository, for example `uwm-genesys-poc`.
2. Upload the contents of this folder to the repository root. Keep `css/` and `js/` as folders.
3. In GitHub open **Settings > Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then Save.
6. GitHub will provide an HTTPS URL similar to `https://YOUR-USER.github.io/uwm-genesys-poc/`.
7. Add the resulting demo-site domain/URL to the appropriate allowed-domain configuration for your Genesys Messenger deployment if required by your configuration.

## POC Objects Referenced
- Org: `UWM-Sandbox`
- Knowledge Base: `UWM_POC_Mortgage_KB`
- Digital Bot: `UWM_POC_MortgageAssistant_Bot`
- Queues:
  - `UWM_POC_Broker_Support`
  - `UWM_POC_Underwriting`
  - `UWM_POC_Closing`
  - `UWM_POC_LoanStatus`

## Demo Flow
1. Navigate through Loan Status / Underwriting / Closing sections.
2. Use the Customer Journey demo buttons to create page activity.
3. Launch Genesys Messenger.
4. Complete the customer-information form.
5. Ask a mortgage question and provide a fictitious loan number.
6. Demonstrate Knowledge/self-service.
7. Escalate and verify the bot routing outcome, queue transfer, and agent context/screen pop.

## Important
This site is a POC/demo and is not a production UWM website. Do not enter real borrower, loan, financial, or personal information.

The design is intentionally a simplified static implementation inspired by the structure and visual language of the supplied UWM homepage capture/source. It does not reproduce the production Next.js application or its analytics/privacy/runtime code.
