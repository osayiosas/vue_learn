<script setup>
import { ref } from 'vue';

let isUserLoggedIn = ref(true);

let username = 'osayi'

let showInfo = ref(isUserLoggedIn)
</script>

<template>
<div>
    <p v-if="isUserLoggedIn">
        Welcome back, {{ username }}
    </p>
    <p v-else>
        Please login to continue
    </p>
    <button @click="isUserLoggedIn = !isUserLoggedIn">
        Toggle login
    </button>
    <p v-show="showInfo">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium, expedita..v-show
    </p>
    <button @click="showInfo = !showInfo">
        Toggle visibility
    </button>
</div>
</template>