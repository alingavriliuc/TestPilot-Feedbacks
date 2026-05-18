# Testpilot — Privacy Policy

_Last updated: 2026-05-20_

Testpilot ("the extension") is a Chrome extension that helps developers and QA testers fill, record, and replay HTML form interactions on web pages they are testing. This policy explains what the extension does and does not do with your data.

**Publisher:** Alin Gavriliuc

## Summary

- Testpilot stores **everything locally on your device**.
- Testpilot **does not** send any of your data to us or to any third-party server.
- Testpilot **does not** sell, rent, or share your data.
- Testpilot **does not** include analytics, advertising, tracking, or remote logging.

## What the extension stores

Testpilot uses the browser's `chrome.storage` API to persist data that you create while using the extension. The data stays on your machine (and is synced by Chrome only if you have Chrome Sync enabled for extensions, which is a browser-level setting you control). This data includes:

- **Test profiles** — sets of form field values you create or generate so you can reuse them across forms (for example: a fake name, email, address, phone number).
- **Recorded form sessions** — sequences of form interactions you explicitly choose to record so you can replay them later for testing.
- **Extension settings** — local preferences such as inter-action delay.

You can delete this data at any time from inside the extension UI, or by removing the extension from Chrome (which clears its local storage).

## What the extension accesses on web pages

When you open Testpilot on a tab, its content script can:

- **Read form fields** on the current page in order to detect them and offer autofill / recording.
- **Write values into form fields** when you ask it to autofill or replay a recording.
- **Observe and replay your interactions with form fields** during an active recording or replay session you started.

The extension only acts on a page **after you explicitly open its UI on that page**. It does not read or modify page content in the background, across other tabs, or before you invoke it.

The contents of the pages you test (including any values entered into forms during autofill, recording, or replay) **never leave your device**. They are not transmitted to the extension's publisher or to any third party.

## Permissions and why they are requested

- `activeTab` — to act on the specific tab where you opened Testpilot.
- `scripting` — to inject Testpilot's content script into that tab on demand.
- `storage` — to save your test profiles, recorded sessions, and settings locally on your device.
- Host permissions (`http://*/*`, `https://*/*`) — QA testers work on arbitrary internal and external sites (staging, intranet, third-party SaaS, customer sites), so the set of hosts cannot be enumerated in advance. Host access is used only to read and write form fields on pages where you choose to open Testpilot.

## Data we do not collect

Testpilot does **not** collect, transmit, or have access to:

- Personally identifiable information.
- Health, financial, authentication, personal communications, location, or web history data.
- Analytics, telemetry, or crash reports.
- The content of pages you visit.
- The values you enter into forms.

## Children

Testpilot is a developer/QA tool and is not directed at children under 13.

## Changes to this policy

If this policy changes, the updated version will be published at the URL above with a new "Last updated" date. Material changes will be reflected in the extension's Chrome Web Store listing.

## Contact

For any question about this policy or the extension's data handling, contact Alin.Gavriliuc@fabernovel.ey.com or open an issue in the source repository linked above.
