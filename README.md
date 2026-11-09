# Memory & Autonomy Engine

SillyTavern third-party extension for the local Memory & Autonomy Engine (MAE).

## Install

Install this repository from SillyTavern with the URL:

```text
https://github.com/uers123/memory-agency.git
```

Then restart SillyTavern and open **世界状态面板** from the extensions menu.

## Runtime requirement

The extension connects to the local MAE service, normally `http://127.0.0.1:8787/api/mae`. Run `st-card-writer` first with `npm install` and `npm start`. The extension can be installed without the service, but it will report a connection error until the service is running.

## Compatibility and security

The service exposes `GET /api/compatibility` with `apiVersion`, `serverVersion`, and SillyTavern support metadata. No model API key is stored in this extension; keep keys in the local server's `.env.local`.
