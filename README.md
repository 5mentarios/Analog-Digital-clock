<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Reloj</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="clock-container">
    <div class="digital-clock" id="digital-clock"></div>
    <div class="analog-clock">
      <div class="hour-hand" id="hour-hand"></div>
      <div class="minute-hand" id="minute-hand"></div>
      <div class="second-hand" id="second-hand"></div>
      <div class="center-circle"></div>
    </div>
  </div>
  <script src="script.js"></script>
</body>
</html>
CSS
body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  margin: 0;
  background-color: #f0f0f0;
}

.clock-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.digital-clock {
  font-size: 2rem;
  margin-bottom: 20px;
}

.analog-clock {
  position: relative;
  width: 200px;
  height: 200px;
  border-radius: 50%;
  border: 2px solid #333;
}

.center-circle {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 10px;
  height: 10px;
  background-color: #333;
  border-radius: 50%;
}

.hour-hand, .minute-hand, .second-hand {
  position: absolute;
  background-color: #333;
  transform-origin: 50% 100%;
}

.hour-hand {
  width: 6px;
  height: 50px;
}

.minute-hand {
  width: 4px;
  height: 70px;
}

.second-hand {
  width: 2px;
  height: 80px;
}
