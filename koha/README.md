# Cara Upload File Di Koha ILS

- ### Pada halaman staff klik `tools > upload`

    ![koha](img/koha1.PNG)
    ![koha](img/koha2.PNG)

- ### Klik `browse` untuk memilih file yang akan di upload kemudian centang `Allow public downloads`

    ![koha](img/koha3.PNG)
    ![koha](img/koha4.PNG)

- ### Salin Hashvalue kemudian gabung dengan `http://ils-opac.pilkommedia.edu/cgi-bin/koha/opac-retrieve-file.pl?id=`
    link ini akan menjadi online resource pada saat membuat record.

# Membuat Record Katalog Baru
- ### `cataloging > new record`

    ![koha](img/koha5.PNG)

- ### Pada halaman MARC record ada banyak kolom yang diisi, silahkan isi sesuai kebutuhan
- ### Pada section ke 8 isi kolom `Uniform Resource Identifier` dengan link yang kita gabung dengan hashvalue sebelumnya

    ![koha](img/koha6.PNG)

- ### Setelah itu klik save