# my love
<!DOCTYPE html>
<html lang="mn">
<head>
<meta charset="UTF-8">
<title>For You</title>
<style>
body{
  margin:0;
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  background:linear-gradient(135deg,#ff0033,#b30000);
  font-family:-apple-system;
  overflow:hidden;
}
#box{
  width:160px;
  height:140px;
  background:#ff1a1a;
  position:relative;
  transform:rotate(-45deg);
  cursor:pointer;
  box-shadow:0 0 30px rgba(255,255,255,.4);
  animation:pulse 1.5s infinite;
}
#box:before,
#box:after{
  content:"";
  width:160px;
  height:140px;
  background:#ff1a1a;
  border-radius:50%;
  position:absolute;
}
#box:before{top:-80px;left:0}
#box:after{left:80px;top:0}

@keyframes pulse{
  0%{transform:scale(1) rotate(-45deg)}
  50%{transform:scale(1.1) rotate(-45deg)}
  100%{transform:scale(1) rotate(-45deg)}
}

#msg{
  display:none;
  position:absolute;
  text-align:center;
  color:white;
  font-size:26px;
  font-weight:600;
  animation:fade 1s ease forwards;
}

@keyframes fade{
  from{opacity:0;transform:scale(.8)}
  to{opacity:1;transform:scale(1)}
}
</style>
</head>

<body>
  <div id="box"></div>
  <div id="msg">Suwdaa<br>би чамд хайртай ❤️</div>

<script>
document.getElementById("box").onclick=()=>{
  box.style.display="none";
  msg.style.display="block";
}
</script>
</body>
</html>
