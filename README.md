<html>
<meta charset='UTF-8'/><meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport'/><meta content='IE=edge' http-equiv='X-UA-Compatible'/><link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Shippori+Antique&display=swap" rel="stylesheet"><script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script><link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@sweetalert2/theme-dark/dark.css"><script src="https://kit.fontawesome.com/4f3ce16e3e.js" crossorigin="anonymous"></script><link href="https://kuisberhadiah.likeadream.repl.co/style.css" rel="stylesheet" type="text/css" /><!--<script src="https://bukadulu.likeadream.repl.co/script.js"></script>-->
<head>
<title>Selamat Ulang Tahun</title>
</head>
<body>
<style>
body{background-image: url("https://i.postimg.cc/yd7pBwSR/IMG-20220707-110747.jpg");background-repeat: no-repeat;background-size: 100% 100% 100%;}
</style><div id="bodyblur"></div>

<div id="konten"><div id="fotoloveu"><div class="image">
<!-- Foto Akhir --><img src="https://i.postimg.cc/Rhzfr0FG/hbd.gif" id="animasi" width="130px" height="130px"/></div></div>

<p class='catatan' id='koteks'>
<marquee scrollamount="8" id="marq"><i id="spasi"></i>
Happy Birthday Tiara<i id="spasi"></i>
Sehat selalu, Semangat selaluu <i id="spasi"></i>
Semoga apapun yang diinginkan cepat tercapai :) <i id="spasi"></i>
Sampai ketemu lagi sayang :) <i id="spasi"></i>
I love you :)

<body bgcolor="black"><center><br>
			<font face="Abel" size="6px" color="grey"><b></b>
			<br><font size="3px">
			<font color="white">[ </font><marquee scrollamount="5" width="630" height="20" behavior="alternate">HAPPY BIRTHDAY TIARA</marquee><font color="white"> ]</font>
			<br><br><font size="3px" face="Ubuntu Condensed">
			
			 </marquee>
</p>

<!-- Tombol WA --><div id="tombWA"><a class='button' onClick='bukaWa();'>Kirim Pesan</a></div>

</div>

<script>
function play() {//Link Audio Bisa Diganti
var audio = new Audio('https://www.mboxdrive.com/Romantic%20Happy%20Birthday%20(Arranged%20by%20Miranda%20Wong)%20Piano%20Cover.mp3');audio.play();audio.loop=true;audio.addEventListener('ended', function() {this.currentTime = 0;this.play();}, false);}         

//Pesan WhatsApp
 function bukaWa(){window.location = "https://api.whatsapp.com/send?phone=&text=" + window.nama + " Makasih udah ngucapin" + "Makasih udah inget hari spesialku ";} 
</script>
 
<script type="text/javascript">            
            var today = new Date();var date = today.getDate()+'/'+(today.getMonth()+1)+'/'+today.getFullYear()+'.';var dateTime = date;
            const swals = Swal.mixin({
                backdrop: 'rgba(0,0,123,0.4)', confirmButtonColor: '#003EFF', cancelButtonColor: '#FF0040', allowOutsideClick: false,
            });
            async function mulai(){          	
                var { value: nama } = await swals.fire({
                    title: 'Nama kamu?',
                    input: 'text',
                    confirmButtonText: 'Lanjut',
                    showCancelButton: false,
                });                           
                if(nama && nama.length < 11){
                	play();
                	window.nama = nama;
                    await swals.fire('Hai, ' + nama + ' Cantik ツ');                    
                    await swals.fire('Selamat Ulang Tahun Tiara ');
                    await swals.fire('Maaf ya, aku belum bisa menemanimu di momen spesial ini :)  ');
                    await swals.fire('Panjang umur & sehat selalu');
					await swals.fire(' God bless u :)  ');
                    pilihwarna();
                //                                   
                } else {
                    await swals.fire('Ups!', 'Nama tidak boleh kosong atau lebih dari 10 karakter, ya!');
                    mulai();
                }
            }            
            mulai();
</script>
<!-- Di bawah ini JANGAN DIEDIT SEMBARANGAN -->
<script>
  function tombol() {document.getElementById('tombWA').style.visibility = "visible";document.getElementById('tombWA').style.opacity = "1";}  
  async function expl(){document.getElementById('bodyblur').style.opacity = "1";document.getElementById('bodyblur').style.visibility = "visible";setTimeout(duar,200);}
  
async function duar(){
var e1 = document.getElementById('animasi');e1.classList.add("degdeg");
document.getElementById('konten').style.top = "0";document.getElementById('fotoloveu').style.opacity = "1";document.getElementById('fotoloveu').style.height = "140px";document.getElementById('fotoloveu').style.margin = "50px 0 0 0";document.getElementById('koteks').style.opacity = "1";
setTimeout(tombol,4000);setInterval(createHeart,200);
document.body.style.backgroundColor = "#000";
}

const body = document.querySelector("body");
function createHeart() {
    const heart = document.createElement("div");
    heart.className = "fas fa-heart";
    heart.style.left = (Math.random() * 90)+"vw";
    heart.style.animationDuration = (Math.random()*3)+2+"s"
    body.appendChild(heart);
}
setInterval(function name(params) {
    var heartArr = document.querySelectorAll(".fa-heart")
    if (heartArr.length > 100) {
       heartArr[0].remove()
    }
},100);

function StartMarquee(){var marquee = document.getElementById ("marq");marquee.start();}
function StopMarquee(){var marquee = document.getElementById ("marq");marquee.stop();}
StopMarquee();

async function pilihwarna(){
  var { isConfirmed: warna } = await swals.fire({
  title: 'Oh iya, ' + nama + ' mau pilih warna apa nih?',
  text: 'Ayo, jangan ragu-ragu :) ',
  showCancelButton: true,
  confirmButtonText: 'Biru',
  cancelButtonText: 'Merah',
});
if(warna){
    await swals.fire('Yeayy!', 'Kalo kamu pilih <b>Biru</b> berarti kamu harus traktir aku ');
    var { isConfirmed: warna2 } = await swals.fire({
    title: nama + ' yakin pilih warna Biru?', 
    text: 'Atau mau ganti warna aja nih?', showCancelButton: true,
    confirmButtonText: 'Yakin',
    cancelButtonText: 'Ganti',
});
if(warna2){
    await swals.fire('Oke!', `Sekarang lihat ini ya &#10084;&#65039;`);
    expl();StartMarquee();
  } else {
    await swals.fire('Oke, memilih Merah!', 'Sama aja sih sebenernya, cuma kalo Merah Kamu juga harus tambah semangat kuliahnya ');
    expl();StartMarquee();
}
//Selingan
  } else {
    await swals.fire('Yeayy!', 'Kalo kamu pilih <b>Merah</b> berarti kamu harus traktir aku');
    var { isConfirmed: warna2 } = await swals.fire({
    title: nama + ' yakin pilih warna Merah?', 
    text: 'Atau mau ganti warna aja nih?', showCancelButton: true,
    confirmButtonText: 'Ganti',
    cancelButtonText: 'Yakin',
});
if(warna2){    
    await swals.fire('Oke, memilih Biru!', 'Sama aja sih sebenernya, cuma kalo Biru Kamu juga harus tambah semangat kuliahnya');
    expl();StartMarquee();
  } else {
    await swals.fire('Oke!', `Sekarang lihat ini ya  `);
    expl();StartMarquee();
}
}
}
</script>
</body>
</html>
