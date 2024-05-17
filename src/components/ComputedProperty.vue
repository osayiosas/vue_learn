<script setup>
import {ref, computed} from 'vue' 

const number = ref(4)

const squaredNumber = computed(() => {
    return number.value * number.value

})

const firstName = ref('John')
const lastName = ref('Doe')

const fullName = computed(() => {
    return firstName.value + ' ' + lastName.value
})

const counter = ref(0)

const squaredCounter = computed(() => counter.value ** 2)
</script>


<template>
    <h1>
        Original Number: {{ number }}
    </h1>
    <h1>
        Squared Number: {{ squaredNumber }}
    </h1>

    <h1>
        First Name: {{ firstName }}
    </h1>
    <h1>
        Last Name: {{ lastName }}
    </h1>
    <h1>
        Full Name: {{ fullName }}
    </h1>

    <h1>
        Counter: {{ counter }}
    </h1>
    <p>
        Squared Counter: {{ squaredCounter }}
    </p>
    <button @click="counter++">Increment</button>
</template>