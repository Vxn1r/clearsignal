# ClearSignal

**A calmer internet starts here. Stay a little harder to fool.**

ClearSignal is a small, privacy-minded web app that checks pasted messages and URLs for common warning signs and explains what a person should review before trusting them.

- **Live app:** https://vxn1r.github.io/clearsignal/
- **Portfolio:** https://vxn1r.github.io/
- **Source:** https://github.com/Vxn1r/clearsignal

## What it does

- Checks user-pasted text and URLs for a limited set of common warning patterns.
- Explains the warning signals in plain language.
- Supports English and Hindi interface text.
- Runs its current checks in the browser; the pasted content is not sent to a ClearSignal analysis server.
- Includes a web-app manifest and service worker for installability and static-asset caching after the first visit.

## Important limitations

ClearSignal is an **early beta**, not a complete phishing, malware, or fraud-detection service.

Its checks are rule-based and limited. It can miss malicious content, and it can flag harmless content. A result with no obvious warning signals does **not** mean a message or URL is safe. Do not use ClearSignal as the only basis for financial, account, or security decisions.

When something looks suspicious, do not open its link or share sensitive information. Verify through the service's official app or website, or contact the organization using details you already know are genuine.

## Privacy

The current analysis runs locally in the user's browser. ClearSignal does not send the pasted message or URL to a ClearSignal backend. The service worker caches static app files; it is not a cloud scanning service.

## Run locally

The app is a static web project. You can open `index.html` in a browser for basic testing. For PWA install and service-worker behavior, serve the folder from a local development server or deploy it over HTTPS.

The main files are:

- `index.html` — interface, translations, and rule-based checks
- `manifest.json` — installable web-app metadata
- `sw.js` — static asset caching
- `icon.svg` — app icon

## Languages

The current interface is available in **English and Hindi**. Other languages shown in the selector are marked as coming soon and are not currently supported.

## Feedback

Found a false positive, a missed warning pattern, or an accessibility issue? Open a GitHub issue with a synthetic example. Please do not include real passwords, private messages, personal data, or active malicious links.

## Project status

Early beta · Built as a learning project · Improvements and careful testing are ongoing.
