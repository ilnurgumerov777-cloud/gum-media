# GUM Media

Public product-image storage for GUM marketplace automation.

## Structure

```text
<SKU>/
├── 01.jpg
├── 02.jpg
├── ...
└── manifest.json
```

Images are stored in marketplace order. Each SKU manifest contains public HTTPS
URLs and SHA-256 checksums used by the `marketplace.images.replace` GUM Control
route.

## Safety

This repository is public. Store product media only. Never commit API keys,
tokens, customer data, supplier documents, invoices, or other private files.

A manifest template is available at `templates/manifest.example.json`.
