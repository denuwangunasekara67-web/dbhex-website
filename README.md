# dbhex-website[index.html](https://github.com/user-attachments/files/26124016/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>DB HEX LOGIN</title>
  <style>
    body {
      background: black;
      color: white;
      font-family: Arial;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .box {
      background: #111;
      padding: 30px;
      border-radius: 10px;
      text-align: center;
      width: 300px;
      box-shadow: 0 0 20px red;
    }

    input {
      width: 90%;
      padding: 10px;
      margin: 10px 0;
      border: none;
    }

    button {
      padding: 10px 20px;
      background: red;
      border: none;
      color: white;
      cursor: pointer;
    }

    button:hover {
      background: darkred;
    }
  </style>
</head>
<body>

<div class="box">
  <h2>DB HEX LOGIN</h2>
  <input type="text" id="user" placeholder="Username">
  <input type="password" id="pass" placeholder="Password">
  <br>
  <button onclick="login()">Login</button>
  <p id="msg"></p>
</div>

<script>
function login() {
  let u = document.getElementById("user").value;
  let p = document.getElementById("pass").value;

  // simple demo login
  if(u === "admin" && p === "1234") {
    window.location.href = "prices.html";
  } else {
    document.getElementById("msg").innerText = "❌ Wrong login";
  }
}
</script>

</body>
</html>
