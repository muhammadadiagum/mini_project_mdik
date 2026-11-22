# Dashboard Bahaya Gempa dan Tsunami Indonesia 2010–2024

## Struktur repo

```
index.html                         dashboard satu halaman
assets/                            Plotly, Leaflet, CSS lokal
data/
├── README.md                      atribusi dan daftar berkas data
├── dashboard_data_usgs_noaa.json  sumber data runtime dashboard
├── raw/                           bukti data mentah + manifest
└── processed/                     CSV bersih + kamus data
```

## GitHub Pages

- Source: **Deploy from a branch**
- Branch: `main`
- Folder: **`/` (root)**
- URL: `https://<username>.github.io/<repo>/`

Semua berkas di repo ini tersaji publik, termasuk `data/raw/` dan `data/processed/`. Itu disengaja sebagai bukti dataset dan aman karena bersumber dari USGS/NOAA public domain serta tidak memuat identitas pribadi korban.

Sumber data: USGS ComCat + NOAA/NCEI G02151, diakses 22 November 2026. Atribusi peta: © OpenStreetMap contributors.
