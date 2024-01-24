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
<-----------------CSS FILE---------------->
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Open Sans", sans-serif;
  }
  
  body {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    width: 100%;
    padding: 0 10px;
  }
  
  body::before {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    background: url("colorful-wallpaper-background-multicolored-generative-ai.jpg"), #000;
    background-position: center;
    background-size: cover;
  }
  
  .container {
    width: 400px;
    border-radius: 8px;
    padding: 30px;
    text-align: center;
    border: 1px solid rgba(255, 255, 255, 0.5);
    backdrop-filter: blur(7px);
    -webkit-backdrop-filter: blur(7px);
  }
  
  form {
    display: flex;
    flex-direction: column;
  }
  
  h2 {
    font-size: 2rem;
    margin-bottom: 20px;
    color: #fff;
  }
  
  .input-field {
    position: relative;
    border-bottom: 2px solid #ccc;
    margin: 15px 0;
  }
  
  .input-field label {
    position: absolute;
    top: 50%;
    left: 0;
    transform: translateY(-50%);
    color: #fff;
    font-size: 16px;
    pointer-events: none;
    transition: 0.15s ease;
  }
  
  .input-field input {
    width: 100%;
    height: 40px;
    background: transparent;
    border: none;
    outline: none;
    font-size: 16px;
    color: #fff;
  }
  
  .input-field input:focus~label,
  .input-field input:valid~label {
    font-size: 0.8rem;
    top: 10px;
    transform: translateY(-120%);
  }
  
  .forget {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 25px 0 35px 0;
    color: #fff;
  }
  
  #Save-login {
    accent-color: #fff;
  }
  
  .forget label {
    display: flex;
    align-items: center;
  }
  
  .forget label p {
    margin-left: 8px;
  }
  
  .container a {
    color: #efefef;
    text-decoration: none;
  }
  
  .container a:hover {
    text-decoration: underline;
  }
  
  button {
