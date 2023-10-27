step 1 :
// dokumen write
var hello = "Hello World YAL";
var in_hello = "<h2>" + hello + "</h2>";
document.write(hello);
document.write(in_hello);

var head = document.head;
//cek tipe data
console.log(head);
document.write("tipe objek head : " + typeof head);

document.write("<br>");

var body = document.body;
console.log(body);
document.write(body.innerText);

document.write("<br>");

var title = document.title;
document.write("panjang judul : " + title.length);
document.write("<br>");

step 2:
// document
var p_hello = (document.createElement("p").textContent = "Hello World");
document.body.append("dicetak dengan document element : " + p_hello);

paragraf("belajar js");
document.write("<br>");

function paragraf(kata) {
  var paragraf = (document.createElement("p").textContent = kata);
  document.write("<br>");
  document.body.append(paragraf);
  document.write("<br>");
}