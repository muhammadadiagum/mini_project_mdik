# Data publikasi dashboard

Sumber: **USGS ComCat** + **NOAA/NCEI G02151** (public domain). Diakses: 2026-11-22.

## Dipakai saat runtime
`dashboard_data_usgs_noaa.json` diambil oleh `index.html` melalui `fetch()` saat dashboard dibuka.

## Bukti dataset
`raw/` berisi respons API, manifest, URL, parameter, dan checksum SHA-256.
`processed/` berisi CSV bersih dan kamus data.

## Daftar berkas

| Berkas | Ukuran | SHA-256 (singkat) |
|---|---:|---|
| `raw/manifest_usgs_noaa.json` | 3,468 byte | 32ac90675906… |
| `raw/noaa_tsunami_event_idn_2010_2024.json` | 10,483 byte | 048c9e20be7a… |
| `raw/noaa_tsunami_runup_idn_2010_2024.json` | 662,219 byte | 0c13e2feebd4… |
| `raw/usgs_gempa_idn_2010_2024.csv` | 547,205 byte | ef146014a03f… |
| `processed/gempa_usgs_2010_2024.csv` | 570,840 byte | d97d84be4e86… |
| `processed/kamus_data_usgs_noaa.md` | 2,346 byte | e0add070d22b… |
| `processed/tsunami_noaa_event_2010_2024.csv` | 2,212 byte | a716fa0d4c22… |
| `processed/tsunami_noaa_runup_2010_2024.csv` | 128,726 byte | 199df365cb70… |
| `dashboard_data_usgs_noaa.json` | 1,072,014 byte | 66a94d12be07… |

Atribusi peta: © OpenStreetMap contributors. Sumber data tercantum juga di header dan footer dashboard.
