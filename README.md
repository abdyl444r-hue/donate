<!DOCTYPE html><html lang="ru">
<head>
<meta charset="UTF-8">
<title>Магазин доната</title>
<style>
body {
    font-family: Arial;
    background: #0f0f0f;
    color: white;
    text-align: center;
}
.container {
    max-width: 900px;
    margin: auto;
}
.card {
    background: #1c1c1c;
    padding: 15px;
    margin: 10px;
    border-radius: 12px;
    display: inline-block;
    width: 250px;
}
button {
    padding: 10px;
    width: 100%;
    border: none;
    border-radius: 8px;
    background: #ff3b3b;
    color: white;
    cursor: pointer;
}
button:hover {
    background: #ff1f1f;
}
input {
    padding: 10px;
    width: 300px;
    border-radius: 8px;
    border: none;
    margin-bottom: 20px;
}
</style>
</head>
<body><h1>Магазин доната Minecraft</h1>
<p>Введите свой ник</p>
<input type="text" id="nick" placeholder="Ваш ник"><div class="container"><div class="card">
<h3>ELITE</h3>
<button onclick="buy('elite')">Купить</button>
</div><div class="card">
<h3>PREMIUM</h3>
<button onclick="buy('premium')">Купить</button>
</div><div class="card">
<h3>BOSS</h3>
<button onclick="buy('boss')">Купить</button>
</div><div class="card">
<h3>VLADELEC</h3>
<button onclick="buy('vladelec')">Купить</button>
</div><div class="card">
<h3>HELPER</h3>
<button onclick="buy('pomogator')">Купить</button>
</div><div class="card">
<h3>MODERATOR</h3>
<button onclick="buy('modetator')">Купить</button>
</div><div class="card">
<h3>ADMIN</h3>
<button onclick="buy('adm')">Купить</button>
</div><div class="card">
<h3>CO-CREATOR</h3>
<button onclick="buy('sovladelec')">Купить</button>
</div><div class="card">
<h3>CO-OWNER SERVER</h3>
<button onclick="buy('zam')">Купить</button>
</div></div><script>
function buy(product) {
    const nick = document.getElementById("nick").value;

    if(!nick) {
        alert("Введите ник!");
        return;
    }

    window.location.href = 
    "https://mydonate.io/pay/orgeim?product=" + product + "&player=" + nick;
}
</script></body>
</html>
