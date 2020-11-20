```css

input.login {
    background-color: teal;
}

.createNew {
    background-color: #2FC411;
    color: white;
    padding: 2%;
    display: block;
    border-radius: 5%;
    width: 50%;
    margin: 0% auto;
    text-align: center;
}

.card {
    width: 50%;
    margin: auto;
    border: 2px gray solid;
    border-radius: 5%;
    padding: 5%;
}

input {
    width: 100%;
    padding: 5% 0%;
    margin-bottom: 5%;
}

.forgotPassword{
    color: teal;
    text-align: center;
    width: 50%;
    display: block;
    margin: 0% auto;
}

hr {
    margin: 5% 0%;
}
```

```html
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="index.css">
    </head>
    <body>
        <div class="card">
            <form>
                <label for="username">Email or Phone Number</label>
                <br>
                <input type="text" id="username" name="usernane">
                <br>
                <label for="password">Password</label>
                <br>
                <input type="password" id="password" name="password">
                <br>
                <input type="submit" value="Log In" class="login">
            </form>
            <a class="forgotPassword">Forgot Password?</a>
            <hr>
            <a class="createNew">Create New Account</a>
        </div>
        <p style="text-align: center;">
            <a href="/">Create a Page</a> for a celebrity, band or business. 
        </p>
    </body>
</html>
```