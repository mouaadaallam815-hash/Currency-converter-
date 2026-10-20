# Currency Converter — starter project

A responsive, multilingual currency converter (Arabic, French, English) with:
- Currency list based on the rate provider's available currencies
- Instant conversion and swap button
- Popular exchange rates against MAD
- Manual refresh and automatic refresh every 30 minutes
- Last-updated timestamp and cached last-known rates
- Progressive Web App (PWA) shell for installable browser use

## Run locally
Because the app fetches live data, serve the folder through a local web server (opening index.html directly may block requests):
- Python: `python -m http.server 8000`
- Open `http://localhost:8000`

## Exchange-rate source
The starter uses `https://open.er-api.com/v6/latest/USD`. It is an open-access endpoint with provider-defined update cadence and terms. It is not a guaranteed tick-by-tick feed. Check the provider's current terms, attribution requirements, supported currencies and availability before public release. The app displays indicative rates only, not bank cash-buy/sell rates.

## Before Google Play release
This is the source project, not a signed Android APK/AAB.
1. Host the app over HTTPS and test on real Android devices.
2. Replace/confirm the data provider and show its attribution/terms as required.
3. Add privacy policy and a public contact email.
4. Complete Play Console app content, data safety, target SDK and testing requirements.
5. Package it as an Android app (for example with Capacitor and Android Studio), configure app ID/version/icon, test offline/error states, and sign a release Android App Bundle (AAB).
6. Verify current Google Play requirements before submission.

The app does not collect account details and does not execute payments or money transfers. If analytics or ads are added later, update the privacy policy and Play Console disclosures accordingly.
