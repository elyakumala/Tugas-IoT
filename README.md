PENJELASAN PROGRAM:

Motion Sensor dihubungkan SBC dengan pin 0(D0), Garage dihubungkan SBC dengan pin 1(D1), dan Light Garage digubungkan SBC dengan pin 2(D2). GPIO (General Purpose Input/Output) merupakan library yang digunakan untuk mengontrol GPIO Raspberry Pi menggunakan Python. GPIO merupakan pin atau tempat yang digunakan sebagai input dan output Fungsi pinMode berguna untuk mengkonfigurasikan nomor pin yang dipakai. Motion_sensor merupakan permisalan yang digunakan untuk digitalRead nya yang berarti membaca input pada pin 0(D0). Dengan menggunakan pengkondisian if yang berarti jika motion_sensor dalam keadaan HIGH atau terdeteksi adanya pergerakan maka akan dijalankan fungsi print yaitu ‘Lampu nyala’ dan ‘Garasi Terbuka’, customWrite(1,1) yang berarti menyetel pin 1(D1) yaitu Garage nya dengan kondisi HIGH/terbuka, customWrite(2,1) berarti menyetel pin 2(D2) yaitu Light Garage nya dengan kondisi HIGH/nyala, masing-masing dengan delay 1 detik. Jika if tidak dijalankan maka akan dijalankan else yaitu mengeprint ‘Lampu mati’ dan ‘Garasi Tertutup’, customWrite(1,0) yang berarti menyetel pin 1(D1) yaitu Garage nya dengan kondisi LOW/tertutup, customWrite(2,0) berarti menyetel pin 2(D2) yaitu Light Garage nya dengan kondisi LOW/mati
