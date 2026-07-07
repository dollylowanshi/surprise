<!DOCTYPE html>
<html>
<head>
  <title>Would You like to go on a date with me?</title>
  <style>
    body{
      font-family: Arial, sans-serif;
      text-align:center;
      margin-top:100px;
      background:#e89c9c;
    }
    button{
      padding:12px 25px;
      margin:10px;
      font-size:20px;
      cursor:pointer;
    }
    #inside h1{
      color:#050303;
      font-style:italic;
      ;
    }
  
  </style>
</head>
<body>

<h1>❤️ Would You like to go on a date with me? ❤️</h1>

<button onclick="yes()">Yes 💖</button>
<button id="no" onmouseover="moveNo()">No 😢</button>

<script>
function yes(){
  document.body.innerHTML =
    "<h1 id ='inside'>Yay! ❤️ You made my day! 🌹</h1>" +
    "<img src='https://images.stockcake.com/public/c/e/b/ceb09fdd-0240-4471-b9b4-51e1e18c19e6_large/romantic-dinner-date-stockcake.jpg' alt='Love Image' style='width:600px;border-radius:15px;box-shadow:0 0 15px rgba(0,0,0,0.3);margin:20px;'>";
}

function moveNo(){
  const btn = document.getElementById("no");
  btn.style.position = "absolute";
  btn.style.left = Math.random() * (window.innerWidth - 100) + "px";
  btn.style.top = Math.random() * (window.innerHeight - 50) + "px";
}
</script>

</body>
</html>
