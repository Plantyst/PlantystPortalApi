# Plantyst Portal API - documentation

Public documentation of the Plantyst Portal API: **https://apidocs.plantyst.com**

- [`openapi.yaml`](openapi.yaml) - source of truth (OpenAPI 3.1)
- [`index.html`](index.html) - viewer ([Scalar](https://github.com/scalar/scalar), version pinned from CDN)
- Publishing: GitHub Pages, automatically via [GitHub Actions](.github/workflows/docs.yml) on push to `master` (the deploy runs only after a successful lint)

## Local development

```sh
# preview (http://localhost:8000)
python3 -m http.server 8000

# validate the specification
npx --yes @redocly/cli@2 lint openapi.yaml
```

## Notes

- The documentation was migrated from Apiary in July 2026 (service shutdown 09/2026). The original source [`apiary.apib`](apiary.apib) (API Blueprint) is temporarily kept for reference and will be removed once the transition is verified.
