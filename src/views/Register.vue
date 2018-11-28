<template>
    <div id="register-wrapper" class="page">
        <div class="container">
            <div class="columns">
                <div class="column" id="login-left-panel">
                    <h1 id="login-header">Register</h1>
                    <p></p>

                    <div class="form-input">
                        <label for="email">Email Address</label>
                        <input type="text" name="email" id="email" v-model="email">
                    </div>

                    <div class="form-input">
                        <label for="password">Password</label>
                        <input type="password" name="password" id="password" v-model="password">
                    </div>

                    <div id="btn-group">
                        <button id="login-btn" @click="login">
                            Register
                        </button>
                    </div>
                    <div>
                        <p id="terms-paragraph">
                            Terms and Conditions <span>&</span> Privacy Policy
                        </p>
                    </div>
                </div>
                <div class="column is-three-fifths" id="login-right-panel">

                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'register'
}
</script>

<style scoped>
    #register-wrapper {
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

    #register-wrapper > .container > .columns {
        background-color: white;
        box-shadow: 5px 5px #3333;
        min-height: 70%;
        height: 600px;
    }

    #register-wrapper > .container > .column {
        padding: auto;
    }

    .form-input {
        width: 95%;
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

    #login-left-panel {
        padding: 50px;
        background-color: #FCFCFC;
    }

    #login-right-panel {
        background-image: url('../assets/register-panel-image.webp');
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
