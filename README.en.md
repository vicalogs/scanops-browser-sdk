<div align="center">
  <img src="https://scanops.niigel.com/logo.svg" alt="ScanOps" width="96" height="96" />

  # ScanOps Browser SDK

  [中文](README.md) | **English**

  [🔗 Live demo](https://scanops.niigel.com) · [📖 Full documentation](https://scanops.niigel.com/en/docs)
</div>

**Give your web app a pair of eyes that can read codes.** No app download, no mini-program redirect — a few lines of code open the camera in the browser and decode QR codes and mainstream 1D barcodes. Decoding happens entirely on the user's own device: no frame is uploaded, nothing goes through the cloud.

- **Fast, no jank** — decoding runs in a dedicated Web Worker thread and never blocks the UI, so checkout counters and pick-list scanners stay responsive
- **Accurate, no false triggers** — built-in multi-frame confirmation and tracking mean the same code is never counted twice, tuned for high-frequency scanning workflows
- **Ten formats out of the box** — QRCode, Code128, Code39, Code93, EAN13, EAN8, UPC-A, UPC-E, ITF, Codabar
- **Framework agnostic** — native TypeScript/ESM; plain HTML/Vue call `ScanOps` directly, and React apps can use the `ScanOpsView` component
- **Licensed per customer** — the core locator model is delivered encrypted and scoped to your registered domains, keeping commercial licensing under control

npm package: [`@niigelog/scanops`](https://www.npmjs.com/package/@niigelog/scanops)

## Getting started

Installation, deploying the runtime files, plain and React integration examples, and the options and events are covered in the documentation:

👉 **[ScanOps documentation](https://scanops.niigel.com/en/docs)**

Before you integrate:

- **A license key is required** — keys are issued per domain and only work on registered domains, including local development origins. Without authorization the camera still previews, but nothing is decoded.
- **HTTPS or localhost is required** — browsers only expose the camera in a secure context.
- **ESM only** — the React component needs React 18.2 or 19.
