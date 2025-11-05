# Estrategia de indexación TCDS

## Objetivo
Maximizar descubribilidad en Google, Bing, y crawlers de IA, preservando trazabilidad Σ-metrics.

## Pasos
1. **Schema unificado**: publique `TCDS_schema_extended.jsonld` en `/schema.jsonld` y enlácelo en `<head>`.
2. **RDF paralelo**: publique `TCDS_schema.ttl` y enlace desde `schema.jsonld` (`distribution`).
3. **Sitemaps**: sirva `sitemap.xml` y declare en `robots.txt`.
4. **Páginas canónicas**: defina `<link rel="canonical">` en `index.html`, `documents.html`, `dataset.html`.
5. **Datos descargables**: mantenga URLs estables para `.jsonld` y `.ttl`; evite parámetros.
6. **PDFs**: añada `<meta name="citation_title">` y `schema:CreativeWork` por PDF con enlaces internos.
7. **Zenodo/DOI**: añada `sameAs` con `https://doi.org/10.5281/zenodo.17505875`.
8. **OpenGraph/Twitter**: agregue `og:title`, `og:description`, `og:url`, `og:type=website`.
9. **Performance**: PageSpeed > 90. Sirva estáticos con `Cache-Control: public, max-age=604800`.
10. **Accesibilidad**: `lang="es"`, etiquetas ARIA, contraste AA.

## Colocación
- `index.html`: inyecte `<script type="application/ld+json" src="schema.jsonld"></script>`.
- `documents.html` y `dataset.html`: repita `WebSite`, `CollectionPage` y `Dataset` con `@id` idénticos.

## Plantillas
**robots.txt**
```
User-agent: *
Allow: /
Sitemap: https://geozunac3536-jpg.github.io/TCDS-PORTAL/sitemap.xml
# Crawl-delay not standard; omit for Google. Keep fast serving and caching.

```

**sitemap.xml**
```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url><loc>https://geozunac3536-jpg.github.io/TCDS-PORTAL/</loc></url>
  <url><loc>https://geozunac3536-jpg.github.io/TCDS-PORTAL/documents.html</loc></url>
  <url><loc>https://geozunac3536-jpg.github.io/TCDS-PORTAL/dataset.html</loc></url>
  <url><loc>https://geozunac3536-jpg.github.io/TCDS-PORTAL/schema.jsonld</loc></url>
  <url><loc>https://geozunac3536-jpg.github.io/TCDS-PORTAL/TCDS_schema.ttl</loc></url>
</urlset>

```

**HTML `<head>` mínimo**
```html
<link rel="canonical" href="https://geozunac3536-jpg.github.io/TCDS-PORTAL/">
<script type="application/ld+json" src="https://geozunac3536-jpg.github.io/TCDS-PORTAL/schema.jsonld"></script>
<meta property="og:title" content="TCDS — Portal de Documentos">
<meta property="og:url" content="https://geozunac3536-jpg.github.io/TCDS-PORTAL/">
<meta name="twitter:card" content="summary_large_image">
```
