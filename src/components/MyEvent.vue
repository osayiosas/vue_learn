<script setup>
import { ref } from 'vue'
  let count = ref(0)

    const increment = () => {
        count.value++
    }

    const decrement = () => {
        count.value--
    }

    const submitHandler = (e) => {
        e.preventDefault()
        alert('Submitted')
    }

    const showMessage = (message) => alert(message)
</script>

<template>
    <h1>
        Count: {{ count }}
    </h1>
    <!-- <button v-on:click="count++">Increment</button> -->
    <button @click="increment">Increment</button>
    <button @click="decrement">Decrement</button>

    <form @:submit="submitHandler">
        <input type="text" placeholder="enter your name">
        <input type="email" placeholder="enter your email">
        <button type="submit">Submit</button>
    </form>

    <button @click="showMessage('we can make this happen again and again')">Hello vue</button>
</template>