# Build SAMSSZ Mobile APK

## GitHub Actions
1. Extract project ZIP.
2. Push semua file ke root repository (`settings.gradle` harus di root).
3. Actions → Build SAMSSZ Mobile APK → artifact **SAMSSZ-Mobile-debug**.

## Extract & OTD
- **Extract** RPF/YTD: jalan murni di APK (Python embedded), tanpa Termux.
- **OTD**: engine builder sudah di `otd_runtime/builder/`. Launcher Wine (xow64) dipasang sekali via Termux — lihat `otd_runtime/PANDUAN_OTD.txt`.

## Version
4.0-full-extract-otd-fixed
