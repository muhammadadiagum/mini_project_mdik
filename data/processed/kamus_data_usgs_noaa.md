# Kamus Data — Desain v2 USGS + NOAA

## gempa_usgs_2010_2024.csv
| Kolom | Arti | Satuan |
|---|---|---|
| id | Identifier unik ComCat USGS | - |
| waktu | Waktu kejadian UTC | timestamp |
| tahun | Tahun kejadian | tahun |
| latitude, longitude | Episenter gempa (koordinat asli USGS) | derajat |
| magnitudo | Magnitudo gempa | Mw/ML sesuai tipe |
| tipe_magnitudo | Skala magnitudo yang dipakai USGS | - |
| kedalaman_km | Kedalaman episenter | km |
| kategori_kedalaman | dangkal <70, menengah 70–300, dalam >300 | kategori |
| lokasi_teks | Deskripsi lokasi dari USGS | teks |
| flag_tsunami | Flag tsunami dari USGS (0/1) | - |
| url | Laman detail kejadian USGS (dibentuk dari ID jika CSV tidak menyertakannya) | URL |
| error_horizontal_km | Ketidakpastian horizontal episenter | km |
| error_kedalaman_km | Ketidakpastian kedalaman | km |
| error_magnitudo | Ketidakpastian magnitudo | satuan mag |
| sumber_magnitudo | Lembaga/metode penentu magnitudo | - |

## tsunami_noaa_event_2010_2024.csv
| Kolom | Arti | Satuan |
|---|---|---|
| id | ID event tsunami NOAA | - |
| tanggal, tahun | Tanggal sumber tsunami | tanggal/tahun |
| latitude, longitude | Koordinat sumber tsunami (asli NOAA) | derajat |
| lokasi | Nama lokasi sumber | teks |
| penyebab | Terjemahan kode penyebab NOAA | kategori |
| magnitudo_gempa | Magnitudo gempa pemicu jika ada | Mw |
| kedalaman_gempa_km | Kedalaman gempa pemicu | km |
| tinggi_gelombang_maks_m | Tinggi gelombang maksimum | m |
| jumlah_runup | Jumlah titik runup terkait | titik |
| meninggal | Korban meninggal (deathsTotal, fallback deaths) | jiwa |
| luka_total | Korban luka | jiwa |
| rumah_hancur_total, rumah_rusak_total | Kerusakan rumah | unit |

## tsunami_noaa_runup_idn_2010_2024.csv
| Kolom | Arti | Satuan |
|---|---|---|
| id | ID titik runup NOAA | - |
| id_event_tsunami | Event tsunami induk | - |
| latitude, longitude | Titik observasi runup (asli NOAA) | derajat |
| lokasi, area | Nama titik dan area observasi | teks |
| tinggi_runup_m | Tinggi runup tercatat | m |
| jarak_sumber_km | Jarak dari sumber | km |
| waktu_tempuh_jam | Waktu tempuh gelombang | jam |
| tipe_pengukuran | Kode metode NOAA | - |
| diragukan | Flag keraguan NOAA (y/n) | - |

Catatan penting: koordinat pada ketiga berkas adalah koordinat kejadian/observasi, bukan centroid administratif.
