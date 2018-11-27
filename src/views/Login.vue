<template>
    <div id="login-wrapper">
        <div class="container">
            <div class="columns">
                <div class="column" id="login-left-panel">
                    <h1 id="login-header">Login</h1>
                    <p>Welcome Back, Please Login to Your Account.</p>

                    <div class="form-input">
                        <label for="email">Email Address</label>
                        <input type="text" name="email" id="email">
                    </div>

                    <div class="form-input">
                        <label for="password">Password</label>
                        <input type="password" name="password" id="password">
                    </div>

                    <div class="columns">
                        <div id="remember-wrapper" class="column">
                            <input type="checkbox" name="remember_me" id="remember_me">
                            <label for="remember_me"> Remember me</label>
                        </div>
                        <div id="forgot-wrapper" class="column">
                            <a href="">Forgot Password</a>
                        </div>
                    </div>
                    <div id="btn-group">
                        <button id="login-btn">
                            Login
                        </button>
                        <button id="back-btn">
                            Register
                        </button>
                    </div>
                    <div>
                        <p id="terms-paragraph">
                            Terms and Conditions <span>&</span> Privacy Policy
                        </p>
                    </div>
                </div>
                <div class="column" id="login-right-panel">

                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'login'
}
</script>

<style scoped>

    #login-wrapper {
    display: flex;
    align-items: center;
    height: calc(100% - 7.5em);
    width: 100%;
    }

    #login-header {
        font-size: 30px;
        color: black;
        font-weight: 600;
    }

    #login-header::first-letter {
        color: #cda34f;
    }

    #login-wrapper > .container > .columns {
        background-color: white;
        box-shadow: 5px 5px #3333;
        min-height: 70%;
    }

    #login-wrapper > .container > .column {
        padding: auto;
    }

    .form-input {
        width: 70%;
        border: 2px solid rgb(241, 241, 241);
        background-color: white;
        border-radius: 3px;
        height: 60px;
        font-size: 12px;
        line-height: 12px;
        border-left: 2px solid #cda34f;
        margin-top: 30px;
        padding: 10px;
        color:rgb(167, 167, 167);
    }

    label {
        display: block;
    }

    input {
        border: none;
        width: 100%;
        font-size: 14px;
        margin-top: 5px;
    }

    input:focus,
    button:focus {
        outline: none;
    }

    #btn-group {
        margin-top: 20px;
    }

    #login-btn {
        background-color: #e9e7da;
        width: 30%;
        height: 45px;
        border: 0px;
        border-radius: 5px;
    }

    #login-btn:hover {
        background-color: #e6e0bb;
    }

    #back-btn {
        background-color: inherit;
        margin-left: 20px;
        width: 30%;
        height: 45px;
        border: 0px;
        border-radius: 5px;
    }

    #back-btn:hover {
        background-color: rgb(235, 235, 235);
    }

    button {
        color: rgb(134, 134, 134);
        font-weight: 600;
    }

    button:hover {
        /* box-shadow: 5px 5px #3333; */
    }

    #login-left-panel {
        padding: 50px;
        background-color: #FCFCFC;
    }

    #login-right-panel {
        background-image: url('../assets/botanical-cactus-close-up-305821.jpg');
        background-repeat: no-repeat;
        background-size: cover;
    }

    p {
        color: rgb(143, 143, 143);
    }

    #remember-wrapper {
        margin: 20px;
        font-size: 12px;
        display: block;
    }

    #remember-wrapper > label,
    #remember-wrapper > input[type=checkbox] {
        width: auto;
        display: inline;
    }

    #forgot-wrapper {
        margin: 20px;
    }

    #forgot-wrapper > a {
        font-size: 12px;
        color: #cda34f;
    }

    #terms-paragraph {
        margin-top: 30px;
        font-size: 12px;
    }
</style>
