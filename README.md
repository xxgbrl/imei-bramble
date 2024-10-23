# imei-bramble

syarat dan bahan:
1. hp google pixel up to 4xl (android 15 blm nyoba, mungkin cara nya sama)
2. kabel usb type c
3. pc/laptop
4. file bahan (https://drive.google.com/drive/folders/1E5HruLM2cAV7YXqM41zIazjluLjaabhX)
5. install semua driver
6. file .qcn sesuai tipe hp (https://www.ahmadservicecenter.com/2023/11/koleksi-file-qcn-google-pixel-fix.html?m=1)
7. rasa sabar

untuk bugjaeger
1. hp lain
2. kabel usb type c
3. otg


cara ubl
1. nyalakan developer options (ketuk 7 kali build number)
2. nyalakan oem unlocking
3. nyalakan usb debugging
4. masuk mode fastboot (matikan hp terus tahan power + volume down)
5. sambungkan hp ke pc/laptop
6. buka cmd, run as administrator atau bisa pake bugjaeger
7. ketik _fastboot devices_ atau _adb device_
8. pastikan device terdeteksi
9. ketik _adb reboot bootloader_
10. ketik _fastboot flashing unlock_

cara root
1. download rom google pixel sesuai tipe hp
2. ekstrak file tersebut
3. ekstrak lagi file image-blablabla.zip
4. cari file boot.img
5. install magisk di hp
6. klik install (yg atas)
7. pilih select and patch a file
8. cari file boot.img tadi
9. klik let's go
10. tunggu sampai selesai

install root
1. sambungkan hp ke pc/laptop
2. masuk mode fastboot (matikan hp terus tahan power + volume down)
3. ketik _fastboot devices_ atau _adb device_ di cmd atau bugjaeger
4. pastikan device terdeteksi
5. buka cmd, run as administrator
6. ketik _adb reboot bootloader_
7. ketik _fastboot flash boot namaboot.img_
8. tunggu sampai selesai
9. reboot

cara rewrite imei
1. buka aplikasi qcn tool
2. isi kolom 3 dan 4 dengan imei
3. export ke folder yg gampang di inget

masuk mode diag (ada di bahan)
1. buka qlm write imei tool
2. pilih port usb
3. klik setting
4. password _ustest_
5. centang imei1 dan imei2
6. balik ke qlm write imei tool
7. isi imei1 dan imei2 sama kayak yg di qcn tool
8. klik write
9. tunggu sampai selesai
10. reboot

masuk mode diag (ada di bahan)
1. buka qpst configuration
2. pilih start client
3. software download
4. restore qcn hasil qcn tool
5. klik start
6. tunggu selesai
7. reboot

note:
1. yg file .qcn ga ada bisa cari sendiri di google atau youtube, keyword _(tipe hp) file qcn_
2. data pasti hilang jadi backup/pindah dulu semua data di hp sebelum di unlock 
