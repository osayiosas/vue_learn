<script setup>
import { ref} from "vue"
const isActive = ref(true)

</script>


<template>
    <div v-if="isActive">
        <h1>My vue blog</h1>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium, expedita..v-show
        </p>
    </div>

    <button @click="isActive = !isActive">
        Toggle visibility
    </button>
</template>