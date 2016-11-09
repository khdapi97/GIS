**PENAMBAHAN CLASS PADA RETREIVE DATA GEOSPASIAL**

**Latar Belakang**

Informasi Geospasial adalah data geospasial yang sudah diolah sedemikian rupa sehingga dapat digunakan pembuat atau seorang pengembang sebagai alat bantu dalam perumusan kebijakan, kemudian untuk pengambilan keputusan ataupun pelaksanaan kegiatan yang berhubungan dengan keruangan pada bumi ini. Kemudian informasi Geospasial juga dapat membatu seorang yang akan mengembangkan suatu prototipe dari perkembangan bumi ini, dan dapat memudahkanseorang dalam menetukan wilayahnya atau lokasi dimana ia berada.

**Pembahasan atau Isi**

Information Retrieval adalah suatu seni dan ilmu yang mencari informasi dalam suatu dokumen, dan untuk mencari dokumen itu sendiri, mencari metadata yang menjelaskan tentang dokumen, atau mencari dalam sebuah database. Kemudian dalam penjelasan kali ini akan membahas tentang pencarian model tyipe data yang berextension shp dan dbf file. Kemudian dalam pembahasan kali ini akan menjelaskan sedikit tentang polyline dan polygon.

Polyline adalah adalah suatu obyek yang tersusun dari beberapa garis yang lurus dan garis lengkung yang bersambung dan diperlakukan sebagai satu obyek tunggal.

Polygon adalah suatu garis yang digunakan dalam pembuatan peta dan sebagai kerangka yang sangat dasar dalam pemetaan yang akan memiliki sebuah titik-titik, dimana titik tersebut mempunyai sebuah koordinat ataupun sumbu X dan Y.

Berikut contoh dari pencarian data shp dan dbf file menggunakan python :

**Operasi pada Python: **

**Implementasi Retrieve Data Geospasial dalam python:**

&gt;&gt;sf = shapefile.Reader(‘namafile.shp’)

**sf** adalah variable

**shapefile** adalah nama class

**Reader** adalah nama method

**Perintah untuk mengambil data perkolom:**

&gt;&gt;sf.record(n)\[n\]

**Perintah untuk melihat isi shapefile:**

&gt;&gt;a = sf.shape(0)

&gt;&gt;dir(a)

**Untuk melihat type:**

&gt;&gt; a.shapetype

**Mencari negara:**

&gt;&gt; for a in sf.records():

&gt;&gt;   if a\[8\] == “indonesia”

&gt;&gt;         print a

**Melihat Baris:**

&gt;&gt; Print i

&gt;&gt;   i = i + 1

**Kesimpulan**

Kesimpulannya adalah Dalam data Retrieve ini kita semua dapat melakukan select/view dan menghitung jumlah record. Dengan mendapatkan data shp dan dbf file kita juga belum tentu dapat melihat data tersebut namun kita juga harus menggunakan aplikasi sepert Qgis dan Python untuk dapat melihat atau melakukan view agar data yang kita cari menggunakan retreive.

**Saran:**

                Sebaiknya lebih banyak lagi pengembang yang mempelajari dan menggunakan data-data yang seperti diatas dan mempraktekannya, banyak pengembang yang mengerti tentang data retrieve pada data geospasial.
