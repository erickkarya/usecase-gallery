# Galeri Use Case IDTC

Galeri karya anggota Indonesia Digital Twin Community — use case, prototipe, dashboard, dan
model Digital Twin yang sudah dibuat dan dibagikan anggota.

**🖼️ Lihat galerinya: [idtc-id.github.io/usecase-gallery](https://idtc-id.github.io/usecase-gallery/)**

## Cara membagikan karya Anda

**Tidak perlu tahu Git atau menulis JSON.** Isi formulir:

1. Buka tab **Issues** → **New issue** → pilih **🏆 Tambah karya ke Galeri Use Case**.
2. Isi formulirnya. Gambar (thumbnail dan tangkapan layar) cukup diseret ke kotak isian —
   GitHub mengunggahnya otomatis.
3. Klik **Create**.
4. Sistem otomatis membuatkan Pull Request berisi karya Anda (satu berkas
   `data/UC-XXXX.json`) dalam beberapa detik.
5. Pengurus menelaah dan menggabungkannya — karya Anda tampil di galeri begitu Pull Request
   itu digabung. Setelah itu sistem membuat satu Pull Request terpisah berlabel
   `chore: perbarui indeks galeri` untuk menyinkronkan daftar; gabungkan juga PR itu.

## Cara memperbarui atau menghapus karya

Setiap karya adalah satu berkas `data/UC-XXXX.json`. Perbarui lewat cara yang sama seperti
mengubah dokumen di repo IDTC lain (lihat modul
[M6 di `panduan-github`](https://github.com/idtc-id/panduan-github/blob/main/modul/M6-mengubah-dokumen-lewat-browser.md)):
buka berkasnya → ikon pensil ✏️ → ubah → **Commit changes...** → **Propose changes** →
**Create pull request**.

> Catatan: daftar di bawah dan `data/index.json` dibangun ulang otomatis dari isi folder
> `data/` yang sebenarnya setiap kali ada perubahan berkas karya di `main` — lewat Pull
> Request terpisah berlabel `chore: perbarui indeks galeri`.

## Apa saja yang diisi

Lihat [`docs/skema.md`](docs/skema.md) untuk penjelasan tiap kolom. Ringkasnya: nama karya,
nama kontributor, instansi (opsional), teknologi yang dipakai, masalah yang diselesaikan
dengan Digital Twin, deskripsi, thumbnail,
tangkapan layar (opsional, boleh beberapa), link aplikasi, link video, dan kontak (opsional).

## Daftar karya

<!-- GALERI:START -->
| ID | Karya | Kontributor | Instansi | Teknologi |
|---|---|---|---|---|
| UC-0005 | [Peta 3D DKI Jakarta](data/UC-0005.json) | Fadhli Akbar dan Muhammad Raihan Tifaldi (@raihantifaldi-jkt) | Dinas Cipta Karya, Tata Ruang dan Pertanahan Provinsi DKI Jakarta | ArcGIS, Cesium, CityGML |
| UC-0008 | [Tata Ruang DKI Jakarta – 3D Viewer](data/UC-0008.json) | Khairul Amri (@geoholix) | Dinas Cipta Karya, Tata Ruang dan Pertanahan Provinsi DKI Jakarta | ArcGIS |
| UC-0009 | [Bhumi 3D Kadaster – ATR/BPN](data/UC-0009.json) | Khairul Amri (@geoholix) | Kementerian ATR/BPN | Cesium |
| UC-0010 | [Volcano3D – Kembar Digital Gunung Berapi (GeoTwinverse)](data/UC-0010.json) | Khairul Amri (@geoholix) | GeoTwinverse | Cesium, React |
| UC-0011 | [Digital Naga](data/UC-0011.json) | Khairul Amri (@geoholix) | ParaKloud | Cesium |
| UC-0012 | [Riset Digital Twin Kampus – Fakultas Teknik UGM](data/UC-0012.json) | Khairul Amri (@geoholix) | Geo AI Twinverse |  |
| UC-0013 | [Blender BIM / Remesh – Outer Shell of a Complete House](data/UC-0013.json) | Khairul Amri (@geoholix) | — | Blender |
| UC-0014 | [Kementerian PU – SMART BIM](data/UC-0014.json) | Khairul Amri (@geoholix) | Kementerian Pekerjaan Umum | BIM, Leaflet |
| UC-0015 | [Kementerian PU – PU Connect](data/UC-0015.json) | Khairul Amri (@geoholix) | Kementerian Pekerjaan Umum | Cesium, BIM |
| UC-0016 | [ARCA – Test Case Digital Twin Area Kementerian PU](data/UC-0016.json) | Khairul Amri (@geoholix) | Paperclip.id | MapLibre, deck.gl, Cesium |
| UC-0017 | [Gaea Engine – Digital Twin Prototype](data/UC-0017.json) | Khairul Amri (@geoholix) | LangitBumi | Three.js |
| UC-0018 | [LangitBumi – Jakarta Digital Twin / Flood Demo](data/UC-0018.json) | Khairul Amri (@geoholix) | LangitBumi | GAEA Engine |
| UC-0019 | [Tata Ruang Jakarta – Spatial / 3D Prototype](data/UC-0019.json) | Khairul Amri (@geoholix) | Dinas Cipta Karya, Tata Ruang dan Pertanahan Provinsi DKI Jakarta | ArcGIS |
| UC-0020 | [Drone Docking – Pilot Digital Twin Aware](data/UC-0020.json) | Khairul Amri (@geoholix) | — |  |
| UC-0021 | [Leica CityMapper – Model Kota 3D Denver](data/UC-0021.json) | Khairul Amri (@geoholix) | Leica Geosystems | Leica CityMapper |
<!-- GALERI:END -->

## Lisensi

Hak cipta tiap karya tetap pada kontributornya masing-masing. Metadata di repo ini
(berkas `data/*.json`) dibagikan dengan lisensi [CC BY 4.0](LICENSE.md) agar bisa dipakai
ulang untuk keperluan komunitas.
