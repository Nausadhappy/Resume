
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Form</title>
    <style>
        *{
    box-sizing: border-box;
    opacity: 1;
}
 
body {
  background-image:url(forest.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  font-family:'Times New Roman', Times, serif;
  
}

.container {
  max-width: 600px;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  height: 100vh;
  position: relative;
}

form{
  background-color: #4554;
  backdrop-filter: saturate(180%)blur(20px);
}

form {
   
  padding: 50px;
  border-radius: 30px;
  width: 350px;
  position: relative;
  z-index: 2;
}


.input-group {
  position: relative;
  margin-bottom: 30px;
}

input {
    padding: 15px;
  border-radius: 30px;
  border: none;
  background-color: #333333;
  color:white;
  width: 100%;
  font-size: 16px;
  font-weight:lighter;
font-family: 'Times New Roman', Times, serif;
}

input:focus {
  outline: none;
  transform: translateY(-5px);
}

button:hover{
    transform: translateY(-5px);
}

label {
  position: absolute;
  left: 20px;
  top: 20px;
  font-size: 16px;
  color: #ffffff;
  transition: all 0.3s ease-in-out;
  pointer-events: none;
}

input:focus ~ label,
input:valid ~ label {
  top: -25px;
  font-size: 14px;
  color: #4CAF50;
}


button[type="submit"],
button[type="reset"] {
  border-radius: 30px;
  border: none;
  padding: 15px;
  font-size: 16px;
  font-weight: bold;
  background-color: #4CAF50;
  color: #ffffff;
  cursor: pointer;
  transition: all 0.3s ease-in-out;
  outline: none;
  width: 120px;
}
 button[type="submit"]:hover,
 button[type="reset"]:hover {
  background-color: #333333;
  color: #4CAF50;
}
 h1{
    color:white
 }   
    </style>
    </head>
<body>
    <div class="container">
        <form>
          <h1>Login</h1>
          <div class="input-group">
            <input type="email" name="email" id="email" required>
            <label for="email">Email</label>
          </div>
          <div class="input-group">
            <input type="password" name="password" id="password" required minlength="8" >
            <label for="password" >Password</label>
          </div>
          <button type="reset">Reset</button>
          <button type="submit" formaction="#">Login</button>
        </form>
      </div>
      
</body>
</html>
