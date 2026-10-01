# Skema Galeri Use Case

Setiap karya di galeri adalah satu berkas `data/UC-XXXX.json`, dibuat otomatis dari isian
formulir Issue. Nomor `UC-XXXX` diambil dari nomor issue, jadi tidak pernah bentrok.

| Atribut | Tipe | Keterangan | Wajib diisi? |
|---|---|---|---|
| **ID Use Case** | Otomatis | `UC-0001`, `UC-0002`, ... — dari nomor issue, bukan diisi manual | — |
| **Nama Use Case / Model Digital Twin** | Teks | Judul karya, tampil sebagai judul kartu | Ya |
| **Nama Kontributor** | Teks | Nama anggota IDTC yang membuat/membagikan karya | Ya |
| **Instansi / Organisasi** | Teks | Dipakai juga sebagai filter di galeri | Tidak |
| **Teknologi yang Digunakan** | Teks, pisah koma | Disimpan sebagai daftar; jadi chip warna sekaligus filter | Ya |
| **Deskripsi Use Case** | Teks panjang | Masalah yang diselesaikan, pendekatan, manfaat | Ya |
| **Thumbnail** | Gambar | Satu gambar sampul kartu, rasio 16:9 disarankan | Ya |
| **Tangkapan Layar Aplikasi** | Gambar | Boleh beberapa; tampil sebagai galeri di halaman detail | Tidak |
| **Link Aplikasi** | URL | Tautan aplikasi/dashboard/demo | Tidak |
| **Link Video** | URL | YouTube & Vimeo otomatis bisa diputar langsung di halaman | Tidak |
| **Kontak** | Teks | Surel atau tautan; surel otomatis jadi tautan `mailto:` | Tidak |
| **Kontributor (username GitHub)** | Otomatis | Diambil dari akun yang membuka issue; dipakai untuk foto profil | — |

## Cara gambar diunggah

Tidak ada server penyimpanan gambar terpisah. Kotak **Thumbnail** dan **Tangkapan Layar**
memanfaatkan kemampuan bawaan GitHub: gambar yang diseret/ditempel ke kotak isian diunggah
GitHub ke CDN-nya sendiri, lalu disisipkan sebagai markdown `![nama](url)`. Workflow
mengambil url dari markdown itu — satu url untuk thumbnail, semua url untuk tangkapan layar.

## Video yang bisa diputar langsung

Halaman galeri mengenali tautan YouTube (`youtube.com/watch`, `youtu.be`, `/shorts/`,
`/live/`) dan Vimeo, lalu menanamkannya sebagai pemutar video di halaman detail. Tautan dari
layanan lain tetap disimpan dan ditampilkan sebagai tombol **Tonton video** biasa.

## Format penyimpanan

```json
{
  "idUsecase": "UC-0001",
  "namaUsecase": "Digital Twin Pemantauan Banjir DAS Ciliwung",
  "kontributor": "Budi Santoso",
  "instansi": "Universitas Indonesia",
  "teknologi": ["ArcGIS", "Python", "PostGIS"],
  "deskripsi": "Model kembaran digital untuk memantau tinggi muka air...",
  "kontak": "budi@contoh.ac.id",
  "thumbnailUrl": "https://github.com/user-attachments/assets/...",
  "tangkapanLayar": [
    "https://github.com/user-attachments/assets/...",
    "https://github.com/user-attachments/assets/..."
  ],
  "linkAplikasi": "https://contoh.id/dashboard",
  "linkVideo": "https://youtube.com/watch?v=xxxxxxxxxxx",
  "kontributorUsernameGithub": "contoh-username",
  "dibuatPada": "2026-10-01T10:00:00Z",
  "issue": "https://github.com/idtc-id/usecase-gallery/issues/1"
}
```

`data/index.json` adalah kumpulan seluruh karya dalam satu berkas — dibangun ulang otomatis
setiap ada perubahan, supaya halaman galeri cukup sekali ambil tanpa memanggil API GitHub
berkali-kali.
