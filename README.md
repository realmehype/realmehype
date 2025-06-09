<!DOCTYPE html><html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>OriginOS Web</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: sans-serif;
      background: linear-gradient(135deg, #4f46e5, #8b5cf6);
      color: white;
      text-align: center;
      overflow-x: hidden;
      animation: fadeIn 1.5s ease-in;
    }@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

h1 {
  margin-top: 50px;
  font-size: 2.5rem;
  animation: slideDown 1s ease-out;
}

@keyframes slideDown {
  from { transform: translateY(-30px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

.apps {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
  gap: 20px;
  padding: 40px 20px;
  max-width: 600px;
  margin: 0 auto;
}

.app {
  background: rgba(255, 255, 255, 0.1);
  border-radius: 15px;
  padding: 20px;
  transition: background 0.3s, transform 0.3s, box-shadow 0.3s;
  animation: fadeUp 1s ease forwards;
  opacity: 0;
}

.app:nth-child(1) { animation-delay: 0.3s; }
.app:nth-child(2) { animation-delay: 0.5s; }
.app:nth-child(3) { animation-delay: 0.7s; }
.app:nth-child(4) { animation-delay: 0.9s; }
.app:nth-child(5) { animation-delay: 1.1s; }
.app:nth-child(6) { animation-delay: 1.3s; }

@keyframes fadeUp {
  from { transform: translateY(20px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

.app:hover {
  background: rgba(255, 255, 255, 0.2);
  transform: translateY(-5px) scale(1.05);
  box-shadow: 0 8px 15px rgba(0,0,0,0.2);
}

.icon {
  font-size: 2rem;
  margin-bottom: 10px;
  display: block;
  animation: popIn 0.8s ease;
}

@keyframes popIn {
  from { transform: scale(0); opacity: 0; }
  to { transform: scale(1); opacity: 1; }
}

  </style>
</head>
<body>
  <h1>OriginOS Web</h1>
  <div class="apps">
    <div class="app">
      <div class="icon">📷</div>
      <div>Камера</div>
    </div>
    <div class="app">
      <div class="icon">🖼️</div>
      <div>Галерея</div>
    </div>
    <div class="app">
      <div class="icon">⚙️</div>
      <div>Настройки</div>
    </div>
    <div class="app">
      <div class="icon">🎵</div>
      <div>Музыка</div>
    </div>
    <div class="app">
      <div class="icon">📞</div>
      <div>Телефон</div>
    </div>
    <div class="app">
      <div class="icon">🌐</div>
      <div>Браузер</div>
    </div>
  </div>
</body>
</html>
