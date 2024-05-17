<script setup>

const isTrue = true;
const isFalse = false;

import { ref } from 'vue';

let isVisbale = ref(true);





</script>

<template>
    <div>
        <p v-if="isTrue">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Accusantium, expedita..true
        </p>
        <p v-else-if="isFalse">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Accusantium, expedita..false
        </p>
        <p v-else>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Accusantium, expedita..else
        </p>
    </div>

    <!-- v-show -->

    <p v-show="isVisbale">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Accusantium, expedita..v-show
    </p>
    <button @click="isVisbale =!isVisbale">Toggle visibilty</button>
</template>