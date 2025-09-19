<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>🎮 Мини-Игры</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background: #f4f4f4;
      margin: 0;
      padding: 20px;
    }
    h1 {
      color: #333;
    }
    .balance {
      font-size: 18px;
      margin: 10px;
    }
    button {
      margin: 5px;
      padding: 10px 15px;
      font-size: 16px;
      cursor: pointer;
      border: none;
      border-radius: 5px;
      background: #3498db;
      color: white;
    }
    button:hover {
      background: #2980b9;
    }
    input {
      padding: 5px;
      font-size: 16px;
      margin-top: 10px;
    }
  </style>
</head>
<body>
  <h1>🎮 Мини-Игры</h1>
  <div class="balance">Баланс: <span id="balance">0</span> 💰</div>

  <button onclick="play('Башня')">🗼 Башня</button>
  <button onclick="play('Краш')">💥 Краш</button>
  <button onclick="play('Голд Мины')">💎 Голд Мины</button>
  <button onclick="play('Бизнес')">🏢 Бизнес</button>

  <div>
    <input type="number" id="amount" placeholder="Введите сумму">
  </div>
  <button onclick="addMoney()">➕ Дать денег</button>
  <button onclick="takeMoney()">❌ Забрать деньги</button>

  <script>
    let balance = 0;

    function updateBalance() {
      document.getElementById('balance').textContent = balance;
    }

    function addMoney() {
      let amount = parseInt(document.getElementById('amount').value);
      if (!isNaN(amount) && amount > 0) {
        balance += amount;
        updateBalance();
      }
    }

    function takeMoney() {
      let amount = parseInt(document.getElementById('amount').value);
      if (!isNaN(amount) && amount > 0 && balance >= amount) {
        balance -= amount;
        updateBalance();
      }
    }

    function play(game) {
      alert("Ты выбрал игру: " + game + " 🚀");
    }

    updateBalance();
  </script>
</body>
</html>
