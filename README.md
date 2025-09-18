#### **1. Jejak Eksekusi Program (UserAssist)**
Tujuannya adalah meninggalkan jejak bahwa Budi telah menjalankan program mencurigakan. Kunci registri ini menyimpan data eksekusi program dalam format ROT13 (enkripsi sederhana).

* **Aksi:**
    1.  Buat file kosong di Desktop. Beri nama `DataRahasia.txt`.
    2.  Buat program palsu. Buka Notepad, ketik apa saja, lalu simpan dengan nama `KirimData.exe` di Desktop.
    3.  **Klik dua kali dan jalankan `KirimData.exe`** beberapa kali.
* **Lokasi Artefak:** `NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Explorer\UserAssist\{GUID}\Count`

#### **2. Jejak URL yang Diketik (TypedURLs)**
Tujuannya adalah menunjukkan Budi mengunjungi situs web untuk mentransfer file.

* **Aksi:**
    1.  Buka browser **Internet Explorer** atau **Microsoft Edge (mode IE)**. (Browser lama lebih andal untuk artefak ini).
    2.  Di address bar, **ketik manual** URL berikut dan tekan Enter: `http://transfer-file-rahasia.com/upload`
* **Lokasi Artefak:** `NTUSER.DAT\Software\Microsoft\Internet Explorer\TypedURLs`

#### **3. Jejak File yang Dibuka (RecentDocs)**
Ini adalah bukti paling umum. Kita akan meninggalkan jejak file dokumen sensitif yang telah dibuka Budi.

* **Aksi:**
    1.  Buat sebuah file di folder `Documents`.
    2.  Beri nama file yang spesifik, misalnya **`Rencana_Akuisisi_Q4_2025.docx`**.
    3.  **Buka file tersebut** dengan Wordpad atau Microsoft Word. Tutup kembali.
* **Lokasi Artefak:** `NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Explorer\RecentDocs`

#### **4. Jejak Pencarian File (WordWheelQuery)**
Kita akan membuat seolah-olah Budi secara aktif mencari file rahasia tersebut.

* **Aksi:**
    1.  Buka File Explorer.
    2.  Gunakan kotak pencarian di pojok kanan atas.
    3.  Ketik kata kunci pencarian: **"Akuisisi"**. Tunggu hingga pencarian selesai.
* **Lokasi Artefak:** `NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Explorer\WordWheelQuery`

---
