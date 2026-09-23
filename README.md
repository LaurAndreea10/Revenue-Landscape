# Revenue Landscape

Dashboard 3D bilingv și accesibil pentru explorarea veniturilor, comparații YoY, forecast și simulări *What-if*.

[![Live Demo](https://img.shields.io/badge/Live_Demo-2ee6c8?style=for-the-badge&logo=github&logoColor=080b17)](https://laurandreea10.github.io/Revenue-Landscape/)
[![Case Study](https://img.shields.io/badge/Case_Study-8b6bff?style=for-the-badge&logo=readme&logoColor=white)](https://laurandreea10.github.io/Revenue-Landscape/case-study.html)
[![PWA](https://img.shields.io/badge/PWA-ready-ff5c9a?style=for-the-badge)](https://laurandreea10.github.io/Revenue-Landscape/manifest.webmanifest)

![Revenue Landscape preview](social-preview.svg)

**[Deschide aplicația](https://laurandreea10.github.io/Revenue-Landscape/)** · **[Citește studiul de caz](https://laurandreea10.github.io/Revenue-Landscape/case-study.html)** · **[Vezi changelog-ul](CHANGELOG.md)**

## Problemă → Decizie → Rezultat

- **Problemă:** un bar chart clasic arată valorile, dar nu susține explorarea, scenariile sau interpretarea rapidă.
- **Decizie:** Canvas 2D cu proiecție 3D, completat de tabel semantic, KPI, forecast și import/export local.
- **Rezultat:** un Analytics Lab fără framework, instalabil, offline și adaptat pentru desktop și mobil.

## Funcții

- grafic 3D cu mouse, touch și tastatură;
- Revenue/Growth, 2025/2026 și target;
- scenarii realist, optimist, pesimist și What-if;
- forecast, insight-uri, progres și tabel accesibil;
- import/export CSV și JSON, export PNG;
- autosave local, Undo și reset;
- RO/EN, dark/light, high contrast și reduced motion;
- PWA offline, SEO și date structurate.

## Rulare

Pornește un server static în directorul proiectului. Service worker-ul nu funcționează prin `file://`.

```bash
python3 -m http.server 8080
```

Deschide `http://localhost:8080`.

## Testare recomandată

1. Editează o valoare și reîncarcă pagina pentru autosave.
2. Importă un CSV cu antetul `month,2025,2026` și 12 rânduri.
3. Verifică modurile Revenue/Growth și scenariile.
4. Navighează graficul cu săgețile.
5. Testează la 320 px și 200% zoom.
6. Rulează Lighthouse pe mobil.

## Arhitectură

- `index.html` — interfață, stiluri și motor Canvas;
- `sw.js` — cache offline;
- `manifest.webmanifest` — instalare PWA;
- `case-study.html` — studiu de caz bilingv;
- `robots.txt` și `sitemap.xml` — indexare;
- `404.html` și `offline.html` — stări de eroare;
- `icon.svg` și `social-preview.svg` — identitate vizuală.

## Confidențialitate

Datele importate rămân în browser. Aplicația nu trimite seturile de date către un server.

## Autor

Laura Andreea Plugaru — front-end self-taught, CRM & Marketing.

[Portofoliu](https://laurandreea10.github.io/codepen-portfolio/) · [GitHub](https://github.com/LaurAndreea10)

---

## English

Revenue Landscape is an accessible bilingual 3D analytics dashboard for revenue exploration, YoY comparison, forecasting and What-if scenarios. It is framework-free, local-first, responsive and installable as a PWA.
