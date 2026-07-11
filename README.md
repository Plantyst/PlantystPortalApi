# Plantyst Portal API - dokumentace

Veřejná dokumentace Plantyst Portal API: **https://apidocs.plantyst.com**

- [`openapi.yaml`](openapi.yaml) - zdroj pravdy (OpenAPI 3.1)
- [`index.html`](index.html) - viewer ([Scalar](https://github.com/scalar/scalar), pinovaná verze z CDN)
- Publikace: GitHub Pages, automaticky přes [GitHub Actions](.github/workflows/docs.yml) při pushi do `master` (deploy proběhne jen po úspěšném lintu)

## Lokální práce

```sh
# preview (http://localhost:8000)
python3 -m http.server 8000

# validace specifikace
npx --yes @redocly/cli@2 lint openapi.yaml
```

## Poznámky

- Dokumentace byla v červenci 2026 migrována z Apiary (ukončení služby 09/2026). Původní zdroj [`apiary.apib`](apiary.apib) (API Blueprint) je dočasně ponechán pro referenci a bude odstraněn po ověřeném přechodu.
