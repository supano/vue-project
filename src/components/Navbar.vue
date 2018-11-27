<template>
    <nav class="navbar" role="navigation" aria-label="main navigation" id="navbar-wrapper">
        <div class="container">
            <div class="navbar-brand">
                <a class="navbar-item" href="https://bulma.io">
                <img src="https://bulma.io/images/bulma-logo.png" width="112" height="28">
                </a>

                <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
                </a>
            </div>
            <div id="navbarBasicExample" class="navbar-menu">
                <div class="navbar-start">

                </div>

                <div class="navbar-end">

                <router-link to="/" class="navbar-item">Home</router-link>
                <router-link to="/register" class="navbar-item">Register</router-link>
                <router-link to="/login" class="navbar-item">Login</router-link>

                </div>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped>
#navbar-wrapper {
  min-height: 7.5em;
  box-shadow: 0 1px 0 0 rgba(142, 81, 199, 0.05);
}

.navbar {
  border-bottom: 2px solid rgb(233, 233, 233);
}

.navbar-end {
  align-items: center;
}

.navbar-item {
  padding: 10px;
  border-radius: 10px;
}

.navbar-item .is-active {
  background-color: #fbfbfd;
}
</style>
