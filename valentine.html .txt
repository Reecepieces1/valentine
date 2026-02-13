<!DOCTYPE html>
<html>
<head>
<title>Important Question 💘</title>
<style>
body {
  text-align: center;
  font-family: Arial;
  background-color: #ffebf0;
  padding-top: 100px;
}
button {
  font-size: 20px;
  padding: 10px 20px;
  margin: 10px;
  cursor: pointer;
}
#no {
  position: absolute;
}
</style>
</head>
<body>

<h1>Will You Be My Valentine? 💖</h1>

<button onclick="yes()">Yes 😍</button>
<button id="no" onmouseover="moveNo()">No 🙃</button>

<script>
function yes() {
  alert("Best decision you’ve made all year 😌💘");
}
function moveNo() {
  document.getElementById("no").style.top = Math.random()*400 + "px";
  document.getElementById("no").style.left = Math.random()*400 + "px";
}
</script>

</body>
</html>
