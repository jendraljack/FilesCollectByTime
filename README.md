# BackupFilesCollectByTime<br/>
Collect files by date<br/>
Jika kamu punya beberapa berkas tertentu tapi berserakan dalam folder di mana-mana.<br/><br/>
skrip shell ini membantu mengumpulkan ke dalam folder sesuai tahun-bulan-tanggal nya.<br/>
misalnya: ada berkas.apk<br/> berkas.apk, pasti semua berkas mempunyai tanda waktu saat dibuat.
<pre>android:~ # ls -l berkas.apk
-rw-rw- root root 4096 2024-05-11 17:30 berkas.apk
android:~ #</pre>
dari 2024-05-11 skrip akan membuatkan folder /2024/05/11 rekursive.<br/>
nanti jika belum ada berkas.apk di
/sdcard/backup/2024/05/11/berkas.apk
<br/>skrip akan membuat folder backup/2024/05/11, lalu memindahkan berkas.apk ke dalamnya.<br/><br/>
perintah skripnya.
simpan skrip di root sdcard.
<pre>android:~ # sh CollectFilesByTime.sh apk</pre><br/>
apk hanya salah satu format yang didukung.<br/>
kamu bisa memindah kan semua format yang kamu mau(zip/mp3/mp4), dengan syarat nama folder dan berkas tidak mengandung karakter spasi. <br/>
update - backup berkas berdasarkan md5.
<pre>sh BackupFilesMd5.sh format(mp4/mp3/mendukung semua tipe format)</pre>

