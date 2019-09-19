# Install Flutter di Windows 10
Nama    : Vincent Julindra Jacob <br>
NIM     : 20175520007 <br>
Program Studi Teknik Informatika 2017 <br>
Mata Kuliah Pemrograman Mobile 

## Tentang Flutter
Flutter adalah sebuah framework aplikasi mobil sumber terbuka yang diciptakan oleh Google. Flutter digunakan dalam pengembangan aplikasi untuk sistem operasi Android dan iOS, serta menjadi metode utama untuk membuat aplikasi Google Fuchsia. <br>
<img src="https://upload.wikimedia.org/wikipedia/commons/1/17/Google-flutter-logo.png" border="0">

## Jangan Khawatir Jika Laptop Kamu Low Spec, Kita Bisa Install Flutter tanpa pakai Android Studio (yang terkenal berat untuk di jalankan) . Berikut Langkah-langkah install Flutter Tanpa Android Studio : 
- Download SDK Flutter.
  Silahkan kunjungi halaman download <a href="https://flutter.dev/docs/get-started/install/windows"> disini </a>, dan sesuaikan dengan sistem operasi teman teman. Saat tulisan ini dibuat flutter dalam versi 1.9.1 Stable. <br>
 Penampakannya seperti berikut : <br>
 <img src ="1.png">
 - Selanjutnya silahkan download Command Line Tools Only di <a href="https://developer.android.com/studio/#command-tools" > halaman ini </a>, penampakan nya seperti berikut, silahkan download sesuai sistem operasi yang digunakan.
 <img src="https://miro.medium.com/max/1347/1*PKF7u_7UwrmyUlBqX19iFw.png" />
 
 - Silahkan Ekstrak kedua file tersebut dan letakkan di C:\Android untuk windows dan untuk sistem operasi yang lainnya bisa menaruh di root dan buat folder Android. Maka hasilnya akan ada 2 folder yaitu folder flutter dan tools.
 
 - Selanjutnya silahkan download OpenJDK di <a href="https://github.com/AdoptOpenJDK/openjdk8-binaries/releases">halaman ini</a>, dan pilih yang berekstensi zip. sesuaikan dengan sistem operasi yang digunakan, saya menggunakan versi jdk1.8.0_201 . setelah di download jangan lupa untuk mengekstrak ke folder Android yang sudah kita punya sebelumnya dan rename nama folder dari jdk1.8.0_201 menjadi openjdk. totalnya sekarang kita punya 3 folder yaitu flutter, tools dan openjdk.
 
 - sampai sini kita harus menge-set Environment Variable dan Path, untuk windows silahkan buka command prompt dan ketikan command perbaris. <br>
 <code> setx JAVA_HOME “C:\Android\openjdk” </code><br>
 <code> setx ANDROID_HOME “C:\Android” </code> <br> 
 <code> setx ANDROID_SDK_ROOT “C:\Android\tools” </code><br>
 <code> setx path “%path%;”C:\Android\sdk;C:\Android\tools\bin;C:\Android\flutter\bin” </code> <br>
 Setelah anda melakukan command diatas, anda bisa cek Enviroment Variables komputer anda , terlihat di JAVA_HOME, ANDROID_HOME , ANDROID_SDK_ROOT dan di PATH sudah berubah sesuai dengan yang kita set. <br>
 <img src = "enviroment.png">
- Buka terminal (Command Prompt) di C:/Android/tools/bin lalu ketikan beberapa perintah berikut. <br> 
<code> sdkmanager “system-images;android-28;default;x86_64” </code> <br> 
  <code> sdkmanager “platform-tools” </code><br>
 <code> sdkmanager “build-tools;28.0.3” .</code><br>
 <code> sdkmanager “platforms;android-28” </code><br>

  untuk pengguna Mac silahkan jalankan dengan single qoute (petik satu) seperti berikut. <br>
  <code> sdkmanager ‘system-images;android-28;default;x86_64’ </code> <br>
  untuk SDK sendiri, Flutter selalu memerlukan Android SDK yang terbaru. jadi silahkan update sdk dengan command : <br>
  <code> sdkmanager —-update </code> <br>
  Jangan lupa untuk menjalankan syntax accept licenses nya  <br> 
  <code> flutter doctor --android-licenses </code> 
 -  Selanjutnya install Visual Studio Code dan ekstension flutter serta dart nya.
 -  Colok Smartphone anda ke laptop dengan kabel USB, jangan lupa untuk mengaktifkan USB Debugging di Developer Options smartphone anda.
 - Jika semuanya sudah selesai silahkan buka terminal (Command Prompt) di Android/flutter atau untuk pengguna windows bisa double klik di C:\Android\Flutter\flutter_console.bat dan jalankan perintah <code> flutter doctor </code>, maka hasilnya seperti gambar berikut. <br> <img src="flutter ,,.png" /> <br> Abaikan saja jika Android studio tidak terinstall karena kita tidak menggunakannya, atau jika anda ingin melihat yang lengkap bisa mengetikkan perintah <code> flutter doctor -v </code> , hasilnya seperti berikut <br>
  <img src="flutter doctor -v.png">
 = Step terakhir adalah buat project di VsCode dengan klik F1 dan mengetikan Flutter: New Project setelah project selesai di load, klik F5 untuk mendeploy ke android device teman-teman. dan hasilnya seperti gambar dibawah ini


## Info Lebih Lengkap
Website : [www.matanauniversity.ac.id](https://www.matanauniversity.ac.id).  
Mahasiswa Teknik Informatika

