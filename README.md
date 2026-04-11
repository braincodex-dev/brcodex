# Brain Codex

**Neurobioscience & Philosophy**

Static site for [braincodex.com.br](https://braincodex.com.br) — the editorial imprint of Felipe Heemann (Heemann, F.), neurobiologist and neuroscience educator based in Ribeirão Preto, SP, Brazil.

---

## What this is

Brain Codex publishes works that refuse the fragmentation of knowledge. The catalog integrates molecular neurobiology, philosophy of consciousness, history of science, and medical epistemology across eight titles in Portuguese and English — from the 826-page *Psychotropicā Neuroscience* to the philosophical essay *Erectus*.

This repository contains the production source for the institutional website: pure HTML and CSS, no framework, no build step, no dependencies. The site deploys directly to GitHub Pages.

## Catalog

| Title | Lang | Pages | ISBN |
|---|---|---|---|
| Biologia Psicotrópica | PT | 346 | 978-65-988126-0-7 |
| Erectus *(PT)* | PT | 104 | 978-65-988126-5-2 |
| História e Filosofia da Biologia | PT | 165 | 978-65-988126-1-4 |
| History and Philosophy of Biology | EN | 170 | 978-65-988126-3-8 |
| Neuropsicofarmacologia Molecular | PT | 492 | 978-65-988126-2-1 |
| Psychotropicā Neuroscience | EN | 826 | 978-65-988126-4-5 |
| Erectus *(EN)* | EN | 100 | 978-65-988126-6-9 |
| The Fractal Brain | EN | 206 | 978-65-988126-7-6 |

All titles carry ISBNs registered with the Brazilian Book Chamber (CBL). International distribution via IngramSpark; Brazilian distribution via Bok2.

## Structure

```
.
├── index.html              # Main page — catalog, featured work, ISBN registry
├── incisions.html          # Incisions — opinion, critique, annotation
├── foundation.html         # Memorabilia — Foundation
├── annotated_canon.html    # Memorabilia — Annotated Canon
├── epistemic_bedrock.html  # Memorabilia — Epistemic Bedrock
├── pessoa.html             # Memorabilia — Pessoa
├── assentamento.html       # Memorabilia — Assentamento
├── sitemap.xml             # XML sitemap for search engines
├── robots.txt              # Crawler directives
├── _headers                # HTTP header configuration
├── _redirects              # Redirect rules
└── [assets]                # Cover images, favicons
```

No JavaScript frameworks. No package managers. No transpilation. The CSS lives inside each HTML file. Images are inlined as base64 where appropriate for single-request loading.

## SEO

The site ships with structured data (JSON-LD) for the publisher entity, individual book records with `offers` and `bookFormat`, an `ItemList` of the full catalog, Open Graph and Twitter Card metadata on every page, canonical URLs, and an XML sitemap. The structured data follows Schema.org `Book` and `Organization` types.

## Deployment

Push to the `main` branch. GitHub Pages serves the root directory. Custom domain configured via CNAME record pointing to GitHub's servers; HTTPS provisioned automatically.

## Contact

**editorial@ciencias.bio.br**

Brain Codex · CNPJ 61.939.651/0001-36

---

*To decipher the brain is to decipher being.*
