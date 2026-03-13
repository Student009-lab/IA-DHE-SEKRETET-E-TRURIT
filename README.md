# IA-DHE-SEKRETET-E-TRURIT
KJO FAQE WEB ESHTE KRIJUAR NGA NXENESIT E KLASAVE TE XI NE MENYRE QE PERDORUESIT TE LUAJNE LOJRA ARGETUESE POR GJITHASHTU EDHE TE MARRIN NE KOHE REALE INFORMACIONIN NGA ASISTENTJA JONE AI DONIKA NE LIDHJE ME TRURIN.
<!DOCTYPE html>
<html lang="sq">
<head>
<meta charset="UTF-8">
<title>Donika AI - Projekti i Trurit</title>

<style>

body{
margin:0;
font-family:Arial;
background:linear-gradient(120deg,#0f2027,#203a43,#2c5364);
color:white;
scroll-behavior:smooth;
}

nav{
position:fixed;
top:0;
width:100%;
background:rgba(0,0,0,0.6);
padding:15px;
text-align:center;
z-index:1000;
}

nav a{
color:white;
margin:20px;
text-decoration:none;
font-size:18px;
}

section{
padding:100px 20px;
text-align:center;
}

h1{
font-size:45px;
}

.hero{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
}

button{
padding:15px 35px;
font-size:18px;
border:none;
border-radius:30px;
background:#00c6ff;
color:white;
cursor:pointer;
}

button:hover{
background:#0072ff;
}

.brain{
background:#f4f7fb;
color:black;
}

.brain img{
width:300px;
margin-top:20px;
}

.donika{
background:#141e30;
}

.donika img{
width:350px;
border-radius:20px;
margin-top:20px;
}

.chatbox{
width:450px;
margin:auto;
background:white;
color:black;
padding:20px;
border-radius:15px;
margin-top:30px;
}

.messages{
height:250px;
overflow:auto;
border:1px solid #ddd;
padding:10px;
margin-bottom:10px;
}

input{
width:70%;
padding:10px;
}

footer{
text-align:center;
padding:20px;
background:black;
}

</style>
</head>

<body>

<nav>
<a href="#home">Home</a>
<a href="#brain">Truri</a>
<a href="#donika">Donika AI</a>
</nav>

<section id="home" class="hero">

<h1>Projekti i Trurit 🧠</h1>

<p style="width:60%">
Kjo faqe është ndërtuar nga nxënësit e klasave XI të Gjimnazit
"Asim Vokshi" Tropojë për Festivalin e Shkencave.
Në këtë projekt kemi studiuar trurin, ëndrrat dhe fenomenin déjà vu.
</p>

<a href="#donika">
<button>Pyet Donika AI</button>
</a>

</section>

<section id="brain" class="brain">

<h1>Truri i Njeriut</h1>

<p style="width:65%; margin:auto">
Truri është organi më kompleks i trupit të njeriut.
Ai përmban rreth 86 miliard neurone dhe kontrollon
mendimet, kujtesën, emocionet dhe lëvizjen.
Truri përdor rreth 20% të energjisë së trupit dhe është
qendra e sistemit nervor.
</p>

<img src="https://cdn-icons-png.flaticon.com/512/3774/3774299.png">

</section>

<section id="donika" class="donika">

<h1>Donika AI</h1>

<p>Bëj një pyetje për trurin, ëndrrat ose déjà vu</p>

<img src="donika.jpg">

<div class="chatbox">

<div class="messages" id="chat"></div>

<input id="input" placeholder="Shkruaj pyetjen...">
<button onclick="ask()">Dërgo</button>

</div>

</section>

<footer>
Nxënësit e klasave XI • Gjimnazi Asim Vokshi Tropojë
</footer>

<script>

function ask(){

let input=document.getElementById("input").value;
let chat=document.getElementById("chat");

chat.innerHTML+="<p><b>Ti:</b> "+input+"</p>";

let q=input.toLowerCase();
let answer="";

if(q.includes("truri")){
answer="Truri është organi kryesor i sistemit nervor dhe kontrollon mendimet, kujtesën, emocionet dhe lëvizjen.";
}

else if(q.includes("funksion")){
answer="Funksionet kryesore të trurit janë mendimi, kujtesa, emocionet, koordinimi i trupit dhe kontrolli i organeve.";
}

else if(q.includes("neurone")){
answer="Truri ka rreth 86 miliard neurone që komunikojnë me njëri-tjetrin përmes sinjaleve elektrike dhe kimike.";
}

else if(q.includes("enderr")){
answer="Ëndrrat ndodhin gjatë fazës REM të gjumit kur truri është shumë aktiv dhe përpunon kujtime dhe emocione.";
}

else if(q.includes("pse enderrojm")){
answer="Shkencëtarët mendojnë se ëndrrat ndihmojnë trurin të përpunojë përvojat dhe emocionet e ditës.";
}

else if(q.includes("deja")){
answer="Déjà vu është ndjesia sikur një moment e kemi përjetuar më parë. Mendohet se lidhet me një gabim të vogël në mënyrën si truri përpunon kujtimet.";
}

else if(q.includes("kujtes")){
answer="Kujtesa formohet kur neuronet krijojnë lidhje të reja dhe forcojnë lidhjet ekzistuese.";
}

else if(q.includes("sa energji")){
answer="Truri përdor rreth 20% të energjisë së trupit edhe pse përbën vetëm rreth 2% të peshës së trupit.";
}

else if(q.includes("gjumi")){
answer="Gjatë gjumit truri pastron toksinat dhe përpunon informacionin që kemi marrë gjatë ditës.";
}

else if(q.includes("emocion")){
answer="Emocionet kontrollohen nga sistemi limbik në tru, veçanërisht nga amigdala dhe hipokampusi.";
}

else{
answer="Kjo është një pyetje interesante për trurin. Truri është shumë kompleks dhe shkencëtarët vazhdojnë ta studiojnë çdo ditë.";
}

chat.innerHTML+="<p><b>Donika AI:</b> "+answer+"</p>";

document.getElementById("input").value="";

}

</script>

</body>
</html>
