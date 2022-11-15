##Business Problem Understanding
###Latar Belakang
Perusahaan asuransi travel ingin menerapkan sistem seleksi cerdas berbasis machine learning. Sistem seleksi cerdas tersebut akan menilai apakah customer  mendapatkan klaim asuransi atau tidak dengan melihat profil yang diekstrak dari data-data perjalanan customer.  

Target :
*   0 -> Customer yang tidak mendapatkan klaim asuransi
*   1 -> Customer yang mendapatkan klaim asuransi

###Problem Statement :
Sebenarnya perusahaan sudah membuat suatu model untuk menerapkan sistem seleksi cerdas yang akurasinya sangat tinggi untuk menyeleksi customer yang tidak untuk mendapatkan klaim asuransi, namun model menjadi sangat tidak akurat untuk menyeleksi customer yang mendapatkan asuransi. Sehingga banyak customer yang seharusnya mendapatkan klaim asuransi merasa dirugikan dan tidak puas. 

###Goals :
Dari permasalahan tersebut perusahaan ingin agar model yang digunakan untuk seleksi otomatis dievaluasi dan diperbaiki sehingga bisa menyeleksi customer yang mendapatkan klaim asuransi. Diharapkan dengan evaluasi dan perbaikan model ini jumlah customer yang merasa dirugikan dan tidak puas menjadi berkurang.

###Metric Evaluation


*   Type 1 Error : False Positive
Konsekuensi : Customer yang seharusnya tidak mendapatkan klaim asuransi bisa mendapatkan klaim asuransi sehingga klaim asuransi yang tidak tepat sasaran bisa bertambah banyak jumlahnya 
*   Type 2 Error : False Negative
Konsekuensi : Customer yang seharusnya mendapatkan klaim asuransi tidak mendapatkan klaim asuransi sehingga customer merasa dirugikan. Hal ini bisa membuat jelek reputasi perusahaan asuransi dan berpotensi membuat customer tidak mau untuk mengikuti asuransi lagi.


Dari konsekuensinya dapat dilihat bahwa model diharapkan dapat memprediksi customer yang mendapatkan klaim dengan baik sehingga customer puas dan reputasi perusahaan asuransi terjaga dengan baik. Dengan sesedikit mungkin kesalahan untuk prediksi customer yang tidak mendapatkan klaim asuransi sehingga mengurangi biaya klaim yang tidak tepat sasaran. Perusahaan menginginkan untuk meminimalkan False Negative pada model sistem deteksi yang dibuat. Sehingga metric yang digunakan untuk kasus ini adalah recall karena berfokus pada satu kelas saja yaitu kelas customer yang mendapatkan klaim asuransi
