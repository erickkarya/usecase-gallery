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
nama kontributor, instansi (opsional), teknologi yang dipakai, deskripsi, thumbnail,
tangkapan layar (opsional, boleh beberapa), link aplikasi, link video, dan kontak (opsional).

## Daftar karya

<!-- GALERI:START -->
| ID | Karya | Kontributor | Instansi | Teknologi |
|---|---|---|---|---|

<!-- GALERI:END -->

## Lisensi

Hak cipta tiap karya tetap pada kontributornya masing-masing. Metadata di repo ini
(berkas `data/*.json`) dibagikan dengan lisensi [CC BY 4.0](LICENSE.md) agar bisa dipakai
ulang untuk keperluan komunitas.
