<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>App Educacional Infantil</title>

<style>
body {
  font-family: Arial, sans-serif;
  background: #f2f7ff;
  text-align: center;
  padding: 20px;
}
.box {
  background: white;
  border-radius: 16px;
  padding: 25px;
  max-width: 350px;
  margin: auto;
}
h1 {
  font-size: 22px;
}
input {
  width: 100%;
  padding: 12px;
  font-size: 16px;
  margin-top: 10px;
}
button {
  margin-top: 15px;
  padding: 14px;
  width: 100%;
  font-size: 18px;
  border-radius: 12px;
  border: none;
  background: #4CAF50;
  color: white;
}
</style>
</head>

<body>

<div class="box">
  <h1>🌍 Aprender desde o início</h1>
  <p>Entre para estudar</p>

  <input type="password" id="senha" placeholder="Digite a senha">

  <button onclick="entrar()">Entrar</button>

  <p id="erro" style="color:red;"></p>
</div>

<script>
function entrar() {
  const senha = document.getElementById("senha").value;
  if (senha === "1234") {
    window.location.href = "home.html";
  } else {
    document.getElementById("erro").innerText = "Senha incorreta";
  }
}
</script>

</body>
</html>
