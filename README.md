# Writing Front-End Week 1

## 1. Module-11 React.js Dasar

<br>

### **Pengertian**

React JS adalah sebuah framework yang khusus untuk membuat tampilan menggunakan library JavaScript

![Gambar 1](./1%20Dasar/LogoReact.webp)

*Gambar 1 Reactjs Logo*

Penggunaan Reactjs sangat berguna apabila kita membutuhkan website yang dapat menghandle berbagai data dengan cepat, selain itu juga pada ReactJS dapat membuat program lebih simple dengan cara membagi satu halaman menjadi beberapa komponen

Reactjs sekarang sudah sangat populer digunakan mulai dari komunitas stackoverflow hingga berbagai artikel yang menyebutkan keuntungan menggunakan ReactJS. Tidak hanya sampai disitu, pengembangan menggunakan ReactJS ini dapat digunakan untuk React Native yang khusus membuat tampilan versi mobile

<br><br>

### **Instalasi**

Proses instalasi ReactJs dapat menggunakan salah satu tools yang telah dikembangkan untuk dapat menggunakan berbagai perintah seperti menginstalasi ReactJS

![Gambar 2](./1%20Dasar/NodeJS.png)

*Gambar 2 NodeJs Logo*

Setelah menginstall NodeJs pada komputer, langkah selanjutnya kita dapat menginstall ReactJS dengan menuliskan perintah berikut ini `npx create-react-app myapp` pada sebuah terminal atau git

![Gambar 3](./1%20Dasar/InstallReact.png)

*Gambar 3 Installasi ReactJS*

Tunggu beberapa saat dan project ReactJS berhasil dibuat dengan nama `myapp` pada komputer. Untuk dapat menjalankan program tersebut dapat menuliskan perintah berikut pada terminal project `npm start`

![Gambar 4](./1%20Dasar/ProjectReactJS.png)

*Gambar 4 ReactJS Berjalan pada komputer*

<br><br>

### **ReactJS**

<br>

Membuat sebuah komponen pada ReactJS adalah sebuah keharusan tetapi bukan sebuah kewajiban tergantung dari kebutuhan program yang dibuat. Terbuatnya komponen adalah karena komponen dapat digunakan pada halaman lain. Membuat komponen dapat dilihat pada gambar 5

![Gambar 5](./1%20Dasar/Directory.png)

*Gambar 5 Directory ReactJS*

Untuk membuat komponen sangat mudah, cukup gunakan folder `components` dan berikan file di dalamnya dengan tipe .js

Selanjutnya, ke aplikasi utama `App.js` disini kita akan memanggil sebuah komponen screen ke dalam aplikasi utama dengan cara seperti gambar 6

![Gambar 6](./1%20Dasar/CallComponents.png)

*Gambar 6 Import Component*

![Gambar 7](./1%20Dasar/Component.png)

*Gambar 7 Component Screen*

![Gambar 8](./1%20Dasar/ResultComponent.png)

*Gambar 8 Result Component*

<br>

JSX

<br>

Penggunaan JSX pada ReactJS adalah salah satu cara bagaimana menuliskan sebuah tampilan seperti menggunakan HTML pada Javascript

![Gambar 9](./1%20Dasar/JSX.png)

*Gambar 9 Penggunaan JSX*

Pada Gambar 9 dapat dilihat ada berbagai cara penggunaan JSX, seperti penggunaan Curly Braces `{}` untuk menuliskan sebuah perintah pada HTML, kemudian juga kita dapat menggunakan sebuah function/method pada HTML

![Gambar 10](./1%20Dasar/JSX2.png)

*Gambar 10 Penggunaan JSX*

Pada Gambar 10 dapat dilihat penggunaan sebuah variabel pada JSX

![Gambar 11](./1%20Dasar/JSX3.png)

*Gambar 11 Penggunaan JSX*

Pada Gambar 11 Juga dapat dilihat penggunaan atribut hampir sama dengan penggunaan HTML, bedanya ada beberapa kondisi dia harus menggunakan `{}` sebagai penggunaan perintah

![Gambar 12](./1%20Dasar/JSX4.png)

*Gambar 12 Penggunaan JSX*

Gambar 12 menunjukkan suatu conditional pada JSX, kita dapat menggunakan conditional seperti if... else if... dalam JSX

![Gambar 13](./1%20Dasar/JSX5.png)

*Gambar 13 Penggunaan JSX*

Gambar 13 adalah cara penggunaan dari method `.map()` yang memiliki tujuan untuk mencetak dari isi sebuah Array pada JSX


<br>

Component

<br>

Terdapat dua perbedaan pada component function dan component class

1. Function Component (Stateless Component)

	![Gambar 14](./1%20Dasar/Stateless.png)

	*Gambar 14. Stateless Component*

	Component ini biasanya digunakan untuk mengganti tampilannya saja, sehingga biasanya pada function hanya dapat menerima sebuah data berupa props. Function ini juga biasa dikenal dengan UI Component

2. Class Component (Stateful Component)

	![Gambar 15](./1%20Dasar/Stateful.png)

	*Gambar 15. Stateful Component*

	Component ini digunakan untuk menangani component yang membutuhkan seperti state dan props, yang artinya lebih kompleks dibandingkan mengubah tampilannya saja

State & Props adalah sesuatu yang dimiliki pada stateful, sedangkan stateless tidak memiliki state

State adalah sebuah data lokal yang dapat dikirimkan ke sebuah component yang dituju

![Gambar 16](./1%20Dasar/StateProps.png)

*Gambar 16. Stateful*

Gambar 16 menunjukkan dari baris 18-19 adalah sebuah state yang dikirimkan ke component screen

![Gambar 17](./1%20Dasar/StateProps2.png)

*Gambar 17. Stateless*

Gambar 17 adalah props yang diterima dari class sebelumnya ke component tersebut

<br>

Lifecycle

<br>

Dalam aplikasi yang memiliki banyak komponen tentunya sangat penting untuk menjaga performa dalam mengatur komponen komponen

Contoh dalam kehidupan yaitu mulai dari jam bangun pagi hingga tertidur dan kembali bangun, pastinya ada banyak event yang terjadi. Nah, dalam ReactJS lifecycle ini dapat membantu dalam penggunaan sebuah komponen

![Gambar 18](./1%20Dasar/Lifecycle.png)

*Gambar 18 Lifecycle ReactJS*

Disini akan menggunakan sebuah contoh dalam penggunaan timer, setiap kali Clock dirender ke DOM ke pertama kali dapat menggunakan "mount" pada React. Untuk menghapus atau mereset waktu dapat menggunakan "unmount"

![Gambar 19](./1%20Dasar/Lifecycle2.png)

*Gambar 19 Lifecycle Timer*

![Gambar 20](./1%20Dasar/Lifecycle3.png)

*Gambar 20 Lifecycle Timer*

Dari gambar 19 dan 20 adalah penerapan dari lifecycle method dimana method componentDidMount() akan berjalan setiap kali dirender dan waktu akan berjalan secara terus menerus

Dan ketika komponen Clock dihapus dari DOM, React akan memanggil komponen componentWillUnmount() sehingga timer diberhentikan


<br>

Styling

<br>

Ada beberapa cara styling pada React

1. Inline Styling

	![Gambar 21](./1%20Dasar/Styling.png)

	*Gambar 21 Inline Styling*

	Penggunaan ini langsung pada JSX atribut

2. Object Styling

	![Gambar 22](./1%20Dasar/Styling2.png)

	*Gambar 22 Object Styling*

	Penggunaan ini menggunakan Object pada `render()` dan pada JSX cukup memanggil nama dari salah satu objectnya

3. CSS Stylesheet

	![Gambar 23](./1%20Dasar/Styling3.png)

	*Gambar 23 Import Styling*

	![Gambar 24](./1%20Dasar/Styling4.png)

	*Gambar 24 External Styling*

	Penggunaan ini direkomendasikan agar styling dan jsx terpisah dengan baik