<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>fany textDesigners</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background: #f4f4f4;
      padding: 20px;
    }
    textarea {
      width: 80%;
      height: 60px;
      font-size: 18px;
      padding: 10px;
      margin-bottom: 20px;
    }
    .style {
      margin: 8px auto;
      padding: 10px;
      width: 80%;
      border: 1px solid #ccc;
      border-radius: 5px;
      background: #fff;
      font-size: 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    button {
      padding: 5px 10px;
      border: none;
      border-radius: 5px;
      background: #007bff;
      color: white;
      cursor: pointer;
    }
    button:hover {
      background: #0056b3;
    }
  </style>
</head>
<body>
  <h2>☠Fancy text Designers☠ </h2>
  <textarea id="input" placeholder="Type your text..."></textarea>

  <div class="style" id="arial" style="font-family: Arial;"></div>
  <div class="style" id="times" style="font-family: 'Times New Roman';"></div>
  <div class="style" id="courier" style="font-family: 'Courier New';"></div>
  <div class="style" id="verdana" style="font-family: Verdana;"></div>
  <div class="style" id="georgia" style="font-family: Georgia;"></div>

  <script>
    const input = document.getElementById("input");
    input.addEventListener("input", () => {
      let t = input.value.replace(/[^a-zA-Z ]/g,""); // English only
      document.getElementById("arial").textContent = "Arial: " + t;
      document.getElementById("times").textContent = "Times New Roman: " + t;
      document.getElementById("courier").textContent = "Courier New: " + t;
      document.getElementById("verdana").textContent = "Verdana: " + t;
      document.getElementById("georgia").textContent = "Georgia: " + t;
    });
  </script>
</body>
</html>
