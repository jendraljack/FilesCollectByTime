# FilesCollectByTime
Collect files by date
kamu punya beberapa berkas tertentu tapi berserakan dalam folder di mana-mana.
skrip shell ini membantu mengumpulkan ke dalam folder sesuai tahun-bulan-tanggal nya.
misalnya: ada berkas berkas.apk
pasti semua berkas mempunyai tanda waktu waktu dibuat.
<pre>android:~ # ls -l berkas.apk
-rw-rw- root root 4096 2024-05-11 berkas.apk
android:~ #</pre>
dari 2024-05-11 saya akan buatkan foldernya.
nanti jika bukan/belum ada berkas.apk di
/sdcard/backup/2024/05/11/berkas.apk
skrip akan membuat folder backup/2024/05/11, lalu memindahkan berkas.apk ke dalamnya.


