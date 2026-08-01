# Condition Inspection Log v1.5.0 - Aviation Maintenance Inspection Logging 2026

> **Condition Inspection Log is a browser-based Progressive Web App for organizing aircraft maintenance inspections, records, photos, estimates, and logbook data, with offline support in version 1.5.0.**

[![Platform](https://img.shields.io/badge/Platform-Web%20browser-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v1.5.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/evan-hayesppy8837/aviation-inspection-log?style=flat-square)](https://github.com/evan-hayesppy8837/aviation-inspection-log)

---

<p align="center">
  <a href="https://evan-hayesppy8837.github.io/aviation-inspection-log/">
    <img src="https://img.shields.io/badge/Download-Condition%20Inspection%20Log%20Latest-brightgreen?style=for-the-badge" alt="Download Condition Inspection Log">
  </a>
</p>

> **[Download Condition Inspection Log v1.5.0](https://evan-hayesppy8837.github.io/aviation-inspection-log/)**

---

[Download Latest Build](https://evan-hayesppy8837.github.io/aviation-inspection-log/)

---

## Aviation Inspection Records in One Workspace

Condition Inspection Log supports aviation maintenance teams and owners who need organized documentation throughout an aircraft inspection. The browser-based workspace combines annual and condition inspection checklists with aircraft records, owner requests, squawks, estimates, and owner-ready reports.

The app remains usable when connectivity is unavailable by keeping information in browser-based IndexedDB storage. It also includes inspection photo capture, Tesseract-powered OCR for receipts and parts prices, Google Drive backup and restore, and installable Progressive Web App support for quick access from a device home screen.

---

## What It Includes

- Record annual and condition inspections using checklists aligned with ICA guidance and 14 CFR Part 43 Appendix D.
- Add pre-work walkaround photographs to an inspection.
- Keep owner requests, squawks, and estimated work details together.
- Monitor recurring inspections, Airworthiness Directives, and Service Bulletins.
- Produce reports intended for aircraft owners.
- Store airframe, engine, and propeller logbook records.
- Continue working offline through browser IndexedDB storage.
- Use Tesseract WebAssembly OCR to help enter receipt and parts-pricing information.
- Back up application records to Google Drive and restore them when needed.
- Move data in and out using JSON import and export.
- Protect the local interface with an access-code screen and install the app through service-worker caching.

---

## Getting Started

The hosted application runs in a modern web browser:

1. Open [Download Latest Build](https://evan-hayesppy8837.github.io/aviation-inspection-log/).
2. Wait for the application assets to finish loading locally.
3. If supported by the browser, select its install option to place the app on the home screen.
4. Configure an access code if you want the lock screen enabled.

To use a local copy of the repository:

```bash
git clone https://github.com/evan-hayesppy8837/aviation-inspection-log.git
cd REPO
```

Start the files with any static web server and visit the local URL it provides. Offline features and service-worker registration may not function when the project is opened directly as a file, so use `http://localhost` or HTTPS.

---

## Inspection Workflow

A standard session can be organized as follows:

1. Launch the app and enter the configured access code.
2. Select an existing aircraft or create a new aircraft record.
3. Upload pre-work walkaround photos and fill in the inspection information.
4. Work through the ICA and 14 CFR Part 43 Appendix D checklist.
5. Enter owner requests, squawks, estimates, recurring items, ADs, and SBs.
6. Add completed work to the airframe, engine, or propeller logbook as appropriate.
7. Apply OCR to receipts or parts-price information when useful.
8. Generate an owner report and export the records as JSON if required.
9. Back up the current records to Google Drive or restore an earlier backup.

---

## Data and Settings

Records and application settings live in the browser's local IndexedDB storage. The access code is managed within the app. Google Drive backup and restore options are handled through the related integration workflow.

For moving or preserving records, create a JSON export before deleting browser data or switching browser profiles. The exported file can then be imported into another local instance of the application.

---

## Requirements

- A modern browser with JavaScript enabled.
- IndexedDB and service-worker support for offline storage and installable-app behavior.
- Internet access for the first hosted load, Google Drive actions, and other online resources.
- Enough browser storage for inspection records, photographs, and exported data.
- A browser environment that can run Tesseract WebAssembly for OCR.
- Google Drive access for cloud backup and restoration.

---

## Frequently Asked Questions

### Does it support offline use?

Yes. Browser caching and IndexedDB allow inspection information to remain available without an ongoing network connection. The first visit and service-worker setup may still need internet access.

### Where are records kept?

The app stores local records in the browser's IndexedDB database. JSON export and Google Drive backup provide additional ways to preserve the data before clearing site storage or changing profiles.

### What is the process for backing up or transferring records?

Export a JSON file for a local backup, or use the Google Drive backup and restore functions. To move records manually, import the JSON file into another application instance.

### What information can the OCR feature read?

Tesseract WebAssembly OCR helps with entering receipt details and parts pricing. Always check the recognized values before saving them to an inspection record.

### How can I add the app to a device?

Visit the hosted build in a compatible browser. When the browser offers an install or add-to-home-screen command, use that option. The service worker caches the resources used by the installed app experience.

### Why is offline mode unavailable?

Make sure the app was opened through a supported web address, allow the initial online load to finish, and verify that service workers and IndexedDB are permitted by the browser. After the first successful online visit, reopening the app can make its cached resources available.

### How does the access-code lock work?

Condition Inspection Log includes an access-code screen that controls entry to the local app interface. Configure or change the code in the application settings, and retain it for later access.

### How do I receive the latest version?

Open the hosted build using the download link to reach the current release. After an update is published, reload the application while connected to the internet so its cached resources can refresh.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
