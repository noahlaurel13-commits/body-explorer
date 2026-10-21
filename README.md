index.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Body Explorer</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background: #101827;
      color: white;
      padding: 20px;
    }
    button {
      padding: 12px 18px;
      margin: 6px;
      border: 0;
      border-radius: 10px;
      background: #38bdf8;
      color: #101827;
      font-size: 16px;
    }
    #info {
      margin-top: 20px;
      padding: 15px;
      background: #243247;
      border-radius: 12px;
    }
  </style>
</head>
<body>
  <h1>🧬 Body Explorer</h1>
  <p>Learn about the parts inside the human body.</p>

  <button onclick="showPart('Skeleton')">🦴 Bones</button>
  <button onclick="showPart('Heart')">❤️ Heart</button>
  <button onclick="showPart('Brain')">🧠 Brain</button>
  <button onclick="showPart('Lungs')">🫁 Lungs</button>

  <div id="info">
    <h2>Welcome!</h2>
    <p>Select a body part to learn about it.</p>
  </div>

  <script>
    const parts = {
      Skeleton: "The skeleton supports your body and protects organs.",
      Heart: "The heart pumps blood throughout your body.",
      Brain: "The brain controls many body functions and helps you think.",
      Lungs: "The lungs help you breathe and exchange oxygen."
    };

    function showPart(part) {
      document.getElementById("info").innerHTML =
        "<h2>" + part + "</h2><p>" + parts[part] + "</p>";
    }
  </script>
</body>
</html>
