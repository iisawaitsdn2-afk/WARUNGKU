# WARUNGKU Rust + WebAssembly

Eksperimen rebuild WARUNGKU dengan Rust, Leptos CSR, dan Trunk.

## Menjalankan di komputer
1. Pasang Rust stable.
2. Jalankan `rustup target add wasm32-unknown-unknown`.
3. Pasang Trunk dengan `cargo install trunk --locked`.
4. Jalankan `trunk serve --open`.

## Build produksi
`trunk build --release --public-url /WARUNGKU/`

## Catatan migrasi
- Versi lama tetap aman di branch `main`; eksperimen ini ada di `rust-rebuild`.
- Data transaksi versi HTML lama belum otomatis dipindahkan ke penyimpanan versi Rust.
- URL Apps Script masih disimpan di pengaturan; format payload perlu disesuaikan dan diuji sebelum integrasi Sheets dipakai.
- Deploy otomatis baru aktif setelah kode ini ditinjau dan digabung ke `main`.
