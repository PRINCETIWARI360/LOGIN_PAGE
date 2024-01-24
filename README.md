<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="container">
    <form action="#">
      <h2>Login Form</h2>
      <div class="input-field">
        <input type="text" required />
        <label >Enter email</label>
      </div>
      <div class="input-field">
        <input type="password" required/>
        <label>Enter Password</label>

      </div>
      <div class="forget">
        <label for="save-login" >
          <input type="checkbox" id=" save-login" />
          <p>Save login information</p>
        </label>
        <a href="#">Forget password</a>
      </div>
      <button type="submit">Log in</button>
      <div class="create-account">
        <p>Don't have an account? <a href="#">create-account</a></p>
      </div>
    </form>

  </div>
</body>
</html>
