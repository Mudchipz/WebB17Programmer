<h3 id="judul">Belajar JS</h3>
<p id="hasil" style="background-color: aqua"></p>

<span id="nama"></span>
<!-- kasih jarak -->
<br>
<span id="lokasi"></span>

<br />
<br />
<script>
  // deklarasi variabel
  document.getElementById("judul").innerHTML = "Belajar Java Script";

  var hasil = document.getElementById("hasil");
  var nama = document.getElementById("nama");
  var lokasi = document.getElementById("lokasi");

  //   variabel numeric
  var nilai1 = 10;
  var nilai2 = 10;
  var hasilNilai = nilai1 + nilai2;

  console.log("hasil : " + hasilNilai);

  var output =
    "<p style='background-color: yellow; style: block-inline'>Hasil : " +
    hasilNilai +
    "</p>";
  hasil.innerHTML = "Hasil : " + hasilNilai;
  hasil.innerHTML += output;
  document.write(
    "Hasil : <span style='background-color: yellow;'>" +
      hasilNilai +
      "</span>"
  );

  var batas = "===".repeat(10);
  document.write("<br>" + batas + "<br>");

  //variabel string
  var namaStr = "Workshop 4 Days";
  var lokasiStr = "Online";
  nama.innerHTML = namaStr;
  lokasi.innerHTML = lokasiStr;
  
  // yang baru
  // variabel (integer/number, string, boolean, object)
  var nilaiBaru = 25;
  // string "Hello Arif" / all karakter
  // char 'A' / 1 karakter
  // boolean true/false

  //   menggunakan .nama // arif
  //   menggunakan .lokasi // jakarta
  // object {nama: "Arif", umur: 25, lokasi: "Jakarta"}

  // menggunakan [0] // arif
  // menggunakan [1] // 25
  // array ["Arif", 25, 2.5, 'A', true]
  var nilaiLama = ["Arif", 25, 2.5, "A", true];
  var outputVariabel = `nilai lama : ${nilaiLama[0]} <br> dengan tipe 
  data "${typeof nilaiLama}"`;

  //   gak pake variabel
  document.write(
    `nilai baru : ${nilaiBaru} <br> dengan tipe data "${typeof nilaiBaru}"`
  );
  document.write("<br>" + batas + "<br>");
  //   cetak dengan variabel
  document.write(outputVariabel);
</script>

======================== BATAS ========================

<h1>Belajar Kalkulator</h1>
<div id="hasil"></div>
<script>
  var nilai1 = 10;
  var nilai2 = 20;

  // statis
  var hasilTambah = nilai1 + nilai2;
  var hasilKurang = nilai1 - nilai2;
  var hasilKali = nilai1 * nilai2;
  var hasilBagi = nilai1 / nilai2;

  var output = document.getElementById("hasil");
  output.innerHTML = hitung(nilai1, nilai2, "tambah");
  //   output.innerHTML = hasilTambah;

  function hitung(nilai1, nilai2, status) {
    // loigc > + - * /
    var hasil = 0;
    if (status == "tambah") {
      hasil = nilai1 + nilai2;
    } else if (status == "kurang") {
      hasil = nilai1 - nilai2;
    } else if (status == "kali") {
      hasil = nilai1 * nilai2;
    } else if (status == "bagi") {
      hasil = nilai1 / nilai2;
    } else {
      hasil = "Status tidak dikenali";
    }
    var outputFunc = `${nilai1} ${status} ${nilai2} <br> hasil : ${hasil}`;
    // output.innerHTML = outputFunc;
    return outputFunc;
  }
</script>
const hitung = document.getElementById("jumlah");
function cetak() {
        const tulis = document.getElementById("pesan");
        const hitung = document.getElementById("jumlah");
        for (let index = 0; index < hitung; hitung = hitung + 1) {
          tulis.innerHTML = tulis.innerHTML + '<li></li>';
        }return cetak()
      }

      <h3 class="teks" style="padding: 20px; border-radius: 2%">
  Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nihil enim iste
  esse neque laudantium qui odit perspiciatis eius a consequatur maxime
  dolores temporibus tempore illo, aliquid, unde aut voluptates numquam!
</h3>

<h3 class="teks" style="padding: 20px; border-radius: 2%">
  Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nihil enim iste
  esse neque laudantium qui odit perspiciatis eius a consequatur maxime
  dolores temporibus tempore illo, aliquid, unde aut voluptates numquam!
</h3>

<h3 class="teks" style="padding: 20px; border-radius: 2%">
  Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nihil enim iste
  esse neque laudantium qui odit perspiciatis eius a consequatur maxime
  dolores temporibus tempore illo, aliquid, unde aut voluptates numquam!
</h3>

<script>
  var tekt = document.getElementsByClassName("teks")[0];
  tekt.style.backgroundColor = "aquamarine";

  // 0 - 5 (6 data)
  var warna = ["red", "green", "blue", "yellow", "pink", "purple"];
  //saat habis waktu (reset)
  setTimeout(() => {
    tekt.style.color = warna[0];
  }, 2000);
  //set interval
  var i = 0;
  setInterval(() => {
    tekt.style.color = warna[i];
    i++;
    if (i == warna.length) {
      //panjang
      i = 0;
    }
  }, 1000);
</script>
