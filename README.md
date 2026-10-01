# SAMSSZ Mobile V18 — FULL FIXED (Extract + OTD + semua fitur)

Satu project lengkap seperti file awal, dengan **Extract** dan **OTD** yang sudah diperbaiki.

## Fitur
| Menu | Status |
|------|--------|
| Smart Mod Builder | OK |
| Full Vehicle Pipeline | OK |
| Auto Scan ZIP/RPF | OK |
| **Extract RPF / YTD** | **FIXED** — pure Python, recursive |
| **Build RPF** | OK |
| **Build OTD** | **FIXED** — butuh xow64 sekali (lihat `otd_runtime/`) |
| Convert to PC | OK |
| Family Renamer | OK |
| AI / Help | OK |
| File size besar | Streaming I/O + largeHeap |

## Build APK (GitHub)
1. Upload **seluruh isi** ZIP ini ke root repo GitHub.
2. Actions → **Build SAMSSZ Mobile APK** → download `app-debug.apk`.

## Supaya OTD jalan di HP (sekali saja)
Baca: `otd_runtime/PANDUAN_OTD.txt`

Ringkas:
```bash
# di Termux
termux-setup-storage
bash /path/ke/project/otd_runtime/01_install_termux.sh
bash /path/ke/project/otd_runtime/02_hubungkan_ke_folder_mod.sh /path/ke/folder_mod
```
Lalu di app: pilih folder_mod → Build → OTD.

Engine `ragebuilder.exe` sudah ada di `otd_runtime/builder/`.
