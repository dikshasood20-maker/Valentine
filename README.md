<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Be My Valentine 💖</title>
<style>
body{
  margin:0;
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  background:linear-gradient(135deg,#ff9a9e,#fad0c4);
  font-family:Arial,sans-serif;
}
.card{
  background:white;
  padding:30px;
  border-radius:20px;
  text-align:center;
  width:320px;
}
button{
  padding:12px 20px;
  border:none;
  border-radius:25px;
  margin:10px;
  font-size:16px;
}
#yesBtn{
  background:#ff4d6d;
  color:white;
}
#noBtn{
  background:#ccc;
  position:relative;
}
</style>
</head>

<body>
<div class="card" id="card">
  <h1 id="question">Will you be my Valentine? 💘</h1>
  <button id="yesBtn">Yes 😍</button>
  <button id="noBtn">No 🙄</button>
</div>

<script>
const noBtn=document.getElementById("noBtn");
const yesBtn=document.getElementById("yesBtn");
const card=document.getElementById("card");
const question=document.getElementById("question");

noBtn.addEventListener("mouseover",()=>{
  noBtn.style.transform=
    translate(${Math.random()*200-100}px,${Math.random()*200-100}px);
  question.innerText="Are you sure? 😏";
});

yesBtn.addEventListener("click",()=>{
  card.innerHTML="<h1>YAYYY ❤️🥰</h1><p>My Valentine forever 💖</p>";
});
</script>
</body>
</html>
