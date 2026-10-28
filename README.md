# CloudAccess Website Source

Frontend source for the CloudAccess website currently associated with https://cloudaccessdigital.com.

## Files
- `index.html` — page structure
- `styles.css` — site styling
- `app.js` — catalogue, cart, and test checkout integration
- `cloudaccess-logo.png` — site logo
- `DEPLOY-UPDATE.txt` — deployment and safety notes

## Local preview
Open `index.html` in a browser. For best results, serve the folder with a simple local web server.

## Deployment notes
The frontend currently calls the separate Cloudflare Worker at `https://cloudaccess-payments.crmongole.workers.dev` for the Razorpay test integration. Do not put payment secrets in frontend files. The current checkout is a test integration and automatic secure guide delivery is not implemented; do not accept live payments until production credentials, secure fulfilment, and failure/refund paths are implemented and tested.

## Publish to GitHub
Create a repository named `cloudaccess-website` under your GitHub account, then upload these files to the repository root. A public repository URL would be `https://github.com/sfdcanil/cloudaccess-website` if that exact repository is created under `sfdcanil`.
