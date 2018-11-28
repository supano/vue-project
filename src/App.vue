<template>
    <div id="app">
        <navbar />
        <div id="page-wrapper">
            <transition name="router-anim" enter-active-class="animated fadeInDown" leave-active-class="animated fadeOutDown">
                <router-view/>
            </transition>
        </div>
    </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'

export default {
    components: {
        Navbar
    }
}
</script>

<style>
    @import 'https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.7.0/animate.min.css';

    html {
        height: 100%;
    }

    body {
        background-color: #cda34f;
        height: 100%;
    }

    #app {
        height: 100%;
    }

    #page-wrapper {
        height: calc(100% - 7.5em);
    }

    .page {
        position: fixed;
        width: inherit;
    }
</style>
