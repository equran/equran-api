![EQuran.id](https://raw.githubusercontent.com/equran/equran-api/main/equran_id.png "Quran Digital Bahasa Indonesia")
___

## API Developer
___

Berikut ini adalah daftar endpoint API yang tersedia. Sumber utama dari data yang terdapat pada API ini adalah Aplikasi Quran Kementrian Agama Republik Indonesia dan audio murottal Misyari Rasyid Al-'Afasi. Semoga dapat dimanfaatkan sebaik-baiknya.

Saran dan masukan dapat disampaikan ke: equran.id@gmail.com.

___

## Daftar Surat

```
GET https://equran.id/api/surat
```

Contoh Response:
```
[
  {
     "nomor": "1",
     "nama": "الفاتحة",
     "nama_latin": "Al-Fatihah",
     "jumlah_ayat": "7",
     "tempat_turun": "mekah",
     "arti": "Pembukaan",
     "deskripsi": "Surat <i>Al Faatihah</i> (Pembukaan) yang diturunkan di Mekah dan terdiri dari 7 ayat adalah surat yang pertama-tama diturunkan dengan lengkap  diantara surat-surat yang ada dalam Al Quran dan termasuk golongan surat Makkiyyah. Surat ini disebut <i>Al Faatihah</i> (Pembukaan), karena dengan surat inilah dibuka dan dimulainya Al Quran. Dinamakan <i>Ummul Quran</i> (induk Al Quran) atau <i>Ummul Kitaab</i> (induk Al Kitaab) karena dia merupakan induk dari semua isi Al Quran, dan karena itu diwajibkan membacanya pada tiap-tiap sembahyang.<br> Dinamakan pula <i>As Sab'ul matsaany</i> (tujuh yang berulang-ulang) karena ayatnya tujuh dan dibaca berulang-ulang dalam sholat.",
     "audio": "https:\/\/equran.id\/content\/audio\/001.mp3"
  },
  {
     "nomor": "2",
     "nama": "البقرة",
     "nama_latin": "Al-Baqarah",
     "jumlah_ayat": "286",
     "tempat_turun": "madinah",
     "arti": "Sapi",
     "deskripsi": "Surat <i>Al Baqarah</i> yang 286 ayat itu turun di Madinah yang sebahagian besar diturunkan pada permulaan tahun Hijrah, kecuali ayat 281 diturunkan di Mina pada Hajji wadaa' (hajji Nabi Muhammad s.a.w. yang terakhir). Seluruh ayat dari surat Al Baqarah termasuk golongan Madaniyyah, merupakan surat yang terpanjang di antara surat-surat Al Quran yang di dalamnya terdapat pula ayat yang terpancang (ayat 282). Surat ini dinamai <i>Al Baqarah</i> karena di dalamnya disebutkan kisah penyembelihan sapi betina yang diperintahkan Allah kepada Bani Israil (ayat 67 sampai dengan 74), dimana dijelaskan watak orang Yahudi pada umumnya. Dinamai <i>Fusthaatul-Quran</i> (puncak Al Quran) karena memuat beberapa hukum yang tidak disebutkan dalam surat yang lain. Dinamai juga surat  <i>alif-laam-miim</i> karena surat ini dimulai dengan Alif-laam-miim.",
     "audio": "https:\/\/equran.id\/content\/audio\/002.mp3"
  }
```

___

## Detail Surat

```
GET https://equran.id/api/surat/{nomor}
```

Contoh Response:
```
{
  "status": true,
  "nomor": "110",
  "nama": "النصر",
  "nama_latin": "An-Nasr",
  "jumlah_ayat": "3",
  "tempat_turun": "madinah",
  "arti": "Pertolongan",
  "deskripsi": "Surat An Nashr terdiri atas 3 ayat, termasuk golongan surat-surat  Madaniyyah yang diturunkan di Mekah sesudah surat At Taubah.  Dinamai <i>An Nashr</i> (pertolongan) diambil dari perkataan <i>Nashr</i> yang  terdapat pada ayat pertama surat ini.",
  "audio": "https:\/\/equran.id\/content\/audio\/110.mp3",
  "ayat": [
     {
         "nomor": "1",
         "ar": "اِذَا جَاۤءَ نَصْرُ اللّٰهِ وَالْفَتْحُۙ",
         "tr": "i<u>dzaa</u> j<u>aa</u>-a na<u>sh</u>ru <strong>al</strong>l<u>aa</u>hi wa<strong>a</strong>lfat<u>h</u><strong>u</strong>",
         "idn": "Apabila telah datang pertolongan Allah dan kemenangan,"
     },
     {
         "nomor": "2",
         "ar": "وَرَاَيْتَ النَّاسَ يَدْخُلُوْنَ فِيْ دِيْنِ اللّٰهِ اَفْوَاجًاۙ",
         "tr": "wara-ayta <strong>al</strong>nn<u>aa</u>sa yadkhuluuna fii diini <strong>al</strong>l<u>aa</u>hi afw<u>aa</u>j<u>aa</u><strong>n</strong>",
         "idn": "dan engkau melihat manusia berbondong-bondong masuk agama Allah,"
     },
     {
         "nomor": "3",
         "ar": "فَسَبِّحْ بِحَمْدِ رَبِّكَ وَاسْتَغْفِرْهُۗ اِنَّهٗ كَانَ تَوَّابًا ࣖ",
         "tr": "fasabbi<u>h</u> bi<u>h</u>amdi rabbika wa<strong>i</strong>staghfirhu innahu k<u>aa</u>na taww<u>aa</u>b<u>aa</u><strong>n</strong>",
         "idn": "maka bertasbihlah dalam dengan Tuhanmu dan mohonlah ampunan kepada-Nya. Sungguh, Dia Maha Penerima tobat."
     }
  ]
}
```

___

## Tafsir Surat

```
GET https://equran.id/api/tafsir/{nomor}
```

Contoh Response:
```
{
  "status": true,
  "nomor": "110",
  "nama": "النصر",
  "nama_latin": "An-Nasr",
  "jumlah_ayat": "3",
  "tempat_turun": "madinah",
  "arti": "Pertolongan",
  "tafsir": [
     {
         "ayat": "1",
         "tafsir": "Dalam ayat-ayat ini, Allah memerintahkan apa yang harus dilakukan Nabi Muhammad pada saat pembebasan Mekah, yaitu apabila ia telah melihat pertolongan Allah terhadap agama-Nya telah tiba, dengan kekalahan orang-orang musyrik dan kemenangan di pihak Nabi, dan melihat pula orang-orang masuk agama Allah beramai-ramai dan berduyun-duyun, bukan perseorangan sebagaimana halnya pada permulaan dakwah.\n\nOrang-orang Arab berkata, \"Manakala Muhammad menang atas penduduk Mekah yang mana Allah telah selamatkan mereka dari pasukan bergajah, maka kalian tidak berdaya melawannya.\" Akhirnya mereka masuk Islam berduyun-duyun, berkelompok-kelompok dan satu kelompok 40 orang."
     },
     {
         "ayat": "2",
         "tafsir": "Dalam ayat-ayat ini, Allah memerintahkan apa yang harus dilakukan Nabi Muhammad pada saat pembebasan Mekah, yaitu apabila ia telah melihat pertolongan Allah terhadap agama-Nya telah tiba, dengan kekalahan orang-orang musyrik dan kemenangan di pihak Nabi, dan melihat pula orang-orang masuk agama Allah beramai-ramai dan berduyun-duyun, bukan perseorangan sebagaimana halnya pada permulaan dakwah.\n\nOrang-orang Arab berkata, \"Manakala Muhammad menang atas penduduk Mekah yang mana Allah telah selamatkan mereka dari pasukan bergajah, maka kalian tidak berdaya melawannya.\" Akhirnya mereka masuk Islam berduyun-duyun, berkelompok-kelompok dan satu kelompok 40 orang."
     },
     {
         "ayat": "3",
         "tafsir": "Bila yang demikian itu telah terjadi, Nabi diperintahkan untuk mengagungkan dan mensucikan Tuhannya dari hal-hal yang tidak layak bagi-Nya, seperti menganggap terlambat datangnya pertolongan dan mengira bahwa Tuhan tidak menepati janji-Nya menolong Nabi atas orang-orang kafir.\n\nMenyucikan Allah hendaknya dengan memuji-Nya atas nikmat-nikmat yang dianugerahkan-Nya dan mensyukuri segala kebaikan-kebaikan yang telah dilimpahkan-Nya dan menyanjung-Nya dengan sepantasnya. Bila Allah Yang Mahakuasa dan Mahabijaksana memberi kesempatan kepada orang-orang kafir, bukanlah berarti Dia telah menyia-nyiakan pahala orang-orang yang beramal baik.\n\nKemudian Nabi Muhammad dianjurkan untuk meminta ampun kepada Allah untuk dirinya dan sahabat-sahabatnya yang telah memperlihatkan kesedihan dan keputusasaan karena merasa pertolongan Allah terlambat datangnya. Bertobat dari keluh-kesah adalah dengan mempercayai penuh akan janji-janji Allah dan membersihkan jiwa dari pemikiran yang bukan-bukan bila menghadapi kesulitan. Hal ini walaupun berat untuk jiwa manusia biasa, tetapi ringan untuk Nabi Muhammad sebagai insan kamil (manusia sempurna). Oleh sebab itu, Allah menyuruh Nabi saw memohon ampunan-Nya.\n\nKeadaan ini terjadi pula pada para sahabat yang memiliki jiwa yang sempurna dan menerima tobat mereka, karena Allah selalu menerima tobat hamba-hamba-Nya. Allah mendidik hamba-hamba-Nya melalui bermacam-macam cobaan dan bila merasa tidak sanggup menghadapinya harus memohon bantuan-Nya serta yakin akan datangnya bantuan itu. Bila ia selalu melakukan yang demikian niscaya menjadi kuat dan sempurnalah jiwanya.\n\nMaksudnya, bila pertolongan telah tiba dan telah mencapai kemenangan serta manusia berbondong-bondong masuk Islam, hilanglah ketakutan dan hendaklah Nabi saw bertasbih menyucikan Tuhannya dan mensyukuri-Nya serta membersihkan jiwa dari pemikiran-pemikiran yang terjadi pada masa kesulitan. Dengan demikian, keluh-kesah dan rasa kecewa tidak lagi akan mempengaruhi jiwa orang-orang yang ikhlas selagi mereka memiliki keikhlasan dan berada dalam persesuaian kata dan cinta sama cinta.\n\nDengan turunnya Surah an-Nasr ini, Nabi memahami bahwa tugas risalahnya telah selesai dan selanjutnya ia hanya menunggu panggilan pulang ke rahmatullah. \n\nIbnu 'AbbAs berkata: \"Ketika turun ayat Idha jaa nasrullahi wal fath, Rasulullah saw memanggil Fatimah, lalu berkata: \"Kematian diriku sudah dekat.\" Fatimah pun menangis. Rasulullah saw berkata, \"Jangan menangis, karea kamu adalah anggota pertama dari keluargaku yang akan menyusulku.\" Fatimah pun tertawa bahagia (mendengarnya). Para istri Nabi saw yang melihat hal itu berkata, \"Wahai Fatimah, kami melihatmu menangis lalu tertawa.\" Fatimah berkata, \"Rasulullah saw memberitahuku bahwa kematian dirinya telah dekat, maka aku menangis. Namun, beliau mengatakan, \"Jangan menangis, karena kamu adalah anggota pertama dari keluargaku yang akan menyusulku.\" Maka aku pun tertawa bahagia. (Riwayat al- Darimi)\n\nIbnu 'Umar berkata, \"Surah ini turun di Mina ketika Nabi mengerjakan Haji Wada', sesudah itu turun firman Allah:\n\nPada hari ini telah Aku sempurnakan agamamu untukmu, dan telah Aku cukupkan nikmat-Ku bagimu, dan telah Aku ridai Islam sebagai agamamu. (al-Ma'idah\/5: 3)\n\nNabi hidup hanya delapan puluh hari setelah turun ayat ini. Kemudian setelah itu, turun ayat Kalalah, dan Nabi hidup sesudahnya lima puluh hari. Setelah itu turun ayat:\n\nSungguh, telah datang kepadamu seorang rasul dari kaummu sendiri. (at-Taubah\/9:128)\n\nMaka Nabi saw hidup sesudahnya tiga puluh lima hari. Kemudian turun firman Allah:\n\nDan takutlah pada hari (ketika) kamu semua dikembalikan kepada Allah. (al Baqarah\/2: 281)\n\nMaka Nabi saw hidup sesudahnya hanya dua puluh satu hari saja."
     }
  ]
```
___

[![EQuran.id](https://raw.githubusercontent.com/equran/equran-api/main/google_play_200.png "Quran Digital Bahasa Indonesia")](https://play.google.com/store/apps/details?id=id.equran.android)
