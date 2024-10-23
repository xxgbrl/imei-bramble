# imei-bramble

tutorial rewrite imei google pixel (4a 5g) mandiri

syarat dan bahan:
1. hp google pixel (android 15 blm nyoba, mungkin cara nya sama)
2. kabel usb type c
3. pc/laptop
4. file bahan (https://unesa.me/o0qo7n)
5. install semua driver
6. file .qcn sesuai tipe hp (https://unesa.me/a8t7zg)
7. rasa sabar

untuk bugjaeger (ubl + pasang root)
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
7. masuk folder platform-tools
8. ketik fastboot devices atau adb device
9. pastikan device terdeteksi
10. ketik adb reboot bootloader
11. ketik fastboot flashing unlock

cara root
1. factory reset/reset pabrik
2. download rom google pixel sesuai tipe hp (https://unesa.me/hdf65u) 
3. ekstrak file tersebut
4. ekstrak lagi file image-blablabla.zip
5. cari file boot.img
6. install magisk di hp
7. klik install (yg atas)
8. pilih select and patch a file
9. cari file boot.img tadi
10. klik let's go
11. tunggu sampai selesai
12. hasil berada di folder download (nama file magisk-blablabla.zip)
13. pindah file ke pc/laptop di folder platform-tools

pasang root
1. sambungkan hp ke pc/laptop
2. masuk mode fastboot (matikan hp terus tahan power + volume down)
3. masuk folder platform-tools
4. buka cmd/power shell (tahan shift + klik kanan) atau pake bugjaeger
5. ketik fastboot devices atau adb device
6. pastikan device terdeteksi
7. ketik adb reboot bootloader
8. ketik fastboot flash boot *namaboot.img (*hasil step cara root)
9. tunggu sampai selesai
10. reboot

edit imei
1. matikan windows defender
2. buka aplikasi qcn tool
3. pilih file .qcn yg udah di download
4. isi kolom 3 dan 4 dengan imei (boleh imei hp lama atau bisa generate online di https://unesa.me/tbf5u6) 
5. export ke folder yg gampang di inget (atau di folder platform-tools)

rewrite imei1
1. hp mode pesawat
2. nyalakan dsds untuk imei2 (*#*#4636#*#*)
3. cek di *#06#, pastikan imei2 muncul
4. nyalakan usb debugging
5. sambungkan hp ke pc/laptop
6. masuk folder platform-tools
7. buka cmd/power shell (tahan shift + klik kanan) atau pake bugjaeger
8. ketik fastboot devices atau adb device
9. masuk mode diag (ada di bahan)
10. cek di device manager, wajib muncul nama usb Qualcomm-HS-USB
11. ke notif hp, ganti pilihan usb jadi transfer file
12. buka qlm write imei tool
13. pilih port usb
14. klik setting
15. password ustest
16. centang imei1 dan imei2
17. balik ke qlm write imei tool
18. isi imei1 dan imei2 sama kayak yg di qcn tool
19. klik write
20. tunggu sampai selesai
21. reboot
22. cek *#06#, pastikan imei1 muncul normal (tidak 0044)

rewrite imei2
1. hp mode pesawat
2. nyalakan dsds untuk imei2 (*#*#4636#*#*)
3. cek di *#06#, pastikan imei2 muncul
4. nyalakan usb debugging
5. sambungkan hp ke pc/laptop
6. masuk folder platform-tools
7. buka cmd/power shell (tahan shift + klik kanan)
8. ketik fastboot devices atau adb device
9. masuk mode diag (ada di bahan)
10. ke notif hp, ganti pilihan usb jadi transfer file
11. cek di device manager, wajib muncul nama usb Qualcomm-HS-USB
12. buka qpst configuration
13. pilih start client
14. software download
15. restore qcn hasil edit imei
16. klik start
17. tunggu selesai
18. reboot
19. cek *#06#, pastikan imei2 muncul normal (tidak 0044)

note:
1. yg file .qcn ga ada bisa cari sendiri di google atau youtube, keyword (tipe hp) file qcn
2. data pasti hilang jadi backup/pindah dulu semua data di hp sebelum di unlock
4. jika bingung bisa sambil buka link youtube di bawah

link youtube:
1. root https://youtu.be/EKuGPRJzzio
2. rewrite imei1 https://youtu.be/BOOebgB4d58
3. rewrite imei2 https://youtu.be/AkfH_-usbVM

maaf kalo tutorial kurang jelas atau berantakan, semoga membantu
